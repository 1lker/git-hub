
# Commonly Used Git Bash Commands

## Basic Commands
- `git init`  
  Initialize a new Git repository in the current directory.

- `git clone <repository-url>`  
  Clone a repository from a remote source.

- `git status`  
  Show the status of the working directory and staging area.

- `git add <file>`  
  Add a specific file to the staging area.

- `git add .`  
  Add all files in the current directory to the staging area.

- `git commit -m "commit message"`  
  Commit staged changes with a message.

- `git commit -am "commit message"`  
  Stage and commit changes to tracked files in one step.

## Branch Management
- `git branch`  
  List all branches in the repository.

- `git branch <branch-name>`  
  Create a new branch.

- `git checkout <branch-name>`  
  Switch to a specific branch.

- `git checkout -b <branch-name>`  
  Create and switch to a new branch.

- `git merge <branch-name>`  
  Merge a specific branch into the current branch.

- `git branch -d <branch-name>`  
  Delete a local branch.

## Remote Repository
- `git remote -v`  
  Show the URLs of remote repositories.

- `git push <remote> <branch>`  
  Push changes to a remote repository.

- `git pull`  
  Fetch and integrate changes from a remote repository.

- `git fetch`  
  Download changes from a remote repository without merging.

## Logs and History
- `git log`  
  View the commit history.

- `git log --oneline`  
  View a compact commit history.

- `git diff`  
  Show changes between commits, branches, or the working directory.

- `git diff --staged`  
  Show changes between the staging area and the last commit.

## Undoing Changes
- `git reset <file>`  
  Unstage a file.

- `git reset --hard`  
  Reset the working directory and staging area to the last commit.

- `git reset --soft <commit>`  
  Undo commits while keeping changes in the staging area.

- `git revert <commit>`  
  Create a new commit that undoes the specified commit.

## Tagging
- `git tag`  
  List all tags in the repository.

- `git tag <tag-name>`  
  Create a new tag.

- `git push origin <tag-name>`  
  Push a tag to a remote repository.

## Stashing Changes
- `git stash`  
  Save uncommitted changes for later use.

- `git stash list`  
  View a list of stashed changes.

- `git stash apply`  
  Apply stashed changes.

- `git stash drop`  
  Remove a specific stash entry.

## Other Useful Commands
- `git config --global user.name "<your-name>"`  
  Set the global username for Git.

- `git config --global user.email "<your-email>"`  
  Set the global email for Git.

- `git blame <file>`  
  Show who last modified each line of a file.

- `git show <commit>`  
  Display information about a specific commit.
