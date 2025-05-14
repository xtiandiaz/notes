# Git

## Add
### By force (file excluded in `.gitignore`)
`git add path/to/file -f`

## Clean
To remove untracked files from the working tree
`git clean [-f]`

## Commit
### Amend latest message
`git commit --amend -m <message>`

## Diff
`git diff <commit>`

## Move
`git mv [<options>] <source> <destination>`

## Remove
`git rm [-f] [-r] <path>`

## Reset 
### Rewind history
`git reset --hard <commit> && git clean -f`

## Log
`git log --oneline --graph`

## Remote
### Add origin
`git remote add orign git@<hostname>:<username>/<repo-name>.git`

### List
`git remote -v`
### Set URL
`git remote set-url origin git@<hostname>:<username>/<repo-name>.git`
e.g., `<hostname>`: `xtiandiaz.github.com` (as described @ `~/.ssh/config`)

## Branch

### Set tracking info.
`git branch --set-upstream-to=origin/<remote-branch> <local-branch>`

## Pull
### Unrelated histories
`git pull origin main --allow-unrelated-histories`
### Without merge, just rebase
`git pull --rebase`

## Push
### First
`git push -u origin main`

## Rebase
### All commits from current to root
`git rebase --root -i`
### For N commits
`git rebase -i HEAD~N`
### From some commit
`git rebase -i <commit>`
#### Amend
`git commit --amend --author="Name <email>" --no-edit`

## Reset
### Forfeit all extra local commits
`git reset --hard origin/main`

### Revert previous commit

`git reset --soft HEAD~1`

But leaves its changes staged.

## Restore

### All staged files
`git restore --staged .`

## Config
### User
`git config user.name <name-or-username> [--global]` \
`git config user.email <email> [--global]`

Local repository's file: `.git/config` \
Global: `~/.gitconfig`

### Submodule
Location: `.git/modules/<name>/config`



## Show
### Summary of commit
`git show <commit> --stat`



## Submodule
### Add
`git submodule add git@<hostname>:<username>/<repo-name>.git <optional-subfolder>`

### Deinit
`git submodule deinit -f -- <path>`
#### All
`git submodule deinit -f --all`

### Update
`git submodule update --init --recursive`

### Remove
`git rm <submodule-folder>` [`--cached`]

### Status
`git submodule status` Lists all active submodules
