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
``
##Bundle 2 
## Exercises 1
```bash

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (dev)
$ git checkout -b ft/bundle-2

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git add .

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git commit -m"add: services.html"
[ft/bundle-2 232dc3f] add: services.html
 1 file changed, 11 insertions(+)
 create mode 100644 services.html

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/bundle-2)
$ git push
fatal: The current branch ft/bundle-2 has no upstream branch.
To push the current branch and set the remote as upstream, use

    git push --set-upstream origin ft/bundle-2

To have this happen automatically for branches without a tracking
upstream, see 'push.autoSetupRemote' in 'git help config'.  


user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/bundle-2)
$  git push --set-upstream origin ft/bundle-2
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
 object.
remote:
remote: Create a pull request for 'ft/bundle-2' on GitHub by visiting:
remote:      https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions/pull/new/ft/bundle-2
remote:
To https://github.com/emmanuel-niyonsaba/Gym-Git-Exercise-Solutions.git
 * [new branch]      ft/bundle-2 -> ft/bundle-2
branch 'ft/bundle-2' set up to track 'origin/ft/bundle-2'.

user@EmmauelNiyonsaba MINGW64 /d/CodingRelated/Gym-Git-Exercise-Solutions (ft/bundle-2)
$
