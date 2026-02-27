# `check_common.py`

Running:
```shell
$ python check_common.py -h
```
prints help:
```
usage: check_common.py [-h] [--tags TAGS] [--file FILE]

Check fixed fortran files for changes in the values in common blocks. CAREFULL this is not
perfect, some value changes may be missed.

options:
  -h, --help       show this help message and exit
  --tags, -t TAGS  Common block name, if not specified all common blocks will be used.
  --file, -f FILE  Path to file for use with ctags, if no files specified *.f will be used.
                   Note all files must be fixed form.
```

Requires:
- `regex` python library for recursive regular expressions
