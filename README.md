# Bundle 3
## Exercise 2
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/home-page-redesign)
$ git rebase origin main
Current branch main is up to date.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git add home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git commit -m "Changed home page"
[main 011538f] Changed home page
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 367 bytes | 367.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Reponse2024/git-revision.git
   c60dff1..011538f  main -> main

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$
```
# Bundle 4
## Exercise 1
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git remote add git-copy https://github.com/Reponse2024/git-revision-new.git

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git add home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git commit -m "Added conversation to home page"
[main d92e86c] Added conversation to home page
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git push git-copy
Enumerating objects: 18, done.
Counting objects: 100% (18/18), done.
Delta compression using up to 2 threads
Compressing objects: 100% (16/16), done.
Writing objects: 100% (18/18), 2.52 KiB | 53.00 KiB/s, done.
Total 18 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), done.
To https://github.com/Reponse2024/git-revision-new.git
 * [new branch]      main -> main

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$
```
# Bundle 4
# Exercise 2

