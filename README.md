# Git Workflow and History Management

This repository was created for Homework 1.

It demonstrates:
- commit history cleanup
- lost commit recovery with reflog
- branch creation from a recovered commit
- custom alias for history
- version tagging

## Custom Git Alias

In this project I also created a custom Git alias for viewing commit history in a cleaner way.

Alias used:

`git config --global alias.hist "log --oneline --graph --decorate --all"`

After creating it, I could use:

`git hist`

This made it easier to visualize branches, commits, and tags in a simplified format.

## Key Git Commands Used

- `git rebase -i --root` to clean commit history
- `git reflog` to recover a lost commit
- `git switch -c recovered-branch` to create a branch from the recovered commit
- `git tag v1.0` to mark the cleaned version