# my-repo
생활코딩 git 공부

commit - 버전이 만들어졌다.

파일 수정 저장 하면 change에 표시 -> commit(버전생성한다)

push - 버전을 원격저장소에 올린다.

pull - 사람들이 올린게 있나? 확인
       원격저장소 -> pull -> 지역저장소

clone - 복제

working -> staging area -> repository
수정한 파일  -> 수정 한것중 버전만들것 -> 버전 완료
1. git init .
- 깃을 이제 시작한다  '.'은 현재 디렉토리에 시작한다.
- initialize repository

2. git status
- working tree status

3. git add hello.txt
- commit을 할수 있는 상태로 만들다
- add to staging area

4. git commit -m "message 1"
- 커밋

5. git log
- 커밋 버전 확인

6. git log --stat
- 버전의 파일 구성 확인 가능

7. git diff
- show chagens
- 수정 내용 확인

8. git reset --hard
- 마지막 버전으로 변경
- 수정 했던게 마지막 버전으로 원복

9. git log -p
- 버전간 차이점 비교

10. git checkout
- git checkout <commit number:git log에서 확인가능>
- git checkout master  : 최신 버전으로 변경

11. git commit -am "Message 5"
- -am : add 와 commit을 한번에 한다.
- 최초 add 하지 않으면 하지 않는다.

12. git add .
- 하위폴더 전부 add 한다.

13. git reset --hard <commit number:git log에서 확인>
- 삭제
- commit number으로 리셋한다. 으로!!!가고자 하는 커밋 번호로 
-협업 할때 조심.... 

14. git revert <최신버전 commit number>
- 버전을 역순으로 차례대로 해야한다. 최신버전 순으로 하나하나 해야한다.
- 되돌리기
- 최신버전 이전으로 되돌린다.

!!diff tool 검색해보기
!!파일명.gitignore 버전관리하기 싫을때 무시하고 싶은 파일 이름
!!branch
  - 저장소이름을 바꾸지 않고, 각각 나눌수 있음 동일 파일에 내용 조금 변경
  
15. git add orgin https:github.com/numbercyi/my-repo.git
- orgin 별명
- https:github.com/numbercyi/my-repo.git 원격저장소 주소
- 원격저장소 연결

16. git remote / git remote -v
- 연결 확인

17. git push --set-upstream origin master
- 한번만 해주면 된다.
- 지역저장소는 여러 원격 저장소랑 연결 가능 한데 기본적으로 어떤거랑 연결 할것인가.

18. git clone <clone address>
- 원격 저장소를 로컬에 복제한다.

19. git pull
- 가져온다.
