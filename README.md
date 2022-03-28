# Mac Setup

## Homebrew

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

### Formulae

autossh	krb5 nvm	python@3.8 zsh
ca-certificates	libpng	openjdk@8	readline
freetype libpq	openssl@1.1	sqlite
gdbm mpdecimal	openssl@3 tcl-tk
jenv ncurses	pcre xz

### Casks

1password		google-chrome		microsoft-outlook
adoptopenjdk11		insomnia		microsoft-powerpoint
adoptopenjdk14		iterm2			microsoft-teams
atom			jetbrains-toolbox	microsoft-word
carbon-copy-cloner	krisp			miro
docker			microsoft-auto-update	spotify
firefox			microsoft-excel

## iterm2 & zsh

### Install ohmyzsh

`sh -c "$(curl -fsSL https://raw.githubusercontent.com/robbyrussell/oh-my-zsh/master/tools/install.sh)"`

### Plugins

zsh-autosuggestions: `git clone https://github.com/zsh-users/zsh-autosuggestions ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-autosuggestions`

zsh-syntax-highlighting: `git clone https://github.com/zsh-users/zsh-syntax-highlighting.git ${ZSH_CUSTOM:-~/.oh-my-zsh/custom}/plugins/zsh-syntax-highlighting`

List of Plugins:
```
git
brew
docker
history
macos
zsh-autosuggestions
zsh-syntax-highlighting
```

### Styling

iterm color theme: `curl -O https://raw.githubusercontent.com/MartinSeeler/iterm2-material-design/master/material-design-colors.itermcolors`

Import theme in iterm2: *Profiles > Colors > Presets...*

ohmyzsh theme: `git clone --depth=1 https://github.com/romkatv/powerlevel10k.git ${ZSH_CUSTOM:-$HOME/.oh-my-zsh/custom}/themes/powerlevel10k`

Change zsh theme: `ZSH_THEME="powerlevel10k/powerlevel10k"`

###

Change the key mapping preset to `Natural Text Editing` in order to skip words or go to start/end of line: *Profiles > Keys > Key Mappings > Presets...*
