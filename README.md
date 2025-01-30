
# Practicing GIT Commands

A brief description of what this project does and who it's for

**1. Git Configuration (First-Time Setup)**
| Command | Description |
| --- | --- |
|`git config --global user.name "Your Name"` |Set global username |
| `git config --global user.email "your@email.com"` | Set global email |
|`git config --global core.editor "vim"`|Set the default text editor|
| `git config --global color.ui auto`| Enable colored output |
|`git config --global core.autocrlf true`|Handle line endings automatically (Windows)|
|`git config --global core.autocrlf input`|Handle line endings automatically (Mac/Linux)|
|`git config --global alias.st status`|Create an alias (git st instead of git status)|
|`git config --global init.defaultBranch main`|Set default branch name to main|
|`git config --global credential.helper cache`|Cache credentials for some time|
|`git config --global credential.helper store`|Store credentials permanently|
|`git config --list`|Show all configured Git settings|
|`git config --system --list`|Show system-wide Git settings|
|`git config --global --edit`|Edit the global configuration file|
|`git config --local --edit`|Edit the local configuration file|

**2. Basic Git Commands**

| Command | Description |
| --- | --- |
|`git init`|Initialize a new Git repository|
|`git clone <repo-url>`|	Clone an existing repository|
|`git status`|Show working directory and staging area status|
|`git add <file>`|Add a file to the staging area|
|`git add .`|Add all files to the staging area|
|`git commit -m "message"`|Commit staged changes with a message|
|`git commit -am "message"`|Add and commit modified files in one step|
|`git log`|Show commit history|
|`git show <commit-hash>`|Show details of a specific commit|
|`git diff`|Show unstaged changes|
|`git diff --staged`|Show staged changes|
|`git rm <file-name>`|Remove/ Delete File |
|`git push origin <branch-Name>`|Pushes the main branch to origin but does not set upstream (must specify origin main every time).|
|`git push -u origin <branch-Name>`|Pushes main and sets it as upstream, allowing future git push and git pull without specifying the branch.|
|`git rm <file-name>`|Remove/ Delete File |

**3. Branching and Merging**

| Command | Description |
| --- | --- |
|`git branch`|List all branches|
|`git branch <branch-name>`|Create a new branch|
|`git switch <branch-name>`|Switch to a branch (alternative to checkout)|
|`git merge <branch-name>`|Merge a branch into the current branch|
|`git rebase <branch-name>`|Reapply commits on top of another base branch|
|`git branch -d <branch-name>`|Delete a branch|
|`git branch -D <branch-name>`|Force delete a branch|

**4. Remote Repositories**
| Command | Description |
| --- | --- |
|`git remote -v`|Show remote repositories|
|`git remote add <name> <url>`|Add a new remote repository|
|`git pull <remote> <branch>`|Fetch and merge changes from a remote branch|
|`git fetch <remote>`|Download changes from a remote repository|
|`git push <remote> <branch>`|Push local commits to a remote repository|
|`git push origin --delete <branch>`|Delete a remote branch|

**5. Undoing Changes**
| Command | Description |
| --- | --- |
|`git checkout -- <file>`|Discard changes in a file|
|`git restore <file>`|Restore a file|
|`git reset HEAD <file>`|	Unstage a file|
|`git reset --hard`|Reset all changes to the last commit|
|`git reset --soft HEAD~1`|Undo last commit but keep changes staged|
|`git revert <commit-hash>`|Create a new commit that undoes a previous commit|

**6. Stashing and Cleaning**
| Command | Description |
| --- | --- |
|`git stash`|Temporarily save changes|
|`git stash list`|Show stash history|
|`git stash pop`|Apply and remove the most recent stash|
|`git stash drop`|Remove the most recent stash|
|`git clean -n`|Show untracked files that would be removed|
|`git clean -f`|Delete untracked files|

**7. Advanced Git Commands**

| Command | Description |
| --- | --- |
|`git cherry-pick <commit-hash>`|Apply a specific commit from another branch|
|`git bisect start`|Start binary search to find a bug|
|`git reflog`|Show reference log of changes|
|`git blame <file>`|Show who modified each line in a file|
|`git tag <tag-name>`|Create a lightweight tag|
|`git push origin <tag-name>`|Push a tag to remote|

**8. Git Submodules**

| Command | Description |
| --- | --- |
|`git submodule add <repo-url>`|Add a submodule|
|`git submodule init`|Initialize submodules|
|`git submodule update`|Update submodules|

**9. Git Hooks (Automation & Customization)**

| Command | Description |
| --- | --- |
|`.git/hooks/pre-commit`|Script to run before committing|
|`.git/hooks/post-commit`|Script to run after committing|
|`.git/hooks/pre-push`|Script to run before pushing|

**10. Git Large File Storage (LFS)**

| Command | Description |
| --- | --- |
|`git lfs install`|Install Git LFS|
|`git lfs track "*.psd"`|Track large files|
|`git push origin <branch>`|Push LFS-tracked files|

**11. Git Worktrees (Multiple Workspaces)**

| Command | Description |
| --- | --- |
|`git worktree add <path> <branch>`|Create a new worktree|
|`git worktree list`|Show all worktrees|
|`git worktree remove <path>`|Remove a worktree|

**12. New Git Features (Latest Additions)**

| Command | Description |
| --- | --- |
|`git switch`|Faster alternative to checkout for switching branches|
|`git restore`|Alternative to checkout for restoring files|
|`git sparse-checkout init`|Enable partial cloning (Git v2.25+)|
|`git sparse-checkout set <path>`|Define paths to keep in sparse checkout|
|`git maintenance start`|Enable background repository maintenance|
|`git merge --autostash`|	Automatically stash changes before merging|
|`git commit --fixup <commit-hash>`|Mark commit as a fixup for autosquash|
|`git rebase --autosquash`|Automatically reorder fixup commits|