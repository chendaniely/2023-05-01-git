# 2023-01-05-git

- `git init`: initialize git repository (repo)
	- do not nest git repos
- `git status`: tells you things about what's going on

- `git add`: `git add README.md` add the file to the staging area
- `git commit`: take whatever is in the staging area and commit it
	- `git commit -m "MY MESSAGE"`: quick oneliner message

- `git log`: show you the log of all commit messages
	- `git log --oneline`: 1 line view of log
	- `git log --oneline --all`: shows all of log, not just HEAD

- `HEAD`: tells you where you are

- `git diff`: shows you new changes to the repo
	- `git diff --staged`: shows you changes in the staging area
	- `git diff <HASH> <FILE>`: compare 2 states in the repo

- `git checkout <HASH>`: move HEAD to <HASH>
	- You will be in a detached HEAD state
	- `git switch main` / `git checkout main`: to reattach to main

