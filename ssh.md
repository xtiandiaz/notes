# SSH

## Add key (to GitHub)

### Copy public
`pbcopy < ~/.ssh/[key_file_name].pub`

And add at the **SSH and GPG keys** section.

## New key

### Generate
`ssh-keygen -t ed25519 -C "associated@email.com"`

### Start SSH agent in background
`eval "$(ssh-agent -s)"`

### Edit `config`
`code ~/.ssh/config`
```
Host prefix.github.com
  Hostname github.com
  IdentityFile ~/.ssh/[key_file_name]
```
Multiple like entries for separate keys.

### Add private key to the SSH-agent
`ssh-add --apple-use-keychain ~/.ssh/[key_file_name]`

### Test connection
`ssh -T git@prefix.github.com`

## Agent

### Start
`eval "$(ssh-agent -s)`

### List
`ssh-add -l`

### Remove (manually added keys)
Single: `ssh-add -d ~/.ssh/[key_file_name]`
All: `ssh-add -D`

### Add new
`ssh-add ~/.ssh/[key_file_name]`

  
