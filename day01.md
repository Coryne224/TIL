# CLI

- CLI vs GUI

- 커멘드라인 명령어

  ``` bash
  # 디렉토리 생성
  mkdir
  # 디렉토리 이동
  cd
  # 파일을 생성
  touch
  # 디렉토리 안 리스트를 확인
  ls
  # 제거
  rm
  ## - r옵션 : 재귀적
  ## -rf :강제 삭제
  #이동/ 경로 변경
  mv
  # 현재의 경로를 보여줌
  pwd
  #화면 깨끗이/스크린 올리기
  clear
  ctrl+L
  
  ```

# 마크다운

​	마크업과 마크다운

​	마크업

- 마크다운 역할
- 마크다운 문법

	1. 제목 : # ~ #######

	2. 목록 : \-, \*,\+ 들여쓰기와 내어쓰기( tab , shift + tab)

	3. 강조

    - *기울임* : \*강조*
    -  **굵게** : \**글자**
    - ***기울이고 굵게*** : ***글자***

	4. 코드

    - 인라인: \`한줄코드` 백틱으로 묶어주기

    - 코드 블럭 : 여러줄 코드를 백틱으로 3개 묶어주기

      ``` python
      print('hello git!')
      ```

      

	5. 링크

    - [보여줄이름](www.naver.com)

	6. 이미지

    \![보여줄이름]\(링크나 사진관련 주소)

    ![구글](https://media.vlpt.us/images/suzieep/post/a137794d-1f46-4af8-ac58-954d4dc0696f/logo-python.png)

	7. 구분선:\---

	8. 표: ctrl + t, command  + t

	9. 인용 

\> 인용 (>개수에 따라 바뀜)



# git 기초

- git의 3공간
  - 분장실,무대,사진 촬영본
  - working directory, staging are, commits



- git 명령

  - git init
    - 맨처음 1회, 절대 홈폴도에서 하지 않는다.
    - git init한 폴더의 하위폴더에서 절대 git init하지 않는다
  - git add
  - git commit -m "메시지"
  - git status
  - git log: 커밋 내역확인
    - --oneline : 한줄 출력

- git 초기 설정

  - git config 

    ``` bash
    git config --global user.name "이름"
    git config --global user.email "유저이메일" # 깃허브에서 사용
    ```



---

# TIL

`Today I Learned`: 하루하루 배웠던 내용을 기록하는 repository

