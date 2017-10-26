# Ipython shell for pyspark
Create script path and file

```
mkdir /path/to/.scripts
vi ipyspark.sh
```
Save below

```
#!/bin/bash
export PYSPARK_DRIVER_PYTHON=ipython

${SPARK_HOME}/bin/pyspark
```
Change permission

```
chmod 711 ipyspark.sh
```
Open `.zshrc`, `.bashrc` or`.bash_profile`

```
export PATH=$PATH:/path/to/.scripts
alias ipyspark="bash /path/to/.scripts/ipyspark.sh"
```
