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