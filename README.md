## Updating `Packages`:
```console
foo@bar:~$ comm -23 <(pacman -Qqett | sort) <(pacman -Qqg base -g base-devel | sort | uniq) > Packages
```
## Install packages:
```console
foo@bar:~# yay -S --needed - < Packages
```
