# 시선 스터디 - Git/Git Hub
## Day1
  *[스터디 url] : (https://ccss17.github.io/ProgrammerBase/git/)*

- **git과 github의 차이점**
  * git -> 개인의 local에서 코드 편집 등 가능
  * github -> local 의 내용을 github 사이트에 원격으로 게시 할 수 있음 (sns?)



- **init, add, commit -m 명령어**
  * ``git init`` : git 시작,초기화 (untracked 상태)
  * ``git add .`` : git에 추가하기 (untracked -> staged 상태)
  * ``git commit -m "<memo>"`` : git에 commit (staged -> committed 상태)



- **remote, clone, push, pull 명령어**
  1. remote 명령어
  * ``git remote add <NAME><URL>`` : url 과 원격 연결
  * ``git remote rename <NAME><NEW>``
  * ``git remote rm <NAME>``
  2. clone 명령어 - ``git clone <URL><NAME>``
  3. push 명령어 - ``git push <NAME><BRANCH>``
  4. pull 명령어 - ``git pull <NAME><BRANCH>``

![github](https://i.ytimg.com/vi/0nqJKEh3YCc/maxresdefault.jpg)

---

## Day2
  *[스터디 url] : (https://hgusight.github.io/study/github/git2/)*

- **branch, checkout 명령어**
  * ``git branch`` : 현재 상주 하고 있는 브랜치 출력
  * ``git branch <NAME>`` : 새로운 브랜치를 만든다.
  * ``git chekout`` : 브랜치로 이주
  * ``git checkout -b`` : 브랜치 생성과 동시에 이주 

- **merge 2가지 설명**
  1. fast-forward
   *  명령어 ``git merge <NAME>`` : 브랜치를 현재 브랜치로 병합
  2. Merge conflict
   * 커밋 후 ``git status`` 명령어 실행, both modified: 에 해당하는 파일 목록에서 충돌이 발생하는 파일을 확인하여 코드 수정 후 다시 커밋 => 병합 완료