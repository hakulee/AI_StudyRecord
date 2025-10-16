# git 기본 명령어

## 1. Git 설치 및 초기 설정
- git 버전 확인
  ```bash
  git --version
  ```
- 사용자 정보 설정
  ```bash
  git config --global user.name "홍길동"
  git config --global user.email "gildong@example.com"

  # 설정 확인
  git config --list
  ```
  > 이렇게 설정하면 이후 생성하는 모든 로컬 저장소에서 동일한 사용자 정보가 사용됩니다.
  > 프로젝트마다 다른 정보가 필요할 경우, 해당 프로젝트 폴더에서 --global 옵션 없이 설정할 수 있습니다.

- 줄바꿈 문자 설정
  - 윈도우와 맥에서 줄바꿈 문자(개행 문자)가 다르게 저장될 수 있으므로, 협업 시 문제를 방지하기 위해 설정을 통일하는 것이 좋습니다.
  - 터미널에서 다음 명령어를 입력합니다.
  - Mac
    ```bash
    git config --global core.autocrlf input
    ```
  - Window
    ```bash
    git config --global core.autocrlf true
    ```

## 2.로컬 저장소 초기화 및 기본 명령어
- 로컬 저장소 초기화 (git init)  
  새 프로젝트 디렉토리 내에서 Git을 초기화하면, 해당 디렉토리가 로컬 저장소로 등록됩니다.
  ```bash
  mkdir my-git-project
  cd my-git-project
  git init
  ```
  이 명령어를 실행하면, 숨겨진 .git 디렉토리가 생성되며, 이후 커밋 이력과 Git 설정 정보가 이곳에 저장됩니다.

- 파일 추가 및 커밋
  - 파일 생성 및 수정  
    예를 들어, ```README.md``` 파일을 생성하고 내용을 작성합니다.
    ```bash
    # My Git Project
    이 저장소는 Git 기본 명령어 실습을 위한 예제 프로젝트입니다.
    ```
  - 
