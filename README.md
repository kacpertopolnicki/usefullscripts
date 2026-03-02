# `check_common.py`

Analize fortran source files (fixed form only) for changes of variables in common blocks.
This might be usefull, for example, when adding OpenMP directives to a program.

Running
```shell
$ python check_common.py -h
```
prints help information:
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
- `regex` python library for recursive regular expressions,
- `ctags` program to generate tags for vim / neovim.

# `rec.py`

Simple module for recording and visualizing the state of python variables in the execution of
some code or algorithm. This might be usefull for teaching purpouses or debugging. Example usage is
in the `__main__` block of `rec.py`. More information is available in the comments.
