Лог консоли второй лекции:

user@compt01 MINGW64 /c/Git_test/test_rep_two (master)
$ git init
Reinitialized existing Git repository in C:/Git_test/test_rep_two/.git/

user@compt01 MINGW64 /c/Git_test/test_rep_two (master)
$ git branch -m master main

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ git add readme.txt

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ git commit -m "add readme.txt"
[main (root-commit) 6fe6143] add readme.txt
 1 file changed, 1 insertion(+)
 create mode 100644 readme.txt

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ git log
commit 6fe61434df2fc5344feda7ea02433dfdaa11f7e8 (HEAD -> main)
Author: npol009-star <npol009@gmail.com>
Date:   Wed Oct 22 14:28:25 2025 +0700

    add readme.txt

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ git log --oneline
6fe6143 (HEAD -> main) add readme.txt

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ git remote add origin https://github.com/npol009-star/test2.git

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Writing objects: 100% (3/3), 216 bytes | 108.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/npol009-star/test2.git
 * [new branch]      main -> main




user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ git add readme2.txt

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ git commit -m "add radme2.txt"
[main 8b88d09] add radme2.txt
 1 file changed, 1 insertion(+)
 create mode 100644 readme2.txt

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ get log --onliline
bash: get: command not found

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ git log --oneline
8b88d09 (HEAD -> main) add radme2.txt
6fe6143 (origin/main) add readme.txt

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ ^C

user@compt01 MINGW64 /c/Git_test/test_rep_two (main)
$ git checkout -b old_state 6fe6143
Switched to a new branch 'old_state'

user@compt01 MINGW64 /c/Git_test/test_rep_two (old_state)
$ git push origin old_state

user@compt01 MINGW64 /c/git_test/test_rep_two (old_state)
$ git switch main
Switched to branch 'main'

user@compt01 MINGW64 /c/git_test/test_rep_two (main)
$ git push origin main
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 239 bytes | 239.00 KiB/s, done.
Total 2 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/npol009-star/test2.git
   6fe6143..8b88d09  main -> main







