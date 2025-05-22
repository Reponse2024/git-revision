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
$ git remote add git-copyy https://github.com/Reponse2024/git-revision-NNew.git

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git add home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git commit -m "Remote Git copy"
[main b99fb09] Remote Git copy
 1 file changed, 1 insertion(+)

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git push git-copyy
Enumerating objects: 24, done.
Counting objects: 100% (24/24), done.
Delta compression using up to 2 threads
Compressing objects: 100% (22/22), done.
Writing objects: 100% (24/24), 3.28 KiB | 209.00 KiB/s, done.
Total 24 (delta 4), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (4/4), done.
To https://github.com/Reponse2024/git-revision-NNew.git
 * [new branch]      main -> main

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 407 bytes | 407.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Reponse2024/git-revision.git
   9f54105..b99fb09  main -> main

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$
```
# Bundle 4
# Exercise 2

```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git checkout -b ft/footer
Switched to a new branch 'ft/footer'

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/footer)
$ git add foot.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/footer)
$ git commit -m "Created a footer"
[ft/footer c9c6ddd] Created a footer
 1 file changed, 11 insertions(+)
 create mode 100644 foot.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/footer)
$ git add foot.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/footer)
$ git commit -m "Updated footer"
[ft/footer f6d4de1] Updated footer
 1 file changed, 4 insertions(+)
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/footer)
$ git push --set-upstream origin ft/footer
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 2 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 811 bytes | 50.00 KiB/s, done.
Total 6 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), done.
remote:
remote: Create a pull request for 'ft/footer' on GitHub by visiting:
remote:      https://github.com/Reponse2024/git-revision/pull/new/ft/footer
remote:
To https://github.com/Reponse2024/git-revision.git
 * [new branch]      ft/footer -> ft/footer
branch 'ft/footer' set up to track 'origin/ft/footer'.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/footer)
$ git checkout main
M       README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git checkout -b ft/squashing
Switched to a new branch 'ft/squashing'
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/squashing)
$ git merge --squash ft/footer
Updating 9f54105..f6d4de1
Fast-forward
Squash commit -- not updating HEAD
 foot.html | 15 +++++++++++++++
 1 file changed, 15 insertions(+)
 create mode 100644 foot.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/squashing)
$ git add .

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/squashing)
$ git commit -m "footer changes squashing"
[ft/squashing b17604d] footer changes squashing
 2 files changed, 19 insertions(+), 1 deletion(-)
 create mode 100644 foot.html
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/squashing)
$ git push --set-upstream origin ft/squashing
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 654 bytes | 327.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/squashing' on GitHub by visiting:
remote:      https://github.com/Reponse2024/git-revision/pull/new/ft/squashing
remote:
To https://github.com/Reponse2024/git-revision.git
 * [new branch]      ft/squashing -> ft/squashing
branch 'ft/squashing' set up to track 'origin/ft/squashing'.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/squashing)
$
```
# Bundle 5
## Exercise 1
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git pull
Already up to date.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git add index.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git add home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        renamed:    home.html -> index.html


User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git commit -m "Renames home.html to index.html"
[main 2b710c8] Renames home.html to index.html
 1 file changed, 0 insertions(+), 0 deletions(-)
 rename home.html => index.html (100%)

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 2 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 247 bytes | 123.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Reponse2024/git-revision.git
   f0c4783..2b710c8  main -> main

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git push git-copyy
Enumerating objects: 7, done.
Counting objects: 100% (7/7), done.
Delta compression using up to 2 threads
Compressing objects: 100% (5/5), done.
Writing objects: 100% (5/5), 763 bytes | 127.00 KiB/s, done.
Total 5 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 1 local object.
To https://github.com/Reponse2024/git-revision-NNew.git
   b99fb09..2b710c8  main -> main

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$
```
# Bundle 5
## Exercise 2
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (ft/cafe)
$ git add .

User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (ft/cafe)
$ git commit -m "Updated index.html"
[ft/cafe 188e596] Updated index.html
 1 file changed, 2 insertions(+), 1 deletion(-)

User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (ft/cafe)
$ git push --set-upstream origin ft/cafe
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 348 bytes | 174.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/cafe' on GitHub by visiting:
remote:      https://github.com/Reponse2024/git-cafe-exercise/pull/new/ft/cafe
remote:
To https://github.com/Reponse2024/git-cafe-exercise.git
 * [new branch]      ft/cafe -> ft/cafe
branch 'ft/cafe' set up to track 'origin/ft/cafe'.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (ft/cafe)
$
```

# Bundle 6
## Exercise 1
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (ft/bundle6-exercise2)
$ git add menu.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (ft/bundle6-exercise2)
$ git commit -m "Added a menu page"
[ft/bundle6-exercise2 ea02c81] Added a menu page
 1 file changed, 18 insertions(+)
 create mode 100644 menu.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (ft/bundle6-exercise2)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 493 bytes | 493.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Reponse2024/git-cafe-exercise.git
   03ef998..ea02c81  ft/bundle6-exercise2 -> ft/bundle6-exercise2

User@sDESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (ft/bundle6-exercise2)
$
```

# Bundle 6
## Exercise 2
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (main)
$ git checkout -b bugfix/fix-contact
Switched to a new branch 'bugfix/fix-contact'

User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (bugfix/fix-contact)
$ git add index-4.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (bugfix/fix-contact)
$ git commit -m "Updated web title"
[bugfix/fix-contact 588f414] Updated web title
 1 file changed, 1 insertion(+), 1 deletion(-)

User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (bugfix/fix-contact)
$ git push --set-upstream origin bugfix/fix-contact
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 304 bytes | 10.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
remote:
remote: Create a pull request for 'bugfix/fix-contact' on GitHub by visiting:
remote:      https://github.com/Reponse2024/git-cafe-exercise/pull/new/bugfix/fix-contact
remote:
To https://github.com/Reponse2024/git-cafe-exercise.git
 * [new branch]      bugfix/fix-contact -> bugfix/fix-contact
branch 'bugfix/fix-contact' set up to track 'origin/bugfix/fix-contact'.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-cafe-exercise (bugfix/fix-contact)
$
```
