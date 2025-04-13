# Git Command Cheat Sheet
This repository is a handy reference for **commonly used Git commands**, perfect for beginners and professionals alike. Keep your version control skills sharp with quick access to essential workflows.

All commands are explained clearly and organized into logical categories.

## Git Configuration
| Command | Description |
|--------|-------------|
| `git config --global user.name "Your Name"` | Sets your Git username (global). |
| `git config --global user.email "your.email@example.com"` | Sets your Git email (global). |
| `git config --global core.editor <editor>` | Sets the default text editor. |
| `git config --list` | Lists all Git config settings. |


## Repository Initialization & Cloning
| Command | Description |
|--------|-------------|
| `git init` | Initializes a new Git repository. |
| `git clone <repo_url>` | Clones an existing repository from GitHub or other remote sources. |


## Basic Snapshotting
| Command | Description |
|--------|-------------|
| `git status` | Shows the current state of the working directory and staging area. |
| `git add <file>` | Stages a specific file. |
| `git add .` | Stages all changes (new, modified, deleted). |
| `git commit -m "commit message"` | Commits the staged changes with a message. |
| `git commit -am "message"` | Adds and commits tracked files in one step. |


## Branching
| Command | Description |
|--------|-------------|
| `git branch` | Lists all local branches. |
| `git branch <branch>` | Creates a new branch. |
| `git checkout <branch>` | Switches to an existing branch. |
| `git checkout -b <branch>` | Creates and switches to a new branch. |
| `git merge <branch>` | Merges changes from the specified branch into the current one. |
| `git branch -d <branch>` | Deletes a branch (safe). |
| `git branch -D <branch>` | Force deletes a branch. |


## Working with Remote Repositories
| Command | Description |
|--------|-------------|
| `git remote -v` | Shows the remote URLs associated with the repo. |
| `git remote add origin <url>` | Adds a remote repository URL. |
| `git push origin <branch>` | Pushes current branch to the remote repository. |
| `git push -u origin <branch>` | Pushes and sets upstream tracking. |
| `git fetch` | Fetches latest changes from remote but doesn’t merge. |
| `git pull` | Fetches and merges changes from remote. |
| `git push` | Pushes changes to remote. |


## Undoing Changes
| Command | Description |
|--------|-------------|
| `git reset <file>` | Unstages a file (keeps changes). |
| `git reset --hard` | Resets working directory and staging area to last commit. |
| `git checkout -- <file>` | Restores file to last committed state. |
| `git revert <commit>` | Creates a new commit that reverses changes from the specified commit. |


## Log and History
| Command | Description |
|--------|-------------|
| `git log` | Shows commit history. |
| `git log --oneline` | Condensed view of commit history. |
| `git log --graph` | Visual representation of branch history. |
| `git diff` | Shows unstaged changes. |
| `git diff --staged` | Shows staged changes. |
| `git show <commit>` | Shows changes introduced by a commit. |


## Stashing
| Command | Description |
|--------|-------------|
| `git stash` | Temporarily saves changes that aren’t ready to commit. |
| `git stash apply` | Reapplies last stashed changes. |
| `git stash list` | Lists all stashes. |
| `git stash drop` | Deletes the latest stash. |


## Tagging
| Command | Description |
|--------|-------------|
| `git tag` | Lists all tags. |
| `git tag <tag>` | Creates a new lightweight tag. |
| `git tag -a <tag> -m "message"` | Creates an annotated tag. |
| `git push origin <tag>` | Pushes a specific tag to remote. |


## Rebasing (Advanced)
| Command | Description |
|--------|-------------|
| `git rebase <branch>` | Reapplies commits from current branch on top of another. |
| `git rebase -i <commit>` | Interactive rebase for squashing, editing, reordering commits. |
| `git rebase --abort` | Cancels a rebase in progress. |


## Cleaning
| Command | Description |
|--------|-------------|
| `git clean -n` | Shows what would be deleted. |
| `git clean -f` | Deletes untracked files. |
| `git clean -fd` | Deletes untracked files and directories. |