# 2023-01-05-git: git bacis

- `git init`: initialize git repository (repo)
	- do not nest git repos
- `git status`: tells you things about what's going on

- `git add`: `git add README.md` add the file to the staging area
- `git commit`: take whatever is in the staging area and commit it
	- `git commit -m "MY MESSAGE"`: quick oneliner message

## history

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

- Delete README.md file
	- THis can also be reverting previous file state
- `git status`: this is your friend
	- `git restore <FILE>`: to revert file to pre commimt stage
- `git checkout <HASH> <FILE>`: revert file from any point in time
- `git restore --source=<HASH> <FILE>`: the "newer" way to restore a file

## Ignore

- `.gitignore`: file of patterns for which files/folders to ignore
- `.gitkeep`: convention to put a file in a folder you want empty

# remotes

- `ssh-keygen`: create a ssh key
	- copy the `~/.ssh/id_rsa.pub` to your github account
	- use the SSH URL not the HTTPS url

- `git remote add <NAME> <URL>`: `git remote add origin <URL>`
	- create the remote connection
- `git push <REMOTE> <BRANCH>`: `git push origin main`
	- push our code to the remote
- `git pull <REMOTE> <BRANCH>`
	- pull code from the remote

# merge conflicts

- You can use the github pencil to edit files directly on github
