# Gym-Git-Exercise-Solutions

``
## Bundle 1 
### Exercises 2
```bash
ngRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash
No local changes to save

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash
No local changes to save

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash pop
On branch dev
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html
        team.html

no changes added to commit (use "git add" and/or "git commit -a")
Dropped refs/stash@{0} (63a650bba597b9c23cf680712a931019aaff369a)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git status
On branch dev
Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        about.html
        home.html
        team.html

$ git stash about.html
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'about.html'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash clear

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git checkout dev
Switched to branch 'dev'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git reset

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash
No local changes to save

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash
No local changes to save

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash
Saved working directory and index state WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: fbc6f54 Initial commit
stash@{1}: WIP on dev: fbc6f54 Initial commit
stash@{2}: WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{1}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html

Dropped stash@{1} (b1910ce9307cda795f57a5c156a460b9cbbca4cd)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: fbc6f54 Initial commit
stash@{1}: WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped stash@{0} (93760499cd582debe6c6605c4e8cbc849ea4e061)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash push -m"team" [team.html]
error: pathspec ':(prefix:0)[team.html]' did not match any file(s) known to git
Did you forget to 'git add'?

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git add team.html 

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash -m"team"
Saved working directory and index state On dev: team

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: On dev: team
stash@{1}: WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash pop@{0}
fatal: subcommand wasn't specified; 'push' can't be assumed due to unexpected token 'pop@{0}'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{0}
On branch dev
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   about.html
        new file:   team.html

Dropped stash@{0} (98144d94416133b05536626459117c99cb532ad3)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash list 
stash@{0}: WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git commit -m"after-stashing"
[dev 91e8646] after-stashing
 2 files changed, 22 insertions(+)
 create mode 100644 about.html
 create mode 100644 team.html

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git push
fatal: The current branch dev has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin dev

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$  git push --set-upstream origin dev
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (4/4), done.
Writing objects: 100% (4/4), 518 bytes | 518.00 KiB/s, done.
Total 4 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), done.
remote:
remote: Create a pull request for 'dev' on GitHub by visiting:
remote:      https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions/pull/new/dev
remote:
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
 * [new branch]      dev -> dev
branch 'dev' set up to track 'origin/dev'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash list
stash@{0}: WIP on dev: fbc6f54 Initial commit

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git stash pop stash@{0}
On branch dev
Your branch is up to date with 'origin/dev'.

Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        new file:   home.html

Dropped stash@{0} (e3ab86aab4d7ecfaf5c59ba2adfc1eb8916fb44c)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git rest
git: 'rest' is not a git command. See 'git --help'.

The most similar commands are
        restore
        reset

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git reset

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git commit -m"stash pop"
On branch dev
Your branch is up to date with 'origin/dev'.

Changes not staged for commit:
  (use "git add <file>..." to update what will be committed)
  (use "git restore <file>..." to discard changes in working directory)
        modified:   README.md

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        home.html

no changes added to commit (use "git add" and/or "git commit -a")

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git commit -m"stash pop"
[dev 69f6d08] stash pop
 2 files changed, 12 insertions(+), 1 deletion(-)
 create mode 100644 home.html

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git push
Enumerating objects: 6, done.
Counting objects: 100% (6/6), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (4/4), 542 bytes | 542.00 KiB/s, done.
Total 4 (delta 0), reused 0 (delta 0), pack-reused 0 (from 0)
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
   91e8646..69f6d08  dev -> dev

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$
 ```
 ## Bundle 2
 ## Exercises 2
 ```bash
  create mode 100644 team.html

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/service-redesign
Switched to a new branch 'ft/service-redesign'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git commit -m"add:service"
[ft/service-redesign 1d81aa7] add:service
 1 file changed, 11 insertions(+)
 create mode 100644 service.html

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git push
fatal: The current branch ft/service-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/service-redesign

To have this happen automatically for branches without a tracking        
upstream, see 'push.autoSetupRemote' in 'git help config'.


Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 235 bytes | 235.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/service-redesign' on GitHub by visiting:
remote:      https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions/pull/new/ft/service-redesign
remote:
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/service-redesign -> ft/service-redesign
branch 'ft/service-redesign' set up to track 'origin/ft/service-redesign'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/service-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git commit -m"add: service2"
[main cbafee0] add: service2
 1 file changed, 12 insertions(+)
 create mode 100644 service.html

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 440 bytes | 440.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
   f2a7804..cbafee0  main -> main

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git pull
remote: Enumerating objects: 8, done.
remote: Counting objects: 100% (8/8), done.
remote: Compressing objects: 100% (4/4), done.
remote: Total 4 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
Unpacking objects: 100% (4/4), 1.85 KiB | 158.00 KiB/s, done.
From https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions
   cbafee0..1c40168  main                -> origin/main
   1d81aa7..bcdc858  ft/service-redesign -> origin/ft/service-redesign
Updating cbafee0..1c40168
Fast-forward
 service.html | 2 ++
 1 file changed, 2 insertions(+)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git commit -m"done with B2 E2"
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git status
On branch main
Your branch is up to date with 'origin/main'.

nothing to commit, working tree clean
```
## Bundle 3
# Exercises 1
```bash

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/team-page
Switched to a new branch 'ft/team-page'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/team-page)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/team-page)
$ git commit -m"add: team2"
[ft/team-page b7d16bc] add: team2
 1 file changed, 11 insertions(+)
 create mode 100644 team2.html

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/team-page)
$ git push
fatal: The current branch ft/team-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/team-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/team-page)
$  git push --set-upstream origin ft/team-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 435 bytes | 435.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/team-page' on GitHub by visiting:
remote:      https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions/pull/new/ft/team-page
remote:
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/team-page -> ft/team-page
branch 'ft/team-page' set up to track 'origin/ft/team-page'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git checkout -b ft/contact-page
Switched to a new branch 'ft/contact-page'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git checkout ft/team-page 
Switched to branch 'ft/team-page'
Your branch is up to date with 'origin/ft/team-page'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/team-page)
$ git log -1
commit b7d16bca1611b00af6cda3ef08fd0ff44610a2a2 (HEAD -> ft/team-page, origin/ft/team-page)
Author: Emmanuel Niyonsaba <emmanuelniyonsaba40@gmail.com>
Date:   Fri Jul 18 00:22:41 2025 +0200

    add: team2

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/team-page)
$ git checkout ft/contact-page 
Switched to branch 'ft/contact-page'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git cherry-pick b7d16bca1611b00af6cda3ef08fd0ff44610a2a2
[ft/contact-page 1ab0e64] add: team2
 Date: Fri Jul 18 00:22:41 2025 +0200
 1 file changed, 11 insertions(+)
 create mode 100644 team2.html

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git commit -m"add:conatct"
[ft/contact-page c18b616] add:conatct
 1 file changed, 1 insertion(+)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git push
fatal: The current branch ft/contact-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/contact-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/contact-page)
$  git push --set-upstream origin ft/contact-page
Enumerating objects: 8, done.
Counting objects: 100% (8/8), done.
Delta compression using up to 16 threads
Compressing objects: 100% (6/6), done.
Writing objects: 100% (6/6), 642 bytes | 642.00 KiB/s, done.
Total 6 (delta 4), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (4/4), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/contact-page' on GitHub by visiting:
remote:      https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions/pull/new/ft/contact-page
remote:
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/contact-page -> ft/contact-page
branch 'ft/contact-page' set up to track 'origin/ft/contact-page'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/contact-page)
$ git checkout -b ft/faq-page
Switched to a new branch 'ft/faq-page'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git commit -m"add faq-page"
[ft/faq-page 4651a90] add faq-page
 1 file changed, 11 insertions(+)
 create mode 100644 faq.html

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push
fatal: The current branch ft/faq-page has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/faq-page

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push --set-upstream origin ft/faq-page
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 432 bytes | 432.00 KiB/s, done.
Total 3 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
remote:
remote: Create a pull request for 'ft/faq-page' on GitHub by visiting:
remote:      https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions/pull/new/ft/faq-page
remote:
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/faq-page -> ft/faq-page
branch 'ft/faq-page' set up to track 'origin/ft/faq-page'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git revert <b7d16bca1611b00af6cda3ef08fd0ff44610a2a2>
bash: syntax error near unexpected token `newline'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git revert b7d16bca1611b00af6cda3ef08fd0ff44610a2a2
hint: Waiting for your editor to close the file... Vim: Error reading input, exiting...
Vim: Finished.

error: there was a problem with the editor 'vi'
Please supply the message using either -m or -F option.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git commit -m"after revert"
[ft/faq-page 31a8754] after revert
 1 file changed, 11 deletions(-)
 delete mode 100644 team2.html

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git push
Enumerating objects: 3, done.
Counting objects: 100% (3/3), done.
Delta compression using up to 16 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (2/2), 232 bytes | 232.00 KiB/s, done.
Total 2 (delta 1), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (1/1), completed with 1 local object.
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
   4651a90..31a8754  ft/faq-page -> ft/faq-page
```
## Bundle 3
## Exercises 2
```bash
user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git chechout -b ft/home-page-redesign
git: 'chechout' is not a git command. See 'git --help'.

The most similar command is
        checkout

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git chechout -b ft/home-page-redesign
git: 'chechout' is not a git command. See 'git --help'.

The most similar command is
        checkout

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/faq-page)
$ git checkout -b ft/home-page-redesign
Switched to a new branch 'ft/home-page-redesign'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git commit -m"add:change3"
[main e98deba] add:change3
 1 file changed, 1 insertion(+)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 325 bytes | 325.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
   861f3b2..e98deba  main -> main

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git rebase main
Auto-merging home.html
CONFLICT (content): Merge conflict in home.html
error: could not apply c18b616... add:conatct
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
hint: Disable this message with "git config set advice.mergeConflict false"
Could not apply c18b616... # add:conatct

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign|REBASE 2/4)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git commit -m"after rebase"
[ft/home-page-redesign a31de48] after rebase
 1 file changed, 1 insertion(+)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 16 threads
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 1.43 KiB | 733.00 KiB/s, done.
Total 14 (delta 8), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (8/8), completed with 2 local objects.
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$
```
## Bundle 4
## Exercises 1
```bash
[main e98deba] add:change3
 1 file changed, 1 insertion(+)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 325 bytes | 325.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
   861f3b2..e98deba  main -> main

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git checkout ft/home-page-redesign
Switched to branch 'ft/home-page-redesign'

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git rebase main
Auto-merging home.html
CONFLICT (content): Merge conflict in home.html
error: could not apply c18b616... add:conatct
hint: Resolve all conflicts manually, mark them as resolved with
hint: "git add/rm <conflicted_files>", then run "git rebase --continue".
hint: You can instead skip this commit: run "git rebase --skip".
hint: To abort and get back to the state before "git rebase", run "git rebase --abort".
hint: Disable this message with "git config set advice.mergeConflict false"
Could not apply c18b616... # add:conatct

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign|REBASE 2/4)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git commit -m"after rebase"
[ft/home-page-redesign a31de48] after rebase
 1 file changed, 1 insertion(+)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git push
fatal: The current branch ft/home-page-redesign has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/home-page-redesign

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.


user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git push --set-upstream origin ft/home-page-redesign
Enumerating objects: 16, done.
Counting objects: 100% (16/16), done.
Delta compression using up to 16 threads
Compressing objects: 100% (14/14), done.
Compressing objects: 100% (14/14), done.
Writing objects: 100% (14/14), 1.43 KiB | 733.00 KiB/s, done.
Writing objects: 100% (14/14), 1.43 KiB | 733.00 KiB/s, done.
Total 14 (delta 8), reused 0 (delta 0), pack-reused 0 (from 0)
Total 14 (delta 8), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (8/8), completed with 2 local objects.
remote: Resolving deltas: 100% (8/8), completed with 2 local objects.
remote:
remote:
remote: Create a pull request for 'ft/home-page-redesign' on GitHub by visiting:
remote:      https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions/pull/new/ft/home-page-redesign
remote:
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/home-page-redesign -> ft/home-page-redesign
branch 'ft/home-page-redesign' set up to track 'origin/ft/home-page-redesign'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/home-page-redesign)
$ git checkout main
Switched to branch 'main'
Your branch is up to date with 'origin/main'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git commit -m"done by B3 e2"
[main 4c1c366] done by B3 e2
 1 file changed, 101 insertions(+)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git push
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 1.05 KiB | 1.05 MiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
   e98deba..4c1c366  main -> main

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$
 *  History restored 


user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git remote add git-copy https://github.com/emmanuel-niyonsaba/git-copy.git

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git commit -m"add:remote-repo"
[main 7133eea] add:remote-repo
 1 file changed, 1 insertion(+)

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git push 
Enumerating objects: 5, done.
Counting objects: 100% (5/5), done.
Delta compression using up to 16 threads
Compressing objects: 100% (3/3), done.
Writing objects: 100% (3/3), 335 bytes | 335.00 KiB/s, done.
Total 3 (delta 2), reused 0 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (2/2), completed with 2 local objects.
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
   4c1c366..7133eea  main -> main

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ git push git-copy
Enumerating objects: 45, done.
Counting objects: 100% (45/45), done.
Delta compression using up to 16 threads
Compressing objects: 100% (42/42), done.
Writing objects: 100% (45/45), 10.18 KiB | 1.70 MiB/s, done.
Total 45 (delta 23), reused 3 (delta 0), pack-reused 0 (from 0)
remote: Resolving deltas: 100% (23/23), done.
To https://github.com/emmanuel-niyonsaba/git-copy.git
 * [new branch]      main -> main

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ ^C


user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (main)
$ 