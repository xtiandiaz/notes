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
Host github.com
AddKeysToAgent yes
UseKeychain yes
IdentityFile ~/.ssh/[key_file_name]
```
Multiple like entries for separate keys.

### Add private key to the SSH-agent
`ssh-add --apple-use-keychain ~/.ssh/[key_file_name]`

  
