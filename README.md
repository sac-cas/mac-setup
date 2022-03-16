# Mac Setup

## Homebrew

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

### Formulae

openjdk@8	zsh	libpq

### Casks

1password	iterm2 microsoft-outlook
atom jetbrains-toolbox	microsoft-powerpoint
carbon-copy-cloner krisp	microsoft-teams
docker microsoft-auto-update microsoft-word
google-chrome microsoft-excel spotify

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
