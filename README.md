## Arch Linux after install
My setup after install Arch Linux

**Update packages**

```
$ sudo pacman -Syy 
```

**Text Editors**
```
$ sudo pacman -S vim
$ pacaur -Sy sublime-text-dev
```

**IDE's**
```
$ sudo pacman -S eclipse-jee
$ sudo pacman -S arduino
```

**Database**
```
$ pacaur -Sy mysql-clients
```

**Fonts**
```
$ sudo pacman -Sy ttf-dejavu

# Power Line
$ git clone https://github.com/powerline/fonts.git
$ cd fonts
$ ./install.sh
$ cd ..
$ rm -rf fonts
```

**System**

Hide user from login list
 - [Gnome](https://wiki.archlinux.org/index.php/GDM#Hide_user_from_login_list)

```
$ sudo pacman -S net-tools
$ sudo pacman -S htoop
$ sudo pacman -S lib32-libstdc++5 glibc
```

**Wifi**
```
$ sudo pacman -S rfkill
$ sudo pacman -S crda
$ sudo pacman -S wireless-regdb
```
Many laptops have a hardware button (or switch) to turn off wireless card, however, the card can also be blocked by kernel. This can be handled by rfkill. Use rfkill to show the current status:

```
$ rfkill list

# If the card is hard-blocked, use the hardware button (switch) to unblock it. If the card is not hard-blocked but soft-blocked, use the following command:
$ rfkill unblock wifi
```

**Image Editor**
```
$ sudo pacman -S gimp
$ sudo pacman -S imagemagick
```

**Browsers**
```
$ sudo pacman -S chromiun
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
Oh my ZSH
```
$ sh -c "$(wget https://raw.github.com/robbyrussell/oh-my-zsh/master/tools/install.sh -O -)"
```

**Docker**
```
$ sudo pacman -S docker
$ sudo gpasswd -a ${USER} docker
$ sudo systemctl enable docker
$ sudo systemctl start docker
```

**Nodejs**
Using [Node Version Manager](https://github.com/creationix/nvm)
```
$ curl -o- https://raw.githubusercontent.com/creationix/nvm/v0.33.1/install.sh | bash

# list the last version
$ nvm ls-remote
# choice the version
$ nvm install [x.x.x]

# The script clones the nvm repository to ~/.nvm and adds the source line to your profile (~/.bash_profile, ~/.zshrc, ~/.profile, or ~/.bashrc).

# This loads nvm
export NVM_DIR="$HOME/.nvm"
[ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh" 
```

