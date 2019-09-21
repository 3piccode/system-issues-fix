# Note: Before any fix start with ->
```shell
      $ sudo apt-get update
 ```
--- --- ---

# The following packages have unmet dependencies: linuxbrew-wrapper : Depends: zlib1g-dev but it is not going to be installed. E: Unable to correct problems, you have held broken packages.

Fix : Take note of the required package version (in your case = 1:1.2.8.dfsg-2ubuntu4)
 ```shell
 $ sudo apt install zlib1g=1:1.2.8.dfsg-2ubuntu4
 ```
 
 ---- --- ----
# Ubuntu Launcher fix.
1. try
```shell
$ sudo service lightdm restart
```
2. If restarting lightdm does not fix the issue, install:
```shell
$ sudo apt-get install unity
```
and
```shell
$ sudo apt-get --reinstall ubuntu-desktop
```
fellowed by
```shell
$ sudo service lightdm restart
```
