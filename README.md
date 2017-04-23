## Arch Linux after install
My setup after install Arch Linux

**Update packages**

```
$ sudo pacman -Syy 
```

**Text Editors**
```
$ sudo pacman -S vim
```

**IDE's**
```
$ sudo pacman -S eclipse-jee
$ sudo pacman -S arduino
```

**System**

[Hide user from login list](https://wiki.archlinux.org/index.php/GDM#Hide_user_from_login_list)

```
$ sudo pacman -S net-tools
$ sudo pacman -S htoop
sudo pacman -S lib32-libstdc++5 glibc
```

**Image Editor**
```
$ sudo pacman -S gimp
```

**Browsers**
```
$ sudo pacman -S firefox
$ sudo pacman -S flashplugin
$ sudo pacman -S wget curl
```

```
$ sudo pacman -S tar gzip bzip2 unzip unrar p7zip
```

**Languages**
```
$ sudo pacman -S jre8-openjdk
$ sudo pacman -S elixir
```

For Ruby, follow the instructions on [Ruby Verion Manager](https://rvm.io/rvm/install)

**Git**
```
$ sudo pacman -S git tig
```

**Terminal**
```
$ sudo pacman -S terminator
$ sudo pacman -S zsh
$ sudo pacman -S tmux
```

**Docker**
```
$ sudo pacman -S docker
$ sudo systemctl enable docker
$ sudo gpasswd -a ${USER} docker
$ sudo systemctl start docker
```

**Nodejs**
Using [Node Version Manager](https://github.com/creationix/nvm)
```
$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.1/install.sh | bash

# list the last version
$ nvm ls-remote
$ nvm install [x.x.x]
```

