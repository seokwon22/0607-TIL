# 기초 파일 시스템 명령어 & Git 명령어

## 기초 파일  시스템 명령어

- pwd (print working directory) : 현재 디렉토리 출력

- cd (change directory) : 디렉토리 이동
    - `.` : 현재 디렉토리, `..` : 상위 디렉토리

- ls (list) : 목록

- mkdir (make directory) : 디렉토리 생성

- touch : 파일 생성

- rm 파일명 : 파일 삭제
    - rm -r 폴더명 : 폴더 삭제하기


## git 명령어

- git init : 로컬 저장소 생성 (git 초기화)

- git add : 특정 파일/ 폴더의 변경사항 추가
    - git add **.** : 모든 파일의 변경사항 추가

- git commit -m '커밋메시지' : 커밋 (버전 기록)

- git status : 상태 확인

- git log : 버전 확인

## git 명령어 +
- git remote rm origin : 삭제
- git remote -v : 원격저장소 목록 조회