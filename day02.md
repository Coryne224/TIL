# 2일차 정리

- 1일차 복습 (Markdown)
  - typora 활용



## github

1. 회원가입 후 (git에서 설정한 username 과 useremail과 동일)

2. Repository default branch를 master로 변경 - (Repository를 master로 생성)

   



## 명령어

``` bash
# 항상 자료가 저장되었는지 확인하고 진행
git init
git touch 파일
git add 파일
git commit - m "이유"

# 원격저장소에 연결시키기 git remote add <이름><주소>
git remote add origin 

# 원격저장소 조회
git remote -v 

# 원격저장소 연결 끊기
git remote rm <이름>


#원격이 확인이 되면
add -> commit -m -> git --logonetime(확인용도) -> git push origin master (원격저장소로 자료 올리기) 
```





## Read ME로 자료 올리기

- `README.md`는 원격 저장소의 소개와 설명이 담겨있는 일종의 대문 역할을 합니다.
- 반드시 파일 이름을 `README.md`로 지정해야 Github가 인식할 수 있습니다.
- 홈 디렉토리에 있는 TIL 폴더에 `README.md` 파일을 생성하고, 자유롭게 `설명, 각오, 분류 등`을 마크다운 문법으로 작성하고 자신의 Github TIL 원격 저장소에 push를 해봅니다.

touch README.md로 파일 만든 후 작성

touch -> add -> commit -m -> push origin master 과정을 거쳐 원격저장소(github)에 올림



READ.md의 자료는 github에서 겉표지 처럼 바로 볼수 있음.  



## .gitignore

> 특정 파일 혹은 폴더에 대해 Git이 버전 관리를 하지 못하도록 지정하는 것

- 반드시 이름을 .gitignore로 작성합니다. 앞의 점(.)은 숨김 파일이라는 뜻입니다.

- 제외 하고 싶은 파일은 반드시 git add 전에 .gitignore에 작성합니다.

 ❗ **왜 git add 전에 .gitignore에 작성해야 할까요?**

`git add a.txt` 라고 작성하면, 이제 Git은 `a.txt`를 버전 관리의 대상으로 여깁니다. 한 번 버전 관리의 대상이 된 `a.txt`는 이후에 .gitignore에 작성하더라도 무시되지 않고 계속 버전 관리의 대상으로 인식됩니다.

따라서 제외 하고 싶은 파일은 반드시 git add 전에 .gitignore에 작성해야 합니다!



1. TIL폴더를 만든 후 해당 폴더에서 vscode 실행
2. touch .gitignore로 파일을 만들어줌
3. https://gitignore.io/ 에서 본인 환경에 따라 .gitignore에 넣거나 , 제외하고 싶은 파일을 .gitignore에 넣어줌
4. add -> commit -m -> push origin master 과정을 거쳐 원격저장소(github)에 올림



## clone, pull

clone - 복제, 원격저장소에 있는 자료를 그대로 복사해서 내 pc에 가져올수 있음 (그대로 다운됨)

pull - push와 반대로 원격저장소(github)에 있는 자료를 내 pc에 가져올수 있음



- clone

1. home 에 새로운 폴더를 만든다 (TIL-class)
2. git clone <주소> <로컬저장소 파일>
3. git init을 사용하지 않아도 원격저장소에 있는것 그대로 가져오기 가능



- pull

1. git pull origin master 로 이미 연결된 원격저장소(github)의 버전을 가져옴
2. 만약 원격저장소에 있는 내용과 로컬pc에 있는 자료가 다르면 오류가 발생하므로 해당 오류를 어떻게 할지 정한 후 다시 add -> commit -m -> push과정을 거쳐 원격저장소에 자료를 올려주면 된다.

