# Practice making repository for learning Git

## Commands users

- git init: Create a new git repository
- git status: Compare working directory, staging area, and current branch
- git add: Add changes from working directory to staging area
- git commit: Commit changes from working directory to staging area
- git config: Set or get configuration
- git log: Show a history (aka "log") of project commits
- git show: Show a single commit
- git diff: Show the difference between commits, the working directory, and the staging area
- git checkout: Check out branch (update HEAD and apply changes to working directory)
- git checkout -b: Create branch, then check it out
- git branch -c: Create a branch
- git branch: List branches
- git merge: Merge changes from different branches

## What's a branch?

A branch is a ref(reference) to a commit. When HEAD points to a branch, we say we're "on" that branch. When a commit is made while we're on a branch, the branch is updated to ref to the new commit.

## What's a HEAD?

HEAD is a ref to the "current" branch (or sometimes a commit). Git commands like 'status'. 'log', and 'branch' use HEAD. 'git checkout' updates HEAD to ref to a different branch.

## Commit Messages

Default editor is vim
  ctrl+s to save commit message after adding it
  exit text editor after saving

Easier way is to use 'git commit -m "<message>"'
  This will append your message to the commit without opening a text editor
  Commit message should be clear, accurate, and concise
  Don't end with a '.'

## Merging

Merging means to bring the changes from one branch into another.

- A fast-forward merge happens when the target branch was branched from the current one, and there are no new changes to the current branch since then.
- An Automatic merge happens when the two histories have diverged, but git is able to reconcile them into one set of changes. This creates a new commit on the current branch.
