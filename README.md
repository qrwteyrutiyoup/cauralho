# cAURalho

cAURalho is a small tool to help with updating AUR packages installed in the system. It displays in a `dialog` the list of packages for which the local version differs from the one in the AUR, and gives the user the change to individually select the ones the user would like to update.

The update itself is done with the AUR helper ([look here for more information on the available AUR helpers](https://wiki.archlinux.org/index.php/AUR_helpers)) the user already has installed and uses regularly.

## Requirements

cAURalho requires `bash` 4.x or newer, `dialog`, `curl`,  `jq`  and an AUR helper.

## Configuration

Simply define the `AUR_HELPER` variable in `/etc/cauralho.conf`.
E.g.: to use [`yay`](https://github.com/Jguer/yay) as the helper, one could have the variable set as:
```
AUR_HELPER="yay -S"
```

## Screenshot
![cAURalho in action](https://i.imgur.com/NEU8rCN.png)

## License
cAURalho is licensed under Apache License 2.0.

