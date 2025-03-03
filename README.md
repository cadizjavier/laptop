## Laptop

Laptop is a script to set up macOS for development, and to keep it up to date.

### Install

 - `git clone git://github.com/cadizjavier/laptop ~/.laptop`
 - `cd ~/.laptop`
 - `source mac`

### What it sets up

 - Homebrew for managing operating system libraries.
 - [Antidote](https://github.com/mattmc3/antidote) for managing zsh dependencies.
 - Zsh [pure](https://github.com/sindresorhus/pure) prompt.

 ### Manual installations
 > TODO: Configure those through brew cask

  - [Ghostty](https://ghostty.org/)

### SSH configuration
```
Host *
    AddKeysToAgent yes
    UseKeychain yes
```
This configuration ensures that SSH keys are automatically added to the SSH agent, so you don’t have to type the passphrase every time you use SSH.

1. Run `ssh-add --apple-use-keychain ~/.ssh/id_rsa`. Replace with your actual private key file.
2. Type `ssh -T git@github.com` to check everything is working as expected.