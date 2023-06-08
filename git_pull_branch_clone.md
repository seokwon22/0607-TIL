# Git 특강 2일차

## 초기 원격저장소 설정하는법 쉽게 외우기
```
$ git remote add origin https://github.com/seokwon22/test.git
    원격저장소 추가해 origin으로
```
진짜로 명령을 내리듯이 생각하면서 하면 쉽게 외워짐.

## pull
- 나/다른 사람의 커밋을 받아오는 명령어

## pull 시 유의사항
- 버전 히스토리가 같아야 한다. 만약 서로 버전이 다르다면 pull으로 받아온 다음 수정 후 다시 push 해야한다.


## branch

- ## branch 주요 명령어
    1. 브랜치 생성
    ```
    (main) $ git branch {branch name}
    ```
    2. 브랜치 이동
    ```
    (main) $ git checkout {branch name}
    ```
    3. 브랜치 생성 및 이동
    ```
    (main) $ git checkout -b {branch name}
    ```
    4. 브랜치 목록
    ```
    (main) $ git branch
    ```
    5. 브랜치 삭제
    ```
    (main) $ git branch -d {branch name}
    ```

## branch merge
- 각 branch에서 작업을 한 후 이력을 합치기 위해 merge를 사용
- 다른 branch에서 커밋하고 main으로 돌아와 merge로 병합

## merge 명령어
```
(main branch에서) merge branch '{branch name}'
```

## 원격에 있는 프로젝트를 시작할 때
`git clone` 사용
- 상대방의 repository에서 fork 누르고 클론 생성 후 터미널에 

`git clone http://github.com/seokwon22/프로젝트명`

입력하면 폴더 생성됨.

- vs code에서 파일 작성 후 init 하지말고 commit 후 push

- 마지막에 pull requests 하면 된다.