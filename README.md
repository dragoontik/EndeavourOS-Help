# EndeavourOS-Help
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
* sudo pacman -Sc
* yay -Sc

Thank you❣️
Senthilkumar Palani (aka SK)
<br>
<a href="https://ostechnix.com/recommended-way-clean-package-cache-arch-linux" target="_blank"/>The Recommended Way To Clean The Package Cache In Arch Linux</a>

## Nvidia Drivers

Make sure to choose the proper installation from the installation menu
> nvidia-inst



## Development Tools (The ones I use Anyway)

### Pyenv (For Python Version Management)


### Postman (API Client)
AppImage from the company works great and allows updating it through the client
[Postman](https://www.postman.com/downloads/)



