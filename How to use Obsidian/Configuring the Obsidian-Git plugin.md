---
tags:
  - howto
  - git
lastupdated: 2023-11-05
---
#TODO migrate this repo to UCCNetsoc account and write docs on how to configure keys for ssh access
- this repo should ideally be private

as of right now I have a private repo on my own github (git@github.com:colmmurphyxyz/Netsoc-Sysadmin-Resources.git) and have the git plugin configured to automatically commit and push changes regularly, and pull changes from the remote on startup.

# SSH Authentication setup
- to enable the option to push to remotes via ssh I first had to create and add an SSH key to my github account https://docs.github.com/en/authentication/connecting-to-github-with-ssh/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent
- I then had to configure my SSH config file to use this key when connecting to github.com via ssh by adding the following entry to `~/.ssh/config`
```
Host github.com
        User git
        HostName github.com
        IdentityFile ~/.ssh/id_rsa_github # replace with your keypath
        IdentitiesOnly yes # use only this identity file
        AddKeysToAgent yes
```
- when pushing, Obsidian will prompt you to select a remote (`origin` in this case) and enter your private key's passphrase

