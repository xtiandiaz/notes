# Git

## Log
`git log --oneline --graph`

## Push

### First
`git push -u origin main`

## Remote
### List
`git remote -v`

### Set URL
`git remote set-url origin git@[hostname]:[username]/[repo_name].git`

e.g., `[hostname]`: `xtiandiaz.github.com` (as described @ `~/.ssh/config`)

## Config
### User
`git config user.name "Name Surname"` \
`git config user.email "my@email.com"`

@ local repository's file `.git/config`

Optional `--global` flag for `~/.gitconfig` file
