
# Git Revision
## Bundle 1
### Exercise 1
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
 ```
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
# Git Revision
## Bundle 2
### Exercise 1
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (Bundle2-Ex2)
$ git branch -M ft/bundle-2

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/bundle-2)
$ git add services.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/bundle-2)
$ git commit -m "Added some services"
[ft/bundle-2 4c53a53] Added some services
 1 file changed, 17 insertions(+)
 create mode 100644 services.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/bundle-2)
$ git push
fatal: The upstream branch of your current branch does not match
the name of your current branch.  To push to the upstream branch
on the remote, use

    git push origin HEAD:Bundle2-Ex2

To push to the branch of the same name on the remote, use

    git push origin HEAD

To choose either option permanently, see push.default in 'git help config'.

To avoid automatically configuring an upstream branch when its name
won't match the local branch, see option 'simple' of branch.autoSetupMerge
in 'git help config'.


User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/bundle-2)
$ git push origin HEAD:Bundle2-Ex2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 521 bytes | 173.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Reponse2024/git-revision.git
   55499a9..4c53a53  HEAD -> Bundle2-Ex2

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/bundle-2)
$ git push origin ft/bundle-2
Total 0 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/Reponse2024/git-revision/pull/new/ft/bundle-2
remote:
To https://github.com/Reponse2024/git-revision.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
 ...
=======
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 407 bytes | 407.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/Reponse2024/git-revision.git
   9f54105..b99fb09  main -> main

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$
# Exercise 1 from bundle 1
# Bundle 2
## Exercise 2
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign|MERGING)
$ git add .

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign|MERGING)
$ git commit -m "Merged serivces into main"
[ft/service-redesign 36c819d] Merged serivces into main

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign)
$ git push 
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 227 bytes | 113.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Reponse2024/git-revision.git
   d316da1..36c819d  ft/service-redesign -> ft/service-redesign

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign)
$
```
# Exercise 1 from bundle 1
# Bundle 2
## Exercise 2

```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign)
$ git merge main
Auto-merging services.html
CONFLICT (add/add): Merge conflict in services.html
Automatic merge failed; fix conflicts and then commit the result.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign|MERGING)
$ git add .

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign|MERGING)
$ git commit -m "Merged serivces into main"
[ft/service-redesign 36c819d] Merged serivces into main

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign)
$ git push 
Enumerating objects: 1, done.
Counting objects: 100% (1/1), done.
Writing objects: 100% (1/1), 227 bytes | 113.00 KiB/s, done.
Total 1 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/Reponse2024/git-revision.git
   d316da1..36c819d  ft/service-redesign -> ft/service-redesign

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign)
$
```

# Bundle 3
## Exercise 1
```bash
User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/service-redesign)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/team-page)
$ git add team.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/team-page)
$ git commit -m "Team members"
[ft/team-page 2dc0c3c] Team members
 1 file changed, 17 insertions(+)
 create mode 100644 team.html

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/team-page)
$ git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 2 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 519 bytes | 259.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
remote: 
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/Reponse2024/git-revision/pull/new/ft/team-page
remote:
To https://github.com/Reponse2024/git-revision.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/team-page)
$ git checkout main
M       README.md
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/contact-page)
$ git checkout ft/team-page
M       README.md
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

User@DESKTOP-PQL5SE4 MINGW64 ~/git-exercises (ft/team-page)
$ git log
commit 2dc0c3c55e4ab8034f2947dae92e635015ed47cd (HEAD -> ft/team-page, origin/ft/team-page)
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Tue May 20 09:59:36 2025 +0200

    Team members

commit 36c819d61c98c6aabbce688fb5a1706042dcb589 (origin/ft/service-redesign, ft/service-redesign)
Merge: d316da1 993e7e8
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 18:13:58 2025 +0200

:
commit 2dc0c3c55e4ab8034f2947dae92e635015ed47cd (HEAD -> ft/team-page, origin/ft/team-page)
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Tue May 20 09:59:36 2025 +0200

    Team members

commit 36c819d61c98c6aabbce688fb5a1706042dcb589 (origin/ft/service-redesign, ft/service-redesign)
Merge: d316da1 993e7e8
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 18:13:58 2025 +0200

    Merged serivces into main

commit 993e7e8e37d73265091110549533db78e8d16eb4 (origin/main, origin/HEAD, main, ft/contact-page)
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:20:11 2025 +0200

    Additional services

commit d316da11af4631d85abaadfa8237893e16f10429
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:14:56 2025 +0200
:
    Merged serivces into main

commit 993e7e8e37d73265091110549533db78e8d16eb4 (origin/main, origin/HEAD, main, ft/contact-page)
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:20:11 2025 +0200

    Additional services

commit d316da11af4631d85abaadfa8237893e16f10429
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:14:56 2025 +0200
:
    Merged serivces into main

commit 993e7e8e37d73265091110549533db78e8d16eb4 (origin/main, origin/HEAD, main, ft/contact-page)
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:20:11 2025 +0200

    Additional services

commit d316da11af4631d85abaadfa8237893e16f10429
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:14:56 2025 +0200

    Launched all services

commit 1104df043e462bac929920f69b568b4810565a24
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Thu May 15 10:06:13 2025 +0200

    Initiating project
(END)
commit d316da11af4631d85abaadfa8237893e16f10429
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:14:56 2025 +0200

    Launched all services

commit 1104df043e462bac929920f69b568b4810565a24
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Thu May 15 10:06:13 2025 +0200

    Initiating project
(END)
commit d316da11af4631d85abaadfa8237893e16f10429
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:14:56 2025 +0200

    Launched all services

commit 1104df043e462bac929920f69b568b4810565a24
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Thu May 15 10:06:13 2025 +0200

    Initiating project
(END)
commit d316da11af4631d85abaadfa8237893e16f10429
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:14:56 2025 +0200

    Launched all services

commit 1104df043e462bac929920f69b568b4810565a24
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Thu May 15 10:06:13 2025 +0200

    Initiating project
(END)
commit d316da11af4631d85abaadfa8237893e16f10429
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:14:56 2025 +0200

    Launched all services

commit 1104df043e462bac929920f69b568b4810565a24
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Thu May 15 10:06:13 2025 +0200

    Initiating project
(END)
commit d316da11af4631d85abaadfa8237893e16f10429
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:14:56 2025 +0200

    Launched all services

commit 1104df043e462bac929920f69b568b4810565a24
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Thu May 15 10:06:13 2025 +0200

    Initiating project
(END)
commit d316da11af4631d85abaadfa8237893e16f10429
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:14:56 2025 +0200

    Launched all services

commit 1104df043e462bac929920f69b568b4810565a24
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Thu May 15 10:06:13 2025 +0200

    Initiating project
(END)
commit d316da11af4631d85abaadfa8237893e16f10429
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Mon May 19 17:14:56 2025 +0200

    Launched all services

commit 1104df043e462bac929920f69b568b4810565a24
Author: Reponse <reponse.iduha2023@kepler.org>
Date:   Thu May 15 10:06:13 2025 +0200

    Initiating project
(END)
```

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
