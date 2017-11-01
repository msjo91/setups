# Matplotlib
### Use in macOS
Open python shell

```
import matplotlib as mpl
print(mpl.matplotlib_fname())
```
Close python shell

```
vi path/to/matplotlibrc
```
Find backend

```
backend      : macosx
```
Replace backend

```
backend      : Tkagg
```
### Font cache error
> UserWarning: Matplotlib is building the font cache using fc-list. This may take a moment.  
> 'Matplotlib is building the font cache using fc-list.

Open python shell

```
import matplotlib as mpl
print(mpl.get_cachedir())
```
Close python shell

```
cd path/to/.matplotlib
```
Remove `fontList.cache`, `fontList.py3k.cache`, `tex.cache`