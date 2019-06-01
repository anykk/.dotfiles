## Updating pkglist.txt:
```console
foo@bar:~$ bash -c 'comm -23 <(pacman -Qqett | sort) <(pacman -Qqg base -g base-devel | sort | uniq)' > pkglist.txt
```
## Install packages from pkglist:
```console
foo@bar:~# pacman -S --needed - < pkglist.txt
```

