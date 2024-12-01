# Essential Git Bash Commands

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

- `git add -A`  
  Add all changes (new, modified, deleted) to staging area.

- `git commit -m "commit message"`  
  Commit staged changes with a message.

- `git commit -am "commit message"`  
  Stage and commit changes to tracked files in one step.

- `git commit --amend -m "new message"`  
  Modify the last commit message.

## Branch Management
- `git branch`  
  List all local branches.

- `git branch -a`  
  List all local and remote branches.

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

- `git branch -D <branch-name>`  
  Force delete a local branch.

- `git push origin --delete <branch-name>`  
  Delete a remote branch.

## Remote Repository
- `git remote -v`  
  Show the URLs of remote repositories.

- `git remote add origin <repository-url>`  
  Add a remote repository.

- `git push -u origin <branch-name>`  
  Push and set upstream branch.

- `git push <remote> <branch>`  
  Push changes to a remote repository.

- `git push --force`  
  Force push changes (use with caution).

- `git pull`  
  Fetch and integrate changes from a remote repository.

- `git pull --rebase`  
  Pull changes and rebase local commits.

- `git fetch`  
  Download changes from a remote repository without merging.

- `git fetch --all`  
  Fetch all remotes.

## Logs and History
- `git log`  
  View the commit history.

- `git log --oneline`  
  View a compact commit history.

- `git log --graph`  
  View commit history as a graph.

- `git log -p`  
  Show commit history with diffs.

- `git log --author="username"`  
  View commits by specific author.

- `git diff`  
  Show changes between commits, branches, or working directory.

- `git diff --staged`  
  Show changes between staging area and last commit.

- `git diff <branch1> <branch2>`  
  Show differences between two branches.

## Undoing Changes
- `git reset <file>`  
  Unstage a file.

- `git reset --hard`  
  Reset working directory and staging area to last commit.

- `git reset --soft HEAD~1`  
  Undo last commit keeping changes staged.

- `git reset --hard HEAD~1`  
  Remove last commit and its changes completely.

- `git reset --hard origin/<branch-name>`  
  Reset local branch to match remote branch.

- `git revert <commit>`  
  Create a new commit that undoes specified commit.

- `git clean -fd`  
  Remove untracked files and directories.

- `git checkout -- <file>`  
  Discard changes in working directory.

## Stashing Changes
- `git stash`  
  Save uncommitted changes for later.

- `git stash save "message"`  
  Stash changes with a description.

- `git stash list`  
  View list of stashed changes.

- `git stash apply`  
  Apply most recent stash.

- `git stash apply stash@{n}`  
  Apply specific stash.

- `git stash pop`  
  Apply and remove most recent stash.

- `git stash drop stash@{n}`  
  Remove specific stash.

- `git stash clear`  
  Remove all stashed changes.

## Configuration
- `git config --global user.name "<your-name>"`  
  Set global username.

- `git config --global user.email "<your-email>"`  
  Set global email.

- `git config --list`  
  List all configurations.

- `git config --global core.editor "<editor>"`  
  Set default text editor.

- `git config --global alias.<shortcut> "<command>"`  
  Create command alias.

## Advanced Commands
- `git blame <file>`  
  Show who modified each line of a file.

- `git show <commit>`  
  Display information about a specific commit.

- `git reflog`  
  View history of HEAD updates.

- `git cherry-pick <commit>`  
  Apply changes from specific commit.

- `git rebase -i HEAD~n`  
  Interactive rebase for last n commits.

- `git bisect start`  
  Binary search for bugs.

- `git archive --format=zip HEAD > archive.zip`  
  Create ZIP archive of repository.

- `git shortlog -sn`  
  Show commit count by author.
