# alias
### application
> Open an app

```
alias <name>="open -a /path/to/app"
```

+ macOS `/path/to/app`

```
/Application/<app_name>.app/Contents/MacOs/<app_launcher>
```
### ssh
> Connect to AWS server

```
alias <name>="ssh -X -i ~/.ssh/<key_name>.pem \
ubuntn@<server>.compute.amazonaws.com"
```
### scp
> Upload to AWS server

```
alias <name>="scp -r -i ~/.ssh/<key_name>.pem \
path/to/upload_folder \
ubuntu@<server>.compute.amazonaws.com:/srv/app/"
```
# scripts
> Script setting

Open `.zshrc`, `.bashrc` or `.bash_profile`

```
export SCRIPTS_PATH="~/.scripts"
export PATH="$PATH:$SCRIPTS_PATH"
```