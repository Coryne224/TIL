# Branch

1. git branch

- 브랜치 조회, 생성, 삭제 관련 명령어

```bash
# 브랜치 목록 확인
git branch

# 브랜치 생성
git branch 신규브랜치명

# 브랜치 삭제
git branch -d 브랜치명
git branch -D 브랜치명 # 강제삭제 옵션
```

2. git switch

- 다른 브랜치로 이동하는 명령어

```bash
# 브랜치 이동
git switch 다른브랜치명

# 브랜치 생성 후 이동
git switch -c 다른브랜치명
```

3. git merge

- 분기된 브랜치들을 합치는 명령어

  ``` bash
  # 주의! 내가 기준으로 가지고 있을 브랜치에 위치
  git switch master
  git merge 브랜치명 # 실습에서는 water
  ```

+) git diff

- 커밋들 사이 변경사항의 차이를 보여주는 명령어

``` bash
# 각 커밋들의 해쉬값 확인
git log --oneline

# 해쉬값들은 log를 통해 확인
git diff 해쉬값 해쉬값
```



# Git workflow

[1] 원격 저장소 소유권이 있는 경우 (Shared repository model)

[2] 원격 저장소 소유권이 없는 경우 (Fork & Pull model)



## 실습

fork&pull model 로 진행

1. educhelsea/acrostic-poem 에서 fork하기
2. 나의 깃허브로 들어와서 code 복사하기
3. 홈에서 gitbash 열고 git clone acrostic-poem로 복사해줌
4. cd acrostic-poem으로 디렉토리 이동
5. acrostic-poem에서 code . 으로 vscode 실행
6. git branch dongho로 생성
7. git switch dongho로 branch이동
8. 파일 작성 및 저장 후 add , commit  (good으로 함)과정 거침
9. git push origin dongho 로 github로 push하기
10. 깃허브에 들어가서 pull request 과정하면 내가 fork한 상대에게 내가 변경한 내용이 가짐

