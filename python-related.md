# 1. When upgrading pip on Linux, the `pip` command stops working ("cannot import main")

Solve this issue by clear hash in bash:

```shell
$ hash -d pip
```

Or in dash (sh):

```shell
$ hash -r pip
```
* For more detail https://github.com/pypa/pip/issues/5221

--- --- ---
