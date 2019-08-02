Paulo Godoy@LAPTOP-00017 MINGW64 /c/Projetos
$ cd ..

Paulo Godoy@LAPTOP-00017 MINGW64 /c
$ cd pro
Program Files/       ProgramData/         Projetos/
Program Files (x86)/ proj/

Paulo Godoy@LAPTOP-00017 MINGW64 /c
$ git config --global user.name "Paulo Godoy"

Paulo Godoy@LAPTOP-00017 MINGW64 /c/proj
$ git config --global user.email "teste@teste.com"

Paulo Godoy@LAPTOP-00017 MINGW64 /c/proj
$ git config --global core.editor code

Paulo Godoy@LAPTOP-00017 MINGW64 /c/proj
$ git config user.name
Paulo Godoy

Paulo Godoy@LAPTOP-00017 MINGW64 /c/proj
$ git config user.email
teste@teste.com

Paulo Godoy@LAPTOP-00017 MINGW64 /c/proj
$ git config core.editor
code

Paulo Godoy@LAPTOP-00017 MINGW64 /c/proj
$ git config --list
core.symlinks=false
core.autocrlf=true
core.fscache=true
color.diff=auto
color.status=auto
color.branch=auto
color.interactive=true
help.format=html
rebase.autosquash=true
http.sslcainfo=C:/Program Files/Git/mingw64/ssl/certs/ca-bundle.crt
http.sslbackend=openssl
diff.astextplain.textconv=astextplain
filter.lfs.clean=git-lfs clean -- %f
filter.lfs.smudge=git-lfs smudge -- %f
filter.lfs.process=git-lfs filter-process
filter.lfs.required=true
credential.helper=manager
user.email=teste@teste.com
user.name=Paulo Godoy
core.editor=code

Paulo Godoy@LAPTOP-00017 MINGW64 /c/proj
$ cd c:]
bash: cd: c:]: No such file or directory

Paulo Godoy@LAPTOP-00017 MINGW64 /c/proj
$ cd \
>

Paulo Godoy@LAPTOP-00017 MINGW64 ~
$

Paulo Godoy@LAPTOP-00017 MINGW64 ~
$ cd c:

Paulo Godoy@LAPTOP-00017 MINGW64 /c
$ mkdir project

Paulo Godoy@LAPTOP-00017 MINGW64 /c
$ cd pro
Program Files/       ProgramData/         project/
Program Files (x86)/ proj/                Projetos/

Paulo Godoy@LAPTOP-00017 MINGW64 /c
$ cd proj
proj/     project/  Projetos/

Paulo Godoy@LAPTOP-00017 MINGW64 /c
$ cd project/

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project
$ ls

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project
$ git init
Initialized empty Git repository in C:/project/.git/

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ ls -la
total 16
drwxr-xr-x 1 Paulo Godoy 197121 0 ago  2 11:51 ./
drwxr-xr-x 1 Paulo Godoy 197121 0 ago  2 11:37 ../
drwxr-xr-x 1 Paulo Godoy 197121 0 ago  2 11:51 .git/

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ cd git
bash: cd: git: No such file or directory

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ cd .git

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project/.git (GIT_DIR!)
$ ls
config  description  HEAD  hooks/  info/  objects/  refs/

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project/.git (GIT_DIR!)
$ cd ..

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ vim Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ ls
Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        Readme.md

nothing added to commit but untracked files present (use "git add" to track)

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git add *
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   Readme.md


Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ vim Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   Readme.md

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   Readme.md


Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git add *
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)

        new file:   Readme.md


Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git commit -m "teste"
[master (root-commit) 9af5b84] teste
 1 file changed, 2 insertions(+)
 create mode 100644 Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git log
commit 9af5b848c059d189f512166f6775ae2eb4d7ce64 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git log --decorate
commit 9af5b848c059d189f512166f6775ae2eb4d7ce64 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git log --author "paulo"
commit 9af5b848c059d189f512166f6775ae2eb4d7ce64 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git shortlog
Paulo Godoy (1):
      teste


Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git shortlog -sn
     1  Paulo Godoy

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git log --graph
* commit 9af5b848c059d189f512166f6775ae2eb4d7ce64 (HEAD -> master)
  Author: Paulo Godoy <teste@teste.com>
  Date:   Fri Aug 2 12:07:04 2019 -0300

      teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git show  9af5b848c059d189f512166f6775ae2eb4d7ce64
commit 9af5b848c059d189f512166f6775ae2eb4d7ce64 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

diff --git a/Readme.md b/Readme.md
new file mode 100644
index 0000000..c8dcccb
--- /dev/null
+++ b/Readme.md
@@ -0,0 +1,2 @@
+#GitHub
+#teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git status
On branch master
nothing to commit, working tree clean

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ vim Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git diff
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory
diff --git a/Readme.md b/Readme.md
index c8dcccb..3e98812 100644
--- a/Readme.md
+++ b/Readme.md
@@ -1,2 +1,4 @@
 #GitHub
 #teste
+
+#jhdflsjkhlsahldkhsakl

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git diff --name-only
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory
Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git commit -am "edicao"
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory
[master 591e6c4] edicao
 1 file changed, 2 insertions(+)

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git diff

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git show  9af5b848c059d189f512166f6775ae2eb4d7ce64
commit 9af5b848c059d189f512166f6775ae2eb4d7ce64
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

diff --git a/Readme.md b/Readme.md
new file mode 100644
index 0000000..c8dcccb
--- /dev/null
+++ b/Readme.md
@@ -0,0 +1,2 @@
+#GitHub
+#teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git log
commit 591e6c4a9d6f648b0228f24da5a6d4a431d61ea2 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:23:53 2019 -0300

    edicao

commit 9af5b848c059d189f512166f6775ae2eb4d7ce64
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git show
commit 591e6c4a9d6f648b0228f24da5a6d4a431d61ea2 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:23:53 2019 -0300

    edicao

diff --git a/Readme.md b/Readme.md
index c8dcccb..3e98812 100644
--- a/Readme.md
+++ b/Readme.md
@@ -1,2 +1,4 @@
 #GitHub
 #teste
+
+#jhdflsjkhlsahldkhsakl

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git status
On branch master
nothing to commit, working tree clean

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ vim Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git diff
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory
diff --git a/Readme.md b/Readme.md
index 3e98812..5492083 100644
--- a/Readme.md
+++ b/Readme.md
@@ -2,3 +2,5 @@
 #teste

 #jhdflsjkhlsahldkhsakl
+
+shjhdsjadhjs

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git diff --name-only
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory
Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git comit -am "teste2"
git: 'comit' is not a git command. See 'git --help'.

The most similar command is
        commit

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git log
commit 591e6c4a9d6f648b0228f24da5a6d4a431d61ea2 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:23:53 2019 -0300

    edicao

commit 9af5b848c059d189f512166f6775ae2eb4d7ce64
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ vim Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git status
On branch master
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   Readme.md

no changes added to commit (use "git add" and/or "git commit -a")

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git diff
warning: LF will be replaced by CRLF in Readme.md.
The file will have its original line endings in your working directory
diff --git a/Readme.md b/Readme.md
index 3e98812..7cf7c4a 100644
--- a/Readme.md
+++ b/Readme.md
@@ -2,3 +2,9 @@
 #teste

 #jhdflsjkhlsahldkhsakl
+
+shjhdsjadhjs
+
+paulo
+murilo
+fabrine

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git checkout Readme.md
Updated 1 path from the index

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git log
commit 591e6c4a9d6f648b0228f24da5a6d4a431d61ea2 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:23:53 2019 -0300

    edicao

commit 9af5b848c059d189f512166f6775ae2eb4d7ce64
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git diff

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ vim Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git add *

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git status
On branch master
Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   Readme.md


Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git diff

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git reset HEAD Readme.md
Unstaged changes after reset:
M       Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git diff
diff --git a/Readme.md b/Readme.md
index 3e98812..8ea6a34 100644
--- a/Readme.md
+++ b/Readme.md
@@ -2,3 +2,7 @@
 #teste

 #jhdflsjkhlsahldkhsakl
+
+jksdhkjahdjkhsajkd
+dkjsalkdjsakljd
+klsajdklsajdkl

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git checkout Readme.md
Updated 1 path from the index

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git status
On branch master
nothing to commit, working tree clean

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ vim Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git commit -am "dskdksdksmdkms"
[master 7210c88] dskdksdksmdkms
 1 file changed, 1 insertion(+)

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git log
commit 7210c884aad3289b57289e53b7c3a9cb0b537c41 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 14:33:20 2019 -0300

    dskdksdksmdkms

commit 591e6c4a9d6f648b0228f24da5a6d4a431d61ea2
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:23:53 2019 -0300

    edicao

commit 9af5b848c059d189f512166f6775ae2eb4d7ce64
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git reset --soft  7210c884aad3289b57289e53b7c3a9cb0b537c41

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git log
commit 7210c884aad3289b57289e53b7c3a9cb0b537c41 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 14:33:20 2019 -0300

    dskdksdksmdkms

commit 591e6c4a9d6f648b0228f24da5a6d4a431d61ea2
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:23:53 2019 -0300

    edicao

commit 9af5b848c059d189f512166f6775ae2eb4d7ce64
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git reset --soft   591e6c4a9d6f648b0228f24da5a6d4a431d61ea2

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git log
commit 591e6c4a9d6f648b0228f24da5a6d4a431d61ea2 (HEAD -> master)
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:23:53 2019 -0300

    edicao

commit 9af5b848c059d189f512166f6775ae2eb4d7ce64
Author: Paulo Godoy <teste@teste.com>
Date:   Fri Aug 2 12:07:04 2019 -0300

    teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ cd ~.ssh
bash: cd: ~.ssh: No such file or directory

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ cd ~/.ssh

Paulo Godoy@LAPTOP-00017 MINGW64 ~/.ssh
$ ls
id_rsa  id_rsa.pub  known_hosts

Paulo Godoy@LAPTOP-00017 MINGW64 ~/.ssh
$ vim id_rsa

Paulo Godoy@LAPTOP-00017 MINGW64 ~/.ssh
$ cat id_rsa.pub


Paulo Godoy@LAPTOP-00017 MINGW64 ~/.ssh
$ git remote add origin teste@git/teste
fatal: not a git repository (or any of the parent directories): .git

Paulo Godoy@LAPTOP-00017 MINGW64 ~/.ssh
$ cd c:

Paulo Godoy@LAPTOP-00017 MINGW64 /c
$ cd project/

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ ls
Readme.md

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git remote add origin teste@git/teste

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git remote
origin

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git remote -v
origin  teste@git/teste (fetch)
origin  teste@git/teste (push)

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$ git push -u origin master
Warning: Permanently added the RSA host key for IP address '192.30.253.113' to the list of known hosts.
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (6/6), 490 bytes | 21.00 KiB/s, done.
Total 6 (delta 0), reused 0 (delta 0)
To github.com:paulo-godoy/curso-git.git
 * [new branch]      master -> master
Branch 'master' set up to track remote branch 'master' from 'origin'.

Paulo Godoy@LAPTOP-00017 MINGW64 /c/project (master)
$
