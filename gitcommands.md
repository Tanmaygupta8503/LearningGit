### write all the important git commands?
# Initialize a new Git repository:
git init

# Check the status of your working directory:
git status

# Add files to the staging area:
git add <file>
git add .

# Commit changes:
git commit -m "Your commit message"

# View commit history:
git log

# Compare differences between commits:
git diff <commit1>..<commit2>

# Branch management:
# Create a new branch:
git branch <new-branch-name>

# Switch to a different branch:
git checkout <branch-name>

# Merge branches:
git merge <branch-name>

# Undo local changes:
# Unstage a file:
git reset <file>

# Discard changes in a file:
git checkout -- <file>

# Fetch and pull updates from remote repositories:
# Fetch updates:
git fetch origin

# Merge updates into your current branch:
git merge origin/<branch-name>
git pull origin <branch-name>


## Show Remote Repositories
bash
git remote -v

Displays a list of remote repositories along with their URLs.

## Rename a Local Branch
bash
git branch -m <new_branch_name>

Renames the current local branch.

## Delete a Local Branch
bash
git branch -d <branch_name>

Deletes the specified local branch.

## Delete a Remote Branch
bash
git push origin --delete <branch_name>

Removes the specified branch from the remote repository.

## Create and Switch to a New Branch
bash
git checkout -b <new_branch_name>

Creates a new branch and switches to it in a single command.

## Stash Changes
bash
git stash

Temporarily saves changes that are not ready to be committed, allowing you to switch branches.

## Apply Stashed Changes
bash
git stash apply

Applies the last set of stashed changes to the working directory.

## List Stashes
bash
git stash list

Displays a list of all stashed changes.

## Rebase
bash
git rebase <base_branch>

Moves or combines a sequence of commits to a new base commit.

## Interactive Rebase
bash
git rebase -i <base_branch>

Allows you to interactively choose which commits to modify, delete, or squash.

## Show Changes Between Branches
bash
git diff <branch1>..<branch2>

Displays the differences between two branches.

## Show Changes in Staging Area
bash
git diff --cached

Shows the changes between the working directory and the staging area.

## Configure User Information
bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"

Sets the user name and email for Git commits.

## Amend the Last Commit
bash
git commit --amend

Adds changes to the last commit without creating a new commit.