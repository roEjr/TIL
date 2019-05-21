# Git

> Git은 소스코드 형상(버전)관리 도구이다.

## 기본명령어

1. 저장소( repository) 만들기

   

   ```bash
   $git init
   // Initialized empty Git repository in C:/Users/user/Desktop/TIL/.git/
   ```

   

   내가 원하는 폴더를 git으로 저장소로 초기화 한다 (` master` )라는 표기를 통해 해다폴더가 git repository 라는것을 확인할 수 있다. ( 더 정확하게는 해당 폴더에 숨김폴더로 .git이 있다.)

   

   

2. `git add`  - 커밋할 목록에추가하기

   ```bash
   git add .
   
   On branch master
   
   No commits yet
   
   Changes to be committed:
     (use "git rm --cached <file>..." to unstage)
   
           new file:   Git.md
   
   ```

   `git add .` 에서 `.` 은 디렉터리를 뜻하는 리눅스표기법. 현재 디렉터리의 변겨사항들을 모두 커밋할 목록에 담아둔다는 뜻이다.

   `git add git.md` 라고 하면, 특정 파일만 올릴 수도 있고, `git add myfloder` 라고하면 특정 폴도를 모두담아둘 수도있다.

   

   

3. 커밋

   ```` bash
   git commit -m '커밋메세지'
   ````

   커밋은 버전의 이력을 남기는것이다. 커밋할 목록에 있는 내용들을 버전에 포함시킨다.(untracke / 목록에 없는것은 포함 안됨.)

4. 커밋 이력 확인 하기

   ```bash
   user@pc9 MINGW64 ~/Desktop/TIL (master)
   $ git log
   commit 5d9765b6905accbf8abecf8d76598699d964d4b8 (HEAD -> master)
   Author: roEjr <fine424@naver.com>
   Date:   Tue May 21 12:38:58 2019 +0900
   
       Git 기초 명령어 정리
   
   ```

   

5. **git 상태 확인하기**

   ```bash
   $ git status
   ```

   CLI(Command Line Interface)에서는 현재 상태를 확인하기 위해서 지속적으로 확인해야 한다.