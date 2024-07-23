# EndeavourOS Help! 🆘
 Tips and trick to help you do development in EndeavorOS (An Arch Based Linux Distro) \
**Note:** Most of these tips should work for other Arch based Distributions as well! 😉

# Install EndeavorOS using offline mode
Installing EndeavourOS via offline mode helps minimize system compatibility. You can always change the desktop env later if you don't like KDE. (Who doesn't like KDE 🤷?)

# System Upkeep! 

## Useful pacman (and yay commands)

### Update system
> sudo pacman -Syy

> yay -Syy

### Checking number of cached packages
> sudo ls /var/cache/pacman/pkg/ | wc -l

### Dealing with Package Cache!

### Checking the disk size of the cached packages
> du -sh /var/cache/pacman/pkg/

### Remove all uninstalled packages from cache
> sudo pacman -Sc

> yay -Sc

Thank you❣️
Senthilkumar Palani (aka SK)
<br>
<a href="https://ostechnix.com/recommended-way-clean-package-cache-arch-linux" target="_blank"/>The Recommended Way To Clean The Package Cache In Arch Linux</a>

### Removing Packages
**pacman** - To remove packages from the offical ARCH repo \
**yay** - To remove packages from the AUR repo

> sudo pacman -R <package_name>

> yay -R <package_name>

<br>

## Nvidia Drivers

Make sure to choose the proper installation from the installation menu
> nvidia-inst

<br>

## Development Tools (The ones I use anyway)

### Pyenv (For Python Version Management)
> sudo pacman -S pyenv

[Arch Package](https://archlinux.org/packages/extra/any/pyenv/)

### Postman (API Client)
The binary from the company works great and allows updating through the client \
Just add it to your Application Menu.  \
[Postman Website](https://www.postman.com/downloads/)



