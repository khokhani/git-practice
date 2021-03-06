# Practice repository to start learning Git


# Commands used
  - git init: Create a Git repository
  - git status: Compare working directory, staging area and current branch
  - git add: Add changes from working directory to staging area
  - git commit: commit changes from staging area to current branch
  - git config: Set or get configurations
  - git log: show a history (aka log) of a commits
  - git checkout: Checkout branch and (update HEAD and apply changes to working directory)
  - git checkout -b: Create branch and then check it out
  - git branch -c : Crate a new branch
  - git branch: List branches
  - git stash: Stash changes from working directory
  - git stash list: List stashes
  - git stash pop: Apply stash changes to working directory
  - git show: Shows single commit
  - git diff: show difference between commits, the working directory and staging area
  - git merge: Merge changes from different branches
  - git remote add <remote> <url>: Add new <remote> at <url>
  - git remote -v: List all remote repositories
  - git push -u <remote> <branch>: Push <branch> to <remote>, and set default upstream for <branch>
  - git fetch: Fetch changes from remote repository
  - git pull: Combine fetch and merge

## What's a branch?
A branch is a ref(rence) to a commit. When HEAD points to a branch we say we'r "on" that branch.
When we make a commit when we'r on that branch, the branch is updated to ref(er) to new commit.

## What's HEAD?
HEAD is a ref(rence) to the current branch (or sometimes a commit...more on this later). Git Commands
like `status`, `log` and `branch` use HEAD. `git checkout` uses HEAD to ref(er) to different branch.

## commit messages

Default editor is vi which can be changed
  - i to enter *insert* mode
  - Type commit message
  - `Esc` -> `:wq` -> `Enter` to write message and quit
Or use `git commit -m "<message>"`

- First line should be clear, accurate, and concise
- Use proper spelling, grammar, and punctuation
- Don't end with `.`

## Merging

Merging means to bring changes from one branch to another.

- A Fast-forward merge happens when target branch was branched from current branch, and there are no new changes in current branch
since then.

- An automatic merge happens when two histories have diverged, but git is able to reconcile them into one set of changes, and create a new commit on current branch.


## What's Remote repository?

A remote repo is hosted somewhere than local machine. We can add remotes with `git remote add`, and setup a *tracking branches* to track a difference between local and remote repositories.

We push to remote with `git push` and fetch from remote using `git fetch`. We can fetch and merge in one command using `git pull`.
