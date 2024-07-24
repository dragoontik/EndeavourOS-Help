# EndeavourOS Help! 🆘
 Tips and trick to help you do development in EndeavorOS (An Arch Based Linux Distro) \
**Note:** Most of these tips should work for other Arch based Distributions as well! 😉

# Install EndeavorOS using offline mode
Installing EndeavourOS via offline mode helps minimize system compatibility. You can always change the desktop env later if you don't like KDE. (Who doesn't like KDE? 🤷)

# System Upkeep! 

## KDE Plasma
I had some glitchyness when using wayland with KDE Plasma 6. If you experiance the same 
I recommend switching to plasma that uses X11 for your desktop

Go to the file

> /etc/sddm.conf

and edit the line 

```
[Autologin]
Session=plasma --> Session=plasmax11
```

X11 desktop is older not the newest or fastest but plays nicer with most apps of July 2024. \
I like Manjaro's philosophy here!

## Useful pacman (and yay commands)

### Update system
> sudo pacman -Syu
> yay -Syu

### Checking number of cached packages
> sudo ls /var/cache/pacman/pkg/ | wc -l

### Dealing with Package Cache!

### Checking the disk size of the cached packages
> du -sh /var/cache/pacman/pkg/

### Remove all uninstalled packages from cache
These are useful for saving some disk space!

> sudo pacman -Sc

> yay -Sc 

The **yay** command helps clean up all the packages

Thank you❣️
Senthilkumar Palani (aka SK) \
[The Recommended Way To Clean The Package Cache In Arch Linux](https://ostechnix.com/recommended-way-clean-package-cache-arch-linux)

### Removing Packages
**pacman** - To remove packages from the offical ARCH repo \
**yay** - To remove packages from the AUR repo

> sudo pacman -R <package_name>

> yay -R <package_name>


### Enable Developer Tools
Enable the build tools for Arch Linux Packages.

> sudo pacman -S base-devel


### Install Octipi
Super helpful GUI that helps manages packages on any ARCH Distro

> 

<br>

## Nvidia Drivers
Make sure to choose the proper installation from the installation menu \
**Note!** - This is only applicable to EndeavourOS as of Jul 2024 \
> nvidia-inst

<br>


## Office Software
I will be using a stable version of libreOffice.

> sudo pacman -S 




## Development Tools (The ones I use(d) anyway)

### Pyenv (For Python Version Management 🐍)
> sudo pacman -S pyenv

[Arch Package](https://archlinux.org/packages/extra/any/pyenv/)

### Postman (API Client 📮)
The binary from the company works great and allows updating through the client \
Just add it to your Application Menu.  \
[Postman Website](https://www.postman.com/downloads/)

### Nodejs (Web Developers' Essential 🕸️)
Recommended way of running and using Node.js is to use a version manager!
The [Nodejs.org](https://nodejs.org/) now has a steps to help you get set up on any OS.

[Node.js Website](https://nodejs.org/en/download/package-manager)


### DbGate (Database Client 📚)
Appimage by the developer works great and is stable but you can also get it from the AUR. \
**Why this one?** - DBGate is simple to use and supports the most common SQL and no-SQL databases open source and commercial. 
<br><br>
[DGate Website](https://dbgate.org/)

### .NET (Because Why Not? It's Sharp! 🔪)

#### Option 1: From Official Install Script!
I was surprised how good it worked on EndeavourOS! 🤯

[All .NET Versions](https://dotnet.microsoft.com/en-us/download/dotnet) 

[Install Script Reference Docs](https://learn.microsoft.com/en-us/dotnet/core/tools/dotnet-install-script)

Main thing is to add the path to .bashrc file in /home.

If you want to remove it just run. \
> rm -rf ./home/.dotnet

#### Option 2: From Arch Packages (For latest SDK)
> sudo pacman -S dotnet-sdk

#### Option 3: From AUR Packages 
Advantage of being able to look up the SDK version you want to install 
> yay -S <package_name>

### MariaDB (aka. MySQL) (Database I'm using for my Apps Currently)
You can use pritty much any commercial or open source SQL and noSQL database you want but here.
are some instructions specific to MySQL (Or MariaDB). \
**SideNote** - Postgres is awesome 😎 too. But I started my database journey with MySQL and lanched my apps on 
a production MySQL server so I'm stuck with it. But it's palletable and gets the job done.

> sudo pacman -S mariadb 

Then run:

> mariadb-install-db --user=mysql --basedir=/usr --datadir=/var/lib/mysql

Then you can create users and connect to it with a database client or via the cli.

Thanks so much Geeks for Geeks! 🤓 \
[How to Install and configure MySQL on Arch-based Linux Distributions(Manjaro)](https://www.geeksforgeeks.org/how-to-install-and-configure-mysql-on-arch-based-linux-distributionsmanjaro/)

### 




