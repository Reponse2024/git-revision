# Git Revision
## Bundle 1
### Exercise 2
```bash

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git add home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: b00a45f Displayed a welcome message

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git add about.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: b00a45f Displayed a welcome message

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git add team.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git stash
Saved working directory and index state WIP on dev: b00a45f Displayed a welcome message

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git stash list
stash@{0}: WIP on dev: b00a45f Displayed a welcome message
stash@{1}: WIP on dev: b00a45f Displayed a welcome message
stash@{2}: WIP on dev: b00a45f Displayed a welcome message

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (3e956ac42ccd36c56d4120feb678837f5a22f92a)

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git stash pop stash@{1}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   home.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   index.html

Dropped stash@{1} (a3f79ff9ab3e4b8fa2b2229ad100db2f4ca6cc5a)

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git stash list
stash@{0}: WIP on dev: b00a45f Displayed a welcome message

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git commit -m "Restored the changes for two files, about.html, and home.html"
[dev 6f0c62b] Restored the changes for two files, about.html, and home.html
 2 files changed, 27 insertions(+)
 create mode 100644 about.html
 create mode 100644 home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 2 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 761 bytes | 108.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Reponse2024/git-revision.git
   b00a45f..6f0c62b  dev -> dev

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   team.html

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md
        modified:   index.html

Dropped stash@{0} (b033d3891cc961e5e674646c6a93efd6e8311156)

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git stash list

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$ git reset --hard
HEAD is now at 6f0c62b Restored the changes for two files, about.html, and home.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (dev)
$
```
