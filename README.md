# Mac Setup

A few tools/configs to setup MacOS for Devs.

## Homebrew

Install homebrew:

`/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"`

Create bundle:

`brew bundle dump`

Install bundle:

`brew bundle install`

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

## Java & jenv

`jenv` helps managing multiple Java versions. 

### Shell config

```
export PATH="$HOME/.jenv/bin:$PATH"
eval "$(jenv init -)"
```

### (optional) support for mvn a.o.

```
# ensure that JAVA_HOME is correct
jenv enable-plugin export
# make Maven aware of the Java version in use (and switch when your project does)
jenv enable-plugin maven
```
### Adding new Java versions

Install new Java version via brew (e.g. `brew install adoptopenjdk11`).

List installed versions:

```
/usr/libexec/java_home -V
```

Add new version: 

```
jenv add <jdk_path>
```
