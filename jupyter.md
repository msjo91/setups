# Jupyter Notebook
+ Install Jupyter Notebook

```
pip install jupyter
```

+ Save .ipynb as .py

```
!jupyter nbconvert --to script [filename].ipynb
```

+ Install Jupyter theme

```
pip install git+https://github.com/dunovank/jupyter-themes.git
```
Thank you, dunovank! (https://github.com/dunovank/jupyter-themes)

+ Apply theme

```
jupyter-theme -T -t <theme> -f <code-font> -fs <code-fontsize>
```

+ Command line options

cl options | arg | default
--- | --- | ---
Help | -h  | --
List themes | -l | --
Theme name to install | -t | --
Code font | -f | --
Code fontsize | -fs | 11
Notebook font | -nf | --
Notebook fontsize | -nfs | 13
Text/MD cell font | -tf | --
Text/MD cell fontsize | -tfs | 13
Pandas DF fontsize | -dfs | 9
Output area fontsize | -ofs | 8.5
Mathjax fontsize (%) | -mathfs | 100
Intro page margins | -m | auto
Cell width | -cellw | 980
Line height | -lineh | 170
Cursor width | -cursw | 2
Cursor colour | -cursc | --
Alt prompt layout | -altp | --
Alt markdown BG colour | -altmd | --
Alt output BG colour | -altout | --
Style VIM NBExt* | -vim | --
Toolbar visibility | -T | --
Name & logo visibility | -N | --
Reset default theme | -r | --
Force default font | -dfonts | --

### Source-code-pro
+ Install source-code-pro

```
brew tap caskroom/fonts
brew install font-source-code-pro
```

+ Jupyter theme example

```
jupyter-theme -T -t onedork -f source -fs 12
```
