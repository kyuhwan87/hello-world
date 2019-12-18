# hello-world

원격 저장소 
나의 작업을 온라인에 저장 
소스코드백업 + 협업 
깃허브 사이트에 올라와 있는 소스역시 사용가능 
소스코드 공유가능 

드롭박스 or 구글드라이브 사용가능(솔로 프로젝트일때 )

브랜치 로나누어 작업
컨트리뷰트 : 접근가능한 인원의 숫자 

프로젝트소개도 작성가능 

"포크" : 다른사람의 프로젝트를 복제 수정 가능 단, 내가 복사한 것에 한해서 
자신의 프로젝트를 포크해 가는 경우도 있다

"git"이 우선 필요 
"시그윈"이라는 프로그램을 기반으로 제작된 프로그램 (리눅스 ->win)
git bash 를 사용 


pwd : 현재 내가 작업할 경로 확인

cd Documents/

$ mkdir gitfth: gitfth이라는 작업 폴더 생성(mkdir)

$ cd gitfth : gitfth 여기로 가자 (cd)

$ git

<버젼 확인, 설정 관리>
usage: git [--version] [--help] [-C <path>] [-c <name>=<value>]
           [--exec-path[=<path>]] [--html-path] [--man-path] [--info-path]
           [-p | --paginate | -P | --no-pager] [--no-replace-objects] [--bare]
           [--git-dir=<path>] [--work-tree=<path>] [--namespace=<name>]
           <command> [<args>]

These are common Git commands used in various situations:

start a working area (see also: git help tutorial) 작업을 시작할꺼면 
   clone     Clone a repository into a new directory '클론' 명령어나 
   init      Create an empty Git repository or reinitialize an existing one '이닛' 명령어를 사용해라
   : 현재 디렉토리에서 작업을 시작하겠다는 뜻 (이니시 )

work on the current change (see also: git help everyday)
   add       Add file contents to the index
   mv        Move or rename a file, a directory, or a symlink
   restore   Restore working tree files
   rm        Remove files from the working tree and from the index

examine the history and state (see also: git help revisions)
   bisect    Use binary search to find the commit that introduced a bug
   diff      Show changes between commits, commit and working tree, etc
   grep      Print lines matching a pattern
   log       Show commit logs
   show      Show various types of objects
   status    Show the working tree status

grow, mark and tweak your common history
   branch    List, create, or delete branches
   commit    Record changes to the repository
   merge     Join two or more development histories together
   rebase    Reapply commits on top of another base tip
   reset     Reset current HEAD to the specified state
   switch    Switch branches
   tag       Create, list, delete or verify a tag object signed with GPG

collaborate (see also: git help workflows)
   fetch     Download objects and refs from another repository
   pull      Fetch from and integrate with another repository or a local branch
   push      Update remote refs along with associated objects

'git help -a' and 'git help -g' list available subcommands and some
concept guides. See 'git help <command>' or 'git help <concept>'
to read about a specific subcommand or concept.
See 'git help git' for an overview of the system.

ls -al : 현재 디렉토리의 파일목록을 보여줌 
drwxr-xr-x 1 propa 197121 0 12월 19 01:37 .git/ (.git 폴더 생긴거 보이제? 버젼관리시 이 폴더안에 버젼의 정보가 저장되므로 즁요한 디렉토리 )

버전설정을 위해 (빔, vim) 이라는 에디터를 사용하는데 다깔려잇음 ㅇㅇ 

//파일을 생성합니다. 
vim f1.txt
파일 생성후에는 어떠한 문자도 입력되지 않는다. ( 알파벳 I 를 눌러주면 다시 입력가능함)





//git이 파일을 추적하도록 명령합니다. 
git add f1.txt

//프로젝트 폴더의 상태를 확인합니다. 
git status







