
yaoa@RYDWS366 MINGW64 ~
$ git config --help

yaoa@RYDWS366 MINGW64 ~
$ git config -h
usage: git config [<options>]

Config file location
    --global              use global config file
    --system              use system config file
    --local               use repository config file
    -f, --file <file>     use given config file
    --blob <blob-id>      read config from given blob object

Action
    --get                 get value: name [value-regex]
    --get-all             get all values: key [value-regex]
    --get-regexp          get values for regexp: name-regex [v                                                                                                                                                                                                                 alue-regex]
    --get-urlmatch        get value specific for the URL: sect                                                                                                                                                                                                                 ion[.var] URL
    --replace-all         replace all matching variables: name                                                                                                                                                                                                                  value [value_regex]
    --add                 add a new variable: name value
    --unset               remove a variable: name [value-regex                                                                                                                                                                                                                 ]
    --unset-all           remove all matches: name [value-rege                                                                                                                                                                                                                 x]
    --rename-section      rename section: old-name new-name
    --remove-section      remove a section: name
    -l, --list            list all
    -e, --edit            open an editor
    --get-color           find the color configured: slot [def                                                                                                                                                                                                                 ault]
    --get-colorbool       find the color setting: slot [stdout                                                                                                                                                                                                                 -is-tty]

Type
    -t, --type <>         value is given this type
    --bool                value is "true" or "false"
    --int                 value is decimal number
    --bool-or-int         value is --bool or --int
    --path                value is a path (file or directory n                                                                                                                                                                                                                 ame)
    --expiry-date         value is an expiry date

Other
    -z, --null            terminate values with NUL byte
    --name-only           show variable names only
    --includes            respect include directives on lookup
    --show-origin         show origin of config (file, standar                                                                                                                                                                                                                 d input, blob, command line)
    --default <value>     with --get, use default value when m                                                                                                                                                                                                                 issing entry


yaoa@RYDWS366 MINGW64 ~
$ git config --global user.name "alanyaoy"

yaoa@RYDWS366 MINGW64 ~
$ git config --global user.email"alanyaoy555@gmail.com"

yaoa@RYDWS366 MINGW64 ~
$ pwd
/c/Users/yaoa

yaoa@RYDWS366 MINGW64 ~
$ git clone https://github.com/alanyaoy/newGITTest.git
Cloning into 'newGITTest'...
remote: Counting objects: 29, done.
remote: Compressing objects: 100% (21/21), done.
remote: Total 29 (delta 3), reused 21 (delta 1), pack-reused 0
Unpacking objects: 100% (29/29), done.

yaoa@RYDWS366 MINGW64 ~
$ ls
 1.txt                     'Application Data'@   Documents/               Links/             NetHood@          ntuser.dat.LOG2                                                                                ntuser.ini   Recent@         SendTo@        test.tx
 Alan_HD/                   Contacts/            Downloads/              'Local Settings'@   newGITTest/       NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TM.blf                                        ntuser.pol   Roaming/        source/        test.txt
'Alan_HD - Shortcut.lnk'*   Cookies@             Favorites/               Music/             NTUSER.DAT        NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000001.regtrans-ms   Pictures/   'Saved Games'/  'Start Menu'@   text.txt
 AppData/                   Desktop/             IntelGraphicsProfiles/  'My Documents'@     ntuser.dat.LOG1   NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000002.regtrans-ms   PrintHood@   Searches/       Templates@     Videos/

yaoa@RYDWS366 MINGW64 ~
$ ls -la
total 28641
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:18  ./
drwxr-xr-x 1 yaoa 1049089        0 Mar 20 12:12  ../
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:06  .atom/
-rw-r--r-- 1 yaoa 1049089       24 Aug  6 12:13  .gitconfig
-rw-r--r-- 1 yaoa 1049089    52617 Dec 11  2017  1.txt
drwxr-xr-x 1 yaoa 1049089        0 May 29 16:45  Alan_HD/
-rwxr-xr-x 1 yaoa 1049089     1102 Sep 11  2017 'Alan_HD - Shortcut.lnk'*
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  AppData/
lrwxrwxrwx 1 yaoa 1049089       29 Sep  8  2017 'Application Data' -> /c/Users/yaoa/AppData/Roaming/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Contacts/
lrwxrwxrwx 1 yaoa 1049089       57 Sep  8  2017  Cookies -> /c/Users/yaoa/AppData/Local/Microsoft/Windows/INetCookies/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:05  Desktop/
drwxr-xr-x 1 yaoa 1049089        0 May 23 14:34  Documents/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:05  Downloads/
drwxr-xr-x 1 yaoa 1049089        0 Jan 15  2018  Favorites/
drwxr-xr-x 1 yaoa 1049089        0 Jul 16 09:20  IntelGraphicsProfiles/
drwxr-xr-x 1 yaoa 1049089        0 Feb 22 15:37  Links/
lrwxrwxrwx 1 yaoa 1049089       27 Sep  8  2017 'Local Settings' -> /c/Users/yaoa/AppData/Local/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Music/
lrwxrwxrwx 1 yaoa 1049089       23 Sep  8  2017 'My Documents' -> /c/Users/yaoa/Documents/
lrwxrwxrwx 1 yaoa 1049089       65 Sep  8  2017  NetHood -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Network Shortcuts'/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:18  newGITTest/
-rw-r--r-- 1 yaoa 1049089 10485760 Jul 16 09:19  NTUSER.DAT
-rw-r--r-- 1 yaoa 1049089  8937472 Sep  8  2017  ntuser.dat.LOG1
-rw-r--r-- 1 yaoa 1049089  5681152 Sep  8  2017  ntuser.dat.LOG2
-rw-r--r-- 1 yaoa 1049089    65536 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TM.blf
-rw-r--r-- 1 yaoa 1049089   524288 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000001.regtrans-ms
-rw-r--r-- 1 yaoa 1049089   524288 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000002.regtrans-ms
-rw-r--r-- 1 yaoa 1049089       20 Sep  8  2017  ntuser.ini
-r--r--r-- 1 yaoa 1049089     2568 Aug  2 12:02  ntuser.pol
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Pictures/
lrwxrwxrwx 1 yaoa 1049089       65 Sep  8  2017  PrintHood -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Printer Shortcuts'/
lrwxrwxrwx 1 yaoa 1049089       54 Sep  8  2017  Recent -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Recent/
drwxr-xr-x 1 yaoa 1049089        0 Aug 31  2017  Roaming/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017 'Saved Games'/
drwxr-xr-x 1 yaoa 1049089        0 Mar 19 11:28  Searches/
lrwxrwxrwx 1 yaoa 1049089       54 Sep  8  2017  SendTo -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/SendTo/
drwxr-xr-x 1 yaoa 1049089        0 Sep 18  2017  source/
lrwxrwxrwx 1 yaoa 1049089       58 Sep  8  2017 'Start Menu' -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Start Menu'/
lrwxrwxrwx 1 yaoa 1049089       57 Sep  8  2017  Templates -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Templates/
-rw-r--r-- 1 yaoa 1049089       15 Dec 11  2017  test.tx
-rw-r--r-- 1 yaoa 1049089       15 Dec 11  2017  test.txt
-rw-r--r-- 1 yaoa 1049089       65 Dec 11  2017  text.txt
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Videos/

yaoa@RYDWS366 MINGW64 ~
$ dir
1.txt                     Application\ Data  Documents              Links            NetHood          ntuser.dat.LOG2                                                                               ntuser.ini  Recent        SendTo       test.tx
Alan_HD                   Contacts           Downloads              Local\ Settings  newGITTest       NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TM.blf                                       ntuser.pol  Roaming       source       test.txt
Alan_HD\ -\ Shortcut.lnk  Cookies            Favorites              Music            NTUSER.DAT       NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000001.regtrans-ms  Pictures    Saved\ Games  Start\ Menu  text.txt
AppData                   Desktop            IntelGraphicsProfiles  My\ Documents    ntuser.dat.LOG1  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000002.regtrans-ms  PrintHood   Searches      Templates    Videos

yaoa@RYDWS366 MINGW64 ~
$ pwd
/c/Users/yaoa

yaoa@RYDWS366 MINGW64 ~
$ cd ..

yaoa@RYDWS366 MINGW64 /c/Users
$ pwd
/c/Users

yaoa@RYDWS366 MINGW64 /c/Users
$ cd ..

yaoa@RYDWS366 MINGW64 /c
$ pwd
/c

yaoa@RYDWS366 MINGW64 /c
$ cd users

yaoa@RYDWS366 MINGW64 /c/users
$ pwd
/c/users

yaoa@RYDWS366 MINGW64 /c/users
$ cd /

yaoa@RYDWS366 MINGW64 /
$ pwd
/

yaoa@RYDWS366 MINGW64 /
$ cd c

yaoa@RYDWS366 MINGW64 /c
$ pwd
/c

yaoa@RYDWS366 MINGW64 /c
$ cd users

yaoa@RYDWS366 MINGW64 /c/users
$ pwd
/c/users

yaoa@RYDWS366 MINGW64 /c/users
$ cd yaoa

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ pwd
/c/users/yaoa

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ ls -la
total 28641
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:18  ./
drwxr-xr-x 1 yaoa 1049089        0 Mar 20 12:12  ../
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:06  .atom/
-rw-r--r-- 1 yaoa 1049089       24 Aug  6 12:13  .gitconfig
-rw-r--r-- 1 yaoa 1049089    52617 Dec 11  2017  1.txt
drwxr-xr-x 1 yaoa 1049089        0 May 29 16:45  Alan_HD/
-rwxr-xr-x 1 yaoa 1049089     1102 Sep 11  2017 'Alan_HD - Shortcut.lnk'*
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  AppData/
lrwxrwxrwx 1 yaoa 1049089       29 Sep  8  2017 'Application Data' -> /c/Users/yaoa/AppData/Roaming/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Contacts/
lrwxrwxrwx 1 yaoa 1049089       57 Sep  8  2017  Cookies -> /c/Users/yaoa/AppData/Local/Microsoft/Windows/INetCookies/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:05  Desktop/
drwxr-xr-x 1 yaoa 1049089        0 May 23 14:34  Documents/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:05  Downloads/
drwxr-xr-x 1 yaoa 1049089        0 Jan 15  2018  Favorites/
drwxr-xr-x 1 yaoa 1049089        0 Jul 16 09:20  IntelGraphicsProfiles/
drwxr-xr-x 1 yaoa 1049089        0 Feb 22 15:37  Links/
lrwxrwxrwx 1 yaoa 1049089       27 Sep  8  2017 'Local Settings' -> /c/Users/yaoa/AppData/Local/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Music/
lrwxrwxrwx 1 yaoa 1049089       23 Sep  8  2017 'My Documents' -> /c/Users/yaoa/Documents/
lrwxrwxrwx 1 yaoa 1049089       65 Sep  8  2017  NetHood -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Network Shortcuts'/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:18  newGITTest/
-rw-r--r-- 1 yaoa 1049089 10485760 Jul 16 09:19  NTUSER.DAT
-rw-r--r-- 1 yaoa 1049089  8937472 Sep  8  2017  ntuser.dat.LOG1
-rw-r--r-- 1 yaoa 1049089  5681152 Sep  8  2017  ntuser.dat.LOG2
-rw-r--r-- 1 yaoa 1049089    65536 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TM.blf
-rw-r--r-- 1 yaoa 1049089   524288 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000001.regtrans-ms
-rw-r--r-- 1 yaoa 1049089   524288 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000002.regtrans-ms
-rw-r--r-- 1 yaoa 1049089       20 Sep  8  2017  ntuser.ini
-r--r--r-- 1 yaoa 1049089     2568 Aug  2 12:02  ntuser.pol
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Pictures/
lrwxrwxrwx 1 yaoa 1049089       65 Sep  8  2017  PrintHood -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Printer Shortcuts'/
lrwxrwxrwx 1 yaoa 1049089       54 Sep  8  2017  Recent -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Recent/
drwxr-xr-x 1 yaoa 1049089        0 Aug 31  2017  Roaming/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017 'Saved Games'/
drwxr-xr-x 1 yaoa 1049089        0 Mar 19 11:28  Searches/
lrwxrwxrwx 1 yaoa 1049089       54 Sep  8  2017  SendTo -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/SendTo/
drwxr-xr-x 1 yaoa 1049089        0 Sep 18  2017  source/
lrwxrwxrwx 1 yaoa 1049089       58 Sep  8  2017 'Start Menu' -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Start Menu'/
lrwxrwxrwx 1 yaoa 1049089       57 Sep  8  2017  Templates -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Templates/
-rw-r--r-- 1 yaoa 1049089       15 Dec 11  2017  test.tx
-rw-r--r-- 1 yaoa 1049089       15 Dec 11  2017  test.txt
-rw-r--r-- 1 yaoa 1049089       65 Dec 11  2017  text.txt
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Videos/

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ ls
 1.txt                     'Application Data'@   Documents/               Links/             NetHood@          ntuser.dat.LOG2                                                                                ntuser.ini   Recent@         SendTo@        test.tx
 Alan_HD/                   Contacts/            Downloads/              'Local Settings'@   newGITTest/       NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TM.blf                                        ntuser.pol   Roaming/        source/        test.txt
'Alan_HD - Shortcut.lnk'*   Cookies@             Favorites/               Music/             NTUSER.DAT        NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000001.regtrans-ms   Pictures/   'Saved Games'/  'Start Menu'@   text.txt
 AppData/                   Desktop/             IntelGraphicsProfiles/  'My Documents'@     ntuser.dat.LOG1   NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000002.regtrans-ms   PrintHood@   Searches/       Templates@     Videos/

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ git --version
git version 2.18.0.windows.1

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ cd newGitTest

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ touch myhdfile.txt

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ echo " I am sam and I like ham." >> myhdfile.txt

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Untracked files:
  (use "git add <file>..." to include in what will be committed)

        myhdfile.txt

nothing added to commit but untracked files present (use "git add" to track)

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git add .
warning: LF will be replaced by CRLF in myhdfile.txt.
The file will have its original line endings in your working directory.

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git diff

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        new file:   myhdfile.txt


yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git commit -m "add hd.txt test file"
[master 0891208] add hd.txt test file
 Committer: alanyaoy <yaoa@hunterdouglas.com.au>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly:

    git config --global user.name "Your Name"
    git config --global user.email you@example.com

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)
 create mode 100644 myhdfile.txt

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git status
On branch master
Your branch is ahead of 'origin/master' by 1 commit.
  (use "git push" to publish your local commits)

nothing to commit, working tree clean

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads.
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 307 bytes | 307.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/alanyaoy/newGITTest.git
   79515e8..0891208  master -> master

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ echo " This is my first hd Git file." >> myhdfile.txt

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   myhdfile.txt

no changes added to commit (use "git add" and/or "git commit -a")

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git checkout -- <file>..." to discard changes in working directory)

        modified:   myhdfile.txt

no changes added to commit (use "git add" and/or "git commit -a")

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git diff
warning: LF will be replaced by CRLF in myhdfile.txt.
The file will have its original line endings in your working directory.
diff --git a/myhdfile.txt b/myhdfile.txt
index af7088b..4da760b 100644
--- a/myhdfile.txt
+++ b/myhdfile.txt
@@ -1 +1,2 @@
  I am sam and I like ham.
+ This is my first hd Git file.

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git add myhdfile.txt
warning: LF will be replaced by CRLF in myhdfile.txt.
The file will have its original line endings in your working directory.

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git status
On branch master
Your branch is up to date with 'origin/master'.

Changes to be committed:
  (use "git reset HEAD <file>..." to unstage)

        modified:   myhdfile.txt


yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git diff

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git diff --staged
diff --git a/myhdfile.txt b/myhdfile.txt
index af7088b..4da760b 100644
--- a/myhdfile.txt
+++ b/myhdfile.txt
@@ -1 +1,2 @@
  I am sam and I like ham.
+ This is my first hd Git file.

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git commit -m "add 2nd line to myhdfile.txt"
[master 3b6ea50] add 2nd line to myhdfile.txt
 Committer: alanyaoy <yaoa@hunterdouglas.com.au>
Your name and email address were configured automatically based
on your username and hostname. Please check that they are accurate.
You can suppress this message by setting them explicitly:

    git config --global user.name "Your Name"
    git config --global user.email you@example.com

After doing this, you may fix the identity used for this commit with:

    git commit --amend --reset-author

 1 file changed, 1 insertion(+)

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 4 threads.
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 319 bytes | 319.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/alanyaoy/newGITTest.git
   0891208..3b6ea50  master -> master

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ ls
code.txt  desktop.ini  myfile.txt  myhdfile.txt  NotepadGit1.txt  README.md

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ ls -la
total 93
drwxr-xr-x 1 yaoa 1049089     0 Aug  6 12:24 ./
drwxr-xr-x 1 yaoa 1049089     0 Aug  6 12:18 ../
drwxr-xr-x 1 yaoa 1049089     0 Aug  6 12:33 .git/
-rw-r--r-- 1 yaoa 1049089 71399 Aug  6 12:18 code.txt
-rw-r--r-- 1 yaoa 1049089    46 Aug  6 12:18 desktop.ini
-rw-r--r-- 1 yaoa 1049089    58 Aug  6 12:18 myfile.txt
-rw-r--r-- 1 yaoa 1049089    57 Aug  6 12:31 myhdfile.txt
-rw-r--r-- 1 yaoa 1049089   238 Aug  6 12:18 NotepadGit1.txt
-rw-r--r-- 1 yaoa 1049089    71 Aug  6 12:18 README.md

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newGitTest (master)
$ cd ..

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ ls
 1.txt                     'Application Data'@   Documents/               Links/             NetHood@          ntuser.dat.LOG2                                                                                ntuser.ini   Recent@         SendTo@        test.tx
 Alan_HD/                   Contacts/            Downloads/              'Local Settings'@   newGITTest/       NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TM.blf                                        ntuser.pol   Roaming/        source/        test.txt
'Alan_HD - Shortcut.lnk'*   Cookies@             Favorites/               Music/             NTUSER.DAT        NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000001.regtrans-ms   Pictures/   'Saved Games'/  'Start Menu'@   text.txt
 AppData/                   Desktop/             IntelGraphicsProfiles/  'My Documents'@     ntuser.dat.LOG1   NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000002.regtrans-ms   PrintHood@   Searches/       Templates@     Videos/

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ ls -la
total 28641
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:18  ./
drwxr-xr-x 1 yaoa 1049089        0 Mar 20 12:12  ../
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:06  .atom/
-rw-r--r-- 1 yaoa 1049089       24 Aug  6 12:13  .gitconfig
-rw-r--r-- 1 yaoa 1049089    52617 Dec 11  2017  1.txt
drwxr-xr-x 1 yaoa 1049089        0 May 29 16:45  Alan_HD/
-rwxr-xr-x 1 yaoa 1049089     1102 Sep 11  2017 'Alan_HD - Shortcut.lnk'*
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  AppData/
lrwxrwxrwx 1 yaoa 1049089       29 Sep  8  2017 'Application Data' -> /c/Users/yaoa/AppData/Roaming/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Contacts/
lrwxrwxrwx 1 yaoa 1049089       57 Sep  8  2017  Cookies -> /c/Users/yaoa/AppData/Local/Microsoft/Windows/INetCookies/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:05  Desktop/
drwxr-xr-x 1 yaoa 1049089        0 May 23 14:34  Documents/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:05  Downloads/
drwxr-xr-x 1 yaoa 1049089        0 Jan 15  2018  Favorites/
drwxr-xr-x 1 yaoa 1049089        0 Jul 16 09:20  IntelGraphicsProfiles/
drwxr-xr-x 1 yaoa 1049089        0 Feb 22 15:37  Links/
lrwxrwxrwx 1 yaoa 1049089       27 Sep  8  2017 'Local Settings' -> /c/Users/yaoa/AppData/Local/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Music/
lrwxrwxrwx 1 yaoa 1049089       23 Sep  8  2017 'My Documents' -> /c/Users/yaoa/Documents/
lrwxrwxrwx 1 yaoa 1049089       65 Sep  8  2017  NetHood -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Network Shortcuts'/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:24  newGITTest/
-rw-r--r-- 1 yaoa 1049089 10485760 Jul 16 09:19  NTUSER.DAT
-rw-r--r-- 1 yaoa 1049089  8937472 Sep  8  2017  ntuser.dat.LOG1
-rw-r--r-- 1 yaoa 1049089  5681152 Sep  8  2017  ntuser.dat.LOG2
-rw-r--r-- 1 yaoa 1049089    65536 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TM.blf
-rw-r--r-- 1 yaoa 1049089   524288 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000001.regtrans-ms
-rw-r--r-- 1 yaoa 1049089   524288 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000002.regtrans-ms
-rw-r--r-- 1 yaoa 1049089       20 Sep  8  2017  ntuser.ini
-r--r--r-- 1 yaoa 1049089     2568 Aug  2 12:02  ntuser.pol
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Pictures/
lrwxrwxrwx 1 yaoa 1049089       65 Sep  8  2017  PrintHood -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Printer Shortcuts'/
lrwxrwxrwx 1 yaoa 1049089       54 Sep  8  2017  Recent -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Recent/
drwxr-xr-x 1 yaoa 1049089        0 Aug 31  2017  Roaming/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017 'Saved Games'/
drwxr-xr-x 1 yaoa 1049089        0 Mar 19 11:28  Searches/
lrwxrwxrwx 1 yaoa 1049089       54 Sep  8  2017  SendTo -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/SendTo/
drwxr-xr-x 1 yaoa 1049089        0 Sep 18  2017  source/
lrwxrwxrwx 1 yaoa 1049089       58 Sep  8  2017 'Start Menu' -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Start Menu'/
lrwxrwxrwx 1 yaoa 1049089       57 Sep  8  2017  Templates -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Templates/
-rw-r--r-- 1 yaoa 1049089       15 Dec 11  2017  test.tx
-rw-r--r-- 1 yaoa 1049089       15 Dec 11  2017  test.txt
-rw-r--r-- 1 yaoa 1049089       65 Dec 11  2017  text.txt
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Videos/

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ doskey /history
Invalid macro definition.

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ doskey /HISTORY
Invalid macro definition.

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ git reflog
fatal: not a git repository (or any of the parent directories): .git

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ git log
fatal: not a git repository (or any of the parent directories): .git

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ cd newgittest

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newgittest (master)
$ doskey /hitory
Invalid macro definition.

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newgittest (master)
$ doskey /history
Invalid macro definition.

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newgittest (master)
$ git reflog
3b6ea50 (HEAD -> master, origin/master, origin/HEAD) HEAD@{0}: commit: add 2nd line to myhdfile.txt
0891208 HEAD@{1}: commit: add hd.txt test file
79515e8 HEAD@{2}: clone: from https://github.com/alanyaoy/newGITTest.git

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newgittest (master)
$ git status -s

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newgittest (master)
$ hitory
bash: hitory: command not found

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newgittest (master)
$ history
    1  git config --help
    2  git config -h
    3  git config --global user.name "alanyaoy"
    4  git config --global user.email"alanyaoy555@gmail.com"
    5  pwd
    6  git clone https://github.com/alanyaoy/newGITTest.git
    7  ls
    8  ls -la
    9  dir
   10  pwd
   11  cd ..
   12  pwd
   13  cd ..
   14  pwd
   15  cd users
   16  pwd
   17  cd /
   18  pwd
   19  cd c
   20  pwd
   21  cd users
   22  pwd
   23  cd yaoa
   24  pwd
   25  ls -la
   26  ls
   27  git --version
   28  cd newGitTest
   29  touch myhdfile.txt
   30  echo " I am sam and I like ham." >> myhdfile.txt
   31  git status
   32  git add .
   33  git diff
   34  git status
   35  git commit -m "add hd.txt test file"
   36  git status
   37  git push
   38  echo " This is my first hd Git file." >> myhdfile.txt
   39  git status
   40  git status
   41  git diff
   42  git add myhdfile.txt
   43  git status
   44  git diff
   45  git diff --staged
   46  git commit -m "add 2nd line to myhdfile.txt"
   47  git push
   48  ls
   49  ls -la
   50  cd ..
   51  ls
   52  ls -la
   53  doskey /history
   54  doskey /HISTORY
   55  git reflog
   56  git log
   57  cd newgittest
   58  doskey /hitory
   59  doskey /history
   60  git reflog
   61  git status -s
   62  hitory
   63  history

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newgittest (master)
$ ls -la
total 93
drwxr-xr-x 1 yaoa 1049089     0 Aug  6 12:24 ./
drwxr-xr-x 1 yaoa 1049089     0 Aug  6 14:07 ../
drwxr-xr-x 1 yaoa 1049089     0 Aug  6 13:40 .git/
-rw-r--r-- 1 yaoa 1049089 71399 Aug  6 12:18 code.txt
-rw-r--r-- 1 yaoa 1049089    46 Aug  6 12:18 desktop.ini
-rw-r--r-- 1 yaoa 1049089    58 Aug  6 12:18 myfile.txt
-rw-r--r-- 1 yaoa 1049089    57 Aug  6 12:31 myhdfile.txt
-rw-r--r-- 1 yaoa 1049089   238 Aug  6 12:18 NotepadGit1.txt
-rw-r--r-- 1 yaoa 1049089    71 Aug  6 12:18 README.md

yaoa@RYDWS366 MINGW64 /c/users/yaoa/newgittest (master)
$ cd ..

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ ls -la
total 28645
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 14:07  ./
drwxr-xr-x 1 yaoa 1049089        0 Mar 20 12:12  ../
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:06  .atom/
-rw-r--r-- 1 yaoa 1049089       24 Aug  6 12:13  .gitconfig
-rw-r--r-- 1 yaoa 1049089    52617 Dec 11  2017  1.txt
drwxr-xr-x 1 yaoa 1049089        0 May 29 16:45  Alan_HD/
-rwxr-xr-x 1 yaoa 1049089     1102 Sep 11  2017 'Alan_HD - Shortcut.lnk'*
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  AppData/
lrwxrwxrwx 1 yaoa 1049089       29 Sep  8  2017 'Application Data' -> /c/Users/yaoa/AppData/Roaming/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Contacts/
lrwxrwxrwx 1 yaoa 1049089       57 Sep  8  2017  Cookies -> /c/Users/yaoa/AppData/Local/Microsoft/Windows/INetCookies/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:05  Desktop/
drwxr-xr-x 1 yaoa 1049089        0 May 23 14:34  Documents/
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:05  Downloads/
drwxr-xr-x 1 yaoa 1049089        0 Jan 15  2018  Favorites/
drwxr-xr-x 1 yaoa 1049089        0 Jul 16 09:20  IntelGraphicsProfiles/
drwxr-xr-x 1 yaoa 1049089        0 Feb 22 15:37  Links/
lrwxrwxrwx 1 yaoa 1049089       27 Sep  8  2017 'Local Settings' -> /c/Users/yaoa/AppData/Local/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Music/
lrwxrwxrwx 1 yaoa 1049089       23 Sep  8  2017 'My Documents' -> /c/Users/yaoa/Documents/
lrwxrwxrwx 1 yaoa 1049089       65 Sep  8  2017  NetHood -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Network Shortcuts'/
-rw-r--r-- 1 yaoa 1049089     3288 Aug  6 14:07  network_info.txt
drwxr-xr-x 1 yaoa 1049089        0 Aug  6 12:24  newGITTest/
-rw-r--r-- 1 yaoa 1049089 10485760 Jul 16 09:19  NTUSER.DAT
-rw-r--r-- 1 yaoa 1049089  8937472 Sep  8  2017  ntuser.dat.LOG1
-rw-r--r-- 1 yaoa 1049089  5681152 Sep  8  2017  ntuser.dat.LOG2
-rw-r--r-- 1 yaoa 1049089    65536 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TM.blf
-rw-r--r-- 1 yaoa 1049089   524288 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000001.regtrans-ms
-rw-r--r-- 1 yaoa 1049089   524288 Sep  8  2017  NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000002.regtrans-ms
-rw-r--r-- 1 yaoa 1049089       20 Sep  8  2017  ntuser.ini
-r--r--r-- 1 yaoa 1049089     2568 Aug  2 12:02  ntuser.pol
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Pictures/
lrwxrwxrwx 1 yaoa 1049089       65 Sep  8  2017  PrintHood -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Printer Shortcuts'/
lrwxrwxrwx 1 yaoa 1049089       54 Sep  8  2017  Recent -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Recent/
drwxr-xr-x 1 yaoa 1049089        0 Aug 31  2017  Roaming/
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017 'Saved Games'/
drwxr-xr-x 1 yaoa 1049089        0 Mar 19 11:28  Searches/
lrwxrwxrwx 1 yaoa 1049089       54 Sep  8  2017  SendTo -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/SendTo/
drwxr-xr-x 1 yaoa 1049089        0 Sep 18  2017  source/
lrwxrwxrwx 1 yaoa 1049089       58 Sep  8  2017 'Start Menu' -> '/c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Start Menu'/
lrwxrwxrwx 1 yaoa 1049089       57 Sep  8  2017  Templates -> /c/Users/yaoa/AppData/Roaming/Microsoft/Windows/Templates/
-rw-r--r-- 1 yaoa 1049089       15 Dec 11  2017  test.tx
-rw-r--r-- 1 yaoa 1049089       15 Dec 11  2017  test.txt
-rw-r--r-- 1 yaoa 1049089       65 Dec 11  2017  text.txt
drwxr-xr-x 1 yaoa 1049089        0 Sep  8  2017  Videos/

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$ ls
 1.txt                      Contacts/    Favorites/              'My Documents'@     ntuser.dat.LOG1                                                                                ntuser.ini   Roaming/       'Start Menu'@   Videos/
 Alan_HD/                   Cookies@     IntelGraphicsProfiles/   NetHood@           ntuser.dat.LOG2                                                                                ntuser.pol  'Saved Games'/   Templates@
'Alan_HD - Shortcut.lnk'*   Desktop/     Links/                   network_info.txt   NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TM.blf                                        Pictures/    Searches/       test.tx
 AppData/                   Documents/  'Local Settings'@         newGITTest/        NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000001.regtrans-ms   PrintHood@   SendTo@         test.txt
'Application Data'@         Downloads/   Music/                   NTUSER.DAT         NTUSER.DAT{bbed3e3b-0b41-11e3-8249-d6927d06400b}.TMContainer00000000000000000002.regtrans-ms   Recent@      source/         text.txt

yaoa@RYDWS366 MINGW64 /c/users/yaoa
$



----------------------------------------------------------------------------------------------------------

Microsoft Windows [Version 6.3.9600]
(c) 2013 Microsoft Corporation. All rights reserved.

C:\Users\yaoa>help color
Sets the default console foreground and background colors.

COLOR [attr]

  attr        Specifies color attribute of console output

Color attributes are specified by TWO hex digits -- the first
corresponds to the background; the second the foreground.  Each digit
can be any of the following values:

    0 = Black       8 = Gray
    1 = Blue        9 = Light Blue
    2 = Green       A = Light Green
    3 = Aqua        B = Light Aqua
    4 = Red         C = Light Red
    5 = Purple      D = Light Purple
    6 = Yellow      E = Light Yellow
    7 = White       F = Bright White

If no argument is given, this command restores the color to what it was
when CMD.EXE started.  This value either comes from the current console
window, the /T command line switch or from the DefaultColor registry
value.

The COLOR command sets ERRORLEVEL to 1 if an attempt is made to execute
the COLOR command with a foreground and background color that are the
same.

Example: "COLOR fc" produces light red on bright white

C:\Users\yaoa>color 02

C:\Users\yaoa>color 01

C:\Users\yaoa>color 03

C:\Users\yaoa>git --version
git version 2.18.0.windows.1

C:\Users\yaoa>cd newgittest

C:\Users\yaoa\newGITTest>type myhdfile.txt
 I am sam and I like ham.

C:\Users\yaoa\newGITTest>type myhdfile.txt
 I am sam and I like ham.
 This is my first hd Git file.

C:\Users\yaoa\newGITTest>doskey /history
help color
color 02
color 01
color 03
git --version
cd newgittest
type myhdfile.txt
doskey /history

C:\Users\yaoa\newGITTest>git status
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean

C:\Users\yaoa\newGITTest>color 05

C:\Users\yaoa\newGITTest>cd ..

C:\Users\yaoa>ipconfig /all >network_info.txt

C:\Users\yaoa>mycommand.exe >file.txt
'mycommand.exe' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\yaoa>