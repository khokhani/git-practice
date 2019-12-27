# Practice repository to start learning Git


# Commands used
  - git init: Create a Git repository
  - git status: Compare working directory, staging area and current branch
  - git add: Add changes from working directory to staging area
  - git commit: commit changes from staging area to current branch
  - git config: Set or get configurations
  - git log: show a history of a (log of) commits
  - git checkout: Checkout branch and (update HEAD and apply changes to working directory). In Master branch.
  - git merge: Merge changes from different branches

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
