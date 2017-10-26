# Brew formula
+ Requirement

> homebrew

+ Check installed formulae

```
brew list
```

+ Check installed formulae and dependencies

```
brew list | while read cask; do echo -n $fg[blue] $cask $fg[white]; brew deps $cask | awk '{printf(" %s ", $0)}'; echo ""; done
```

+ Check available formulae

```
brew search
```

+ Search formulae with keyword

```
brew search <keyword>
```

+ Install formula

```
brew install <formula>
```

+ Update all

```
brew update
```

+ Upgrade all

```
brew upgrade
```

+ Cleanup all

```
brew cleanup
```

+ Call download path

```
brew --cache
```

+ Uninstall

```
brew uninstall <formula>
```
# Virtual python environment
+ Requirement
> pyenv  
> pyenv-virtualenv

+ Check installed python versions

```
pyenv versions
```

+ Check available python versions

```
pyenv install --list
```

+ Install python version

```
pyenv install <version>
```

+ Create virtual environment

```
pyenv virtualenv <version> <venv_name>
```

+ Apply virtual environment

```
pyenv local <venv_name>
```

+ Check applied python environment

```
pyenv version
```

+ Uninstall python environment

```
pyenv uninstall <env_name>
```

# PIP
+ Check installed packages

```
pip list
```

+ Install package

```
pip install <package>
```

+ Install packages in requirements.txt

```
pip install -r requirements.txt
```

+ Check upgrades

```
pip list --outdated
```

+ Upgrade packages

```
pip install --upgrade <package>
```

+ Save package info in requirements.txt

```
pip freeze > requirements.txt
```

+ Uninstall

```
pip uninstall <package>
```

+ Uninstall all

```
pip freeze | grep -v "^-e" | xargs pip uninstall -y
```