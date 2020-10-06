# Arch Linux Maintenence Tasks

1. Check systemd failed services:

```
systemctl --failed
```

2. Check Journal entries:

```
sudo journalctl -p 3 -xb
```

3. Update packages:

```
sudo pacman -Syu

yay -Syu
```

4. Remove unwanted dependencies:

```
yay -Yc
```

5. Check for orphans:

```
$ pacman -Qtdq
```

6. Remove Orphans:

```
sudo Pacman -Rns $(pacman -Qtdq)
```

7. Check directory size:

```
du -sh .cache/

du -sh .config/

du -sh /var/log/journal/
```

8. Clean the journal:

```
sudo journalctl vacuum-time=2weeks (in my case)
```

#### references:

> https://wiki.archlinux.org/index.php/System_maintenance

> https://wiki.archlinux.org/index.php/Pacman/Tips_and_tricks
