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