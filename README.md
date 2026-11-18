# My Project
1. Git이란?
Git은 내가 작성한 코드의 변경 이력을 기록하고 관리하는 도구
2. Git의 핵심 구조 3가지
** Working Directory → Staging Area → Repository
 #1. Working Directory : 실제 코드를 작성하고 수정하는 작업 공간 ex) hello. py 작성
 #2. Staging Area : 다음 버전에 기록할 파일을 골라 놓는 공간 ex) hello.py를 다음 커밋에 포함하도록 선택
 #3. Repository : 선택한 병경사항을 하나의 버전으로 기록하는 공간 ex) Create hello.py로 저장
  3. 오늘배운 명령어 하나씩 이해하기
 - git inint : git 시작하기
 - git status : 현재상태 확인하기
 - git add: 커밋할 파일 선택하기
    ㄴ 전체파일을 포함 : git add .
 - git commit - "~~~" : 버전 기록하기
 - git log : 과거 기록 확인하기
  ** HEAD : 현재 내가 위치한 커밋을 가리키는 참조
  4. branch는 왜 필요한가.
브랜치는 기존 프로젝트에 영향을 주지 않고 별도로 작업할 수 있도록 만든 작업 흐름.
- 브랜치 생성 : git branch feat/api
- 브렌치 이동 : git switch feat/api
- 현재 브랜치 확인 : git branch
5. Merge는 무엇인가.
따로 작업한 내용을 합치기.
6. Fast-Forward와 3-way Merge
 #1. Fast- Forward Merge : 한쪽 브랜치만 작업이 진행된 상황
 #2.3-way Merge : main에서도 작업하고 feat/login에서도 작업
 7. 전체 흐름
```text
작업 폴더 생성
  ↓
git init (로컬 저장소 초기화)
  ↓
VS Code에서 파일 작성 및 저장
  ↓
git status (상태 확인)
  ↓
git add (커밋할 변경사항 선택)
  ↓
git commit (버전 기록)
  ↓
git branch / git switch (작업 브랜치 생성·이동)
  ↓
브랜치에서 추가 작업 및 커밋
  ↓
main으로 이동 → git merge (병합)
  ↓
작업 브랜치 삭제₩