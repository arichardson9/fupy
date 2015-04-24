### Description ###
A small and dirty Python 2 decompiler written in Python.


### Dependencies ###
Only a standard CPython interpreter is needed. The decompiler is contained in a single file.

The standard module `dis` is used to disassemble the bytecode, so you will probably need the same version of Python that was used to compile the target file.


### Compatibility ###
Not compatible with Python 3 bytecode. Only tested against 2.5, 2.6 and 2.7.

Probably full of bugs (this was just a pretext for me to learn Python). Feel free to report any problem though.


---


```
Usage: ./fupy [options] <pycfile>
Reverse a Python pyc file back into a human readable form.
 -h, --help                Display this message.
 --disass                  Disassemble bytecode only.
 -i style, --indent=style  Set indentation style (default to 4s).
                            style is [num]char where char is 's' for spaces or 't' for tabs.
 -o file, --output=file    Redirect output to file (default to stdout).
```