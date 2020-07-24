## Arch Linux after install
My setup after install Arch Linux

Update the system
```shell
sudo pacman -Syu
```
<a id="system"></a>
**System**
```shell
sudo pacman -S cowsay fortune-mod
sudo pacman -S htop
sudo pacman -S glances
sudo pacman -S putty
sudo pacman -S neofetch
sudo pacman -S pv
sudo pacman -S lsof

# yaourt
sudo pacman -Sy yaourt
yaourt -Syu

# pkgfile
sudo pacman -S pkgfile
sudo pkgfile -u
```

**Text Editors**
```
sudo pacman -S code
```

<a id="games"></a>
**Games**
```
sudo apt-get install -y snes9x
sudo apt-get install -y stella
sudo apt-get install -y mame
```

<a id="databases"></a>
**Databases Clients**
```
sudo apt-get install -y mysql-clients
```

<a id="terminal"></a>
**Terminal**
```
sudo apt-get install -y tmux
```

<a id="browser"></a>
**Browsers**
```shell
sudo pacman -S curl wget
sudo pacman -S lynx
```

<a id="video"></a>
**Video**
```shell
sudo pacman -S vlc
```

**Image Editor**
```
sudo pacman -S gimp
```

**Languages**
```
sudo pacman -S jre8-openjdk
```

For Ruby, follow the instructions on [Ruby Verion Manager](https://rvm.io/rvm/install)

**Git**
```
sudo pacman -S tig
```
