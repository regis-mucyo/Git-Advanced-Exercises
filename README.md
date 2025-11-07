# First Advanced Git Exercise

```bash

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises
$ git init -b main
Initialized empty Git repository in D:/The Gym's/PHASE 2/Git Advanced Exercises/.git/

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (main)
$ git add index.html

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (main)
$ git commit -m "Initial project setup"
[main (root-commit) c21070c] Initial project setup
 1 file changed, 45 insertions(+)
 create mode 100644 index.html

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (main)
$ git checkout -b feature/projects
Switched to a new branch 'feature/projects'

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$
 *  History restored



user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)


user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git add index.html

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git commit -m "WIP - added project grid"
[feature/projects f2c39e3] WIP - added project grid
 1 file changed, 6 insertions(+), 1 deletion(-)

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git add index.html

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git commit -m "adding project 2"
[feature/projects c3166cc] adding project 2
 1 file changed, 4 insertions(+)

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git commit -am "fix: typo" --allow-empty
[feature/projects 8774eba] fix: typo

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git log --oneline
8774eba (HEAD -> feature/projects) fix: typo
c3166cc adding project 2
f2c39e3 WIP - added project grid
c21070c (main) Initial project setup

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git rebase -i HEAD~3
[detached HEAD 9b305b8] WIP - added project grid
 Date: Fri Nov 7 06:10:25 2025 +0200
 1 file changed, 10 insertions(+), 1 deletion(-)
Successfully rebased and updated refs/heads/feature/projects.

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git log --oneline
9b305b8 (HEAD -> feature/projects) WIP - added project grid
c21070c (main) Initial project setup

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git reflog
9b305b8 (HEAD -> feature/projects) HEAD@{0}: rebase (finish): returning to refs/heads/feature/projects
9b305b8 (HEAD -> feature/projects) HEAD@{1}: rebase (squash): WIP - added project grid
281b1df HEAD@{2}: rebase (squash): # This is a combination of 2 commits.
f2c39e3 HEAD@{3}: rebase (start): checkout HEAD~3
8774eba HEAD@{4}: commit: fix: typo
c3166cc HEAD@{5}: commit: adding project 2
f2c39e3 HEAD@{6}: commit: WIP - added project grid
c21070c (main) HEAD@{7}: checkout: moving from main to feature/projects
c21070c (main) HEAD@{8}: commit (initial): Initial project setup

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git reset --hard 8774eba
HEAD is now at 8774eba fix: typo

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git log --oneline
8774eba (HEAD -> feature/projects) fix: typo
c3166cc adding project 2
f2c39e3 WIP - added project grid
c21070c (main) Initial project setup

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git rebase -i HEAD~3
[detached HEAD ad85049] feat: add project cards section
 Date: Fri Nov 7 06:10:25 2025 +0200
 1 file changed, 10 insertions(+), 1 deletion(-)
Successfully rebased and updated refs/heads/feature/projects.

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git log --oneline
ad85049 (HEAD -> feature/projects) feat: add project cards section
c21070c (main) Initial project setup

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git status
On branch feature/projects
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git commit -m "add gitignore file"
On branch feature/projects
Untracked files:
  (use "git add <file>..." to include in what will be committed)
        .gitignore

nothing added to commit but untracked files present (use "git add" to track)

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git add .gitignore

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git commit -m "add gitignore file"
[feature/projects 0db9c7b] add gitignore file
 1 file changed, 1 insertion(+)
 create mode 100644 .gitignore

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$ git remote add origin https://github.com/regis-mucyo/Git-Advanced-Exercises.git

user@Regis MINGW64 /d/The Gym's/PHASE 2/Git Advanced Exercises (feature/projects)
$

```
