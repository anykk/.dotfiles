# Updating requirements:
```console
foo@bar:~$ bash -c 'comm -23 <(pacman -Qqett | sort) <(pacman -Qqg base -g base-devel | sort | uniq)' > requirements.txt
```
