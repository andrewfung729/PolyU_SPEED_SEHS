# SEHS4701 NodeJS Dev Env

Some classmates may be interested in NodeJS development environment setup. This section will guide you through the
installation and configuration of NodeJS development environment.

## Installation

We will use NVM to install NodeJS. NVM is a version manager for NodeJS.

### Mac

```Bash
brew install nvm

# You should create NVM's working directory if it doesn't exist:
mkdir ~/.nvm

# Add the following to ~/.zshrc or your shell's profile:
cat <<EOF >> ~/.zshrc
  export NVM_DIR="$HOME/.nvm"
  [ -s "/opt/homebrew/opt/nvm/nvm.sh" ] && \. "/opt/homebrew/opt/nvm/nvm.sh"  # This loads nvm
  [ -s "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm" ] && \. "/opt/homebrew/opt/nvm/etc/bash_completion.d/nvm"  # This loads nvm bash_completion
EOF
```

## NVM Commands

```Bash
# list all available NodeJS versions
nvm ls-remote

# list all installed NodeJS versions
nvm ls

# install NodeJS latest LTS version
nvm install --lts

# make the installed NodeJS version the default
nvm alias default node
```

## Alternative Package Manager: PNPM

```Bash
brew install pnpm
```