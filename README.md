# Setups
+ vim
+ xcode
+ homebrew
+ zsh
+ git
+ pyenv-virtualenv
+ highlight
+ tree

## vim
> Shell text editor

+ Ubuntu

```
sudo apt-get install vim
```
## xcode
> Integrated development environment for macOS

+ macOS

```
xcode-select --install
```
## homebrew
> Package manager for macOS

+ macOS

```
cd /usr/local
mkdir homebrew && \
curl -L https://github.com/Homebrew/brew/tarball/master | \
tar xz --strip 1 -C homebrew
```
## zsh
> UNIX shell

+ Ubuntu

```
sudo apt-get install zsh
curl -L http://install.ohmyz.sh | sh
chsh -s `which zsh`
```

+ macOS

```
brew install zsh zsh-completions
curl -L http://install.ohmyz.sh | sh
chsh -s `which zsh`
```
> **`chsh: /usr/local/bin/zsh: non-standard shell` error**
> 
> ```
> sudo vim /etc/shells
> ```
> Save `which zsh` result at bottom

## git
> Version control system

+ Ubuntu

```
sudo apt-get install git
```

+ macOS

```
brew install git
```
## pyenv-virtualenv
> Python environment manager

### Install
+ Ubuntu

```
curl -L https://raw.githubusercontent.com/yyuu/pyenv-installer/master/bin/pyenv-installer | bash
```

+ macOS

```
brew install pyenv
brew install pyenv-virtualenv
```
### Bash settings
```
vim ~/.zshrc
```

+ Ubuntu

```
export PATH="$HOME/.pyenv/bin:$PATH"
eval "$(pyenv init -)"
eval "$(pyenv virtualenv-init -)"
```

+ macOS

```
export PYENV_ROOT=/usr/local/var/pyenv
if which pyenv > /dev/null; then eval "$(pyenv init -)"; fi
if which pyenv-virtualenv-init > /dev/null; then eval "$(pyenv virtualenv-init -)"; fi
```
### Common build problems
> https://github.com/pyenv/pyenv/wiki/Common-build-problems

+ Ubuntu

```
sudo apt-get install -y make build-essential libssl-dev zlib1g-dev libbz2-dev \
libreadline-dev libsqlite3-dev wget curl llvm libncurses5-dev libncursesw5-dev \
xz-utils tk-dev
```

+ macOS

```
brew install readline xz
```
## highlight
> Convert source code to formatted text with syntax highlighting

+ macOS

```
brew install highlight
```
## tree
> Display directories as trees

+ macOS

```
brew install tree
```