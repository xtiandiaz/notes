# Git

## Log
`git log --oneline --graph`
### First
`git push -u origin main`

## Remote
### Add
`git remote add orign git@[hostname]:[username]/[repo_name].git`

### List
`git remote -v`
### Set URL
`git remote set-url origin git@[hostname]:[username]/[repo_name].git`
e.g., `[hostname]`: `xtiandiaz.github.com` (as described @ `~/.ssh/config`)

## Branch

### Set tracking info.
`git branch --set-upstream-to=origin/<remote-branch> <local-branch>`

## Add
### By force (file excluded in `.gitignore`)
`git add path/to/file -f`

## Pull
### Unrelated histories
`git pull origin main --allow-unrelated-histories`
### Without merge, just rebase
`git pull --rebase`

## Reset
## Forfeit all extra local commits
`git reset --hard origin/main`

## Rebase
### All commits from current to root
`git rebase --root -i`
### For N commits
`git rebase -i HEAD~N`
### From some commit
`git rebase -i <commit>`
#### Amend
`git commit --amend --author="Name <email>" --no-edit`

## Config
### User
`git config user.name [name_or_username]` \
`git config user.email [e_mail]`

@ local repository's file `.git/config`

Optional `--global` flag for `~/.gitconfig` file

#### Submodule
Location: `.git/modules/[name]/config`

## Submodules
### Add
`git submodule add git@[hostname]:[username]/[repo_name].git [optional_subfolder]`

### Remove
`git rm [submodule_folder]`
