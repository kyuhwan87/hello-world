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

//현재 디렉토리를 git의 (버전) 저장소로 만듭니다. 
git init


ls -al : 현재 디렉토리의 파일목록을 보여줌 
drwxr-xr-x 1 propa 197121 0 12월 19 01:37 .git/ (.git 폴더 생긴거 보이제? 버젼관리시 이 폴더안에 버젼의 정보가 저장되므로 즁요한 디렉토리 )

버전설정을 위해 (빔, vim) 이라는 에디터를 사용하는데 다깔려잇음 ㅇㅇ 

//파일을 생성합니다. 
vim f1.txt
파일 생성후에는 어떠한 문자도 입력되지 않는다. ( 알파벳 I 를 눌러주면 다시 입력가능함: 끼워 넣기)

source : 1 (f1.txt에 데이터 입력 )

$  cat f1.txt : f1.txt 내용 살펴보기 
:wq (문서 빠쪄나오기)(write + quit)


//git이 파일을 추적하도록 명령합니다. 
git add f1.txt :관리해야할 파일을 명확하게 하기 위해서 

//프로젝트 폴더의 상태를 확인합니다. 
git status

작업이 완료된 상태  = 버전 
버젼 만들때 이름을 정해 주어야 한다 .

만약 vim이 아니라 nano와 같은 에디터가 실행되면 아래 명령을 사용하시면 됩니다.
git config --global core.editor "vim"  

버전에 포함될 버전을 만든 사람에 대한 정보를 설정합니다. 이 설정은 ~/.gitconfig 파일에 저장되고 1번만 해주면 됩니다.

git config --global user.name "자신의 닉네임"
git config --global user.email "자신의 이메일"

<커밋하기>
1. $ git status (상태확인 )
~~~ modified:   f1.txt
no changes added to commit (use "git add" and/or "git commit -a")

2. $ git add f1.txt (내용 추가 )
warning: LF will be replaced by CRLF in f1.txt.
The file will have its original line endings in your working directory

3. $ git status (추가 잘 되었나 확인 )
Changes to be committed: modified:   f1.txt

4. $ git commit ( 커밋 실행 (커밋을 해줘야 add가 확실히 완료 된다)
[master 71b2874] 2
 1 file changed, 1 insertion(+), 1 deletion(-)

5. $ git log (그 동안의 기록 확인 )
commit 71b28749f4854a12768802500764240e86dcea5f (HEAD -> master)
Author: kyuhwan <kyuhwan1020@gmail.com>
Date:   Thu Dec 19 11:38:32 2019 +0900

    2

commit 585108cbdb8277cfd5f3fafe4ed31be0fdceedba
Author: kyuhwan <kyuhwan1020@gmail.com>
Date:   Thu Dec 19 11:32:30 2019 +0900

    1#

<저장 공간 > 
 cp f2.txt f3.txt 파일 복제 
clear : 입력부분 초기화 





