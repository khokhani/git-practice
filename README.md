# Practice repository to start learning Git


# Commands used
  - git init: Create a repository
  - git status: Compare working directory, staging area and current branch
  - git add: Add changes from working directory to staging area
  - git commit: commit changes from staging area to current branch
  - git config: Set or get configurations
  - git log: show a history of commits
  - git branch: List branches
  - git checkout: Checkout branch update HEAD
  - git checkout -b: Create branch and then check it out
  - git stash: Stash changes from working directory
  - git stash list: List stashes
  - git stash pop: Apply stash changes to working directory


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
