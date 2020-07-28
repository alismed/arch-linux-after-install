## Arch Linux after install
My setup after install Arch Linux

- [IDE's](#ides)
- [System](#system)
- [Security](#security)
- [Git](#git)
- [Games](#games)
- [Databases](#databases)
- [Languages](#languages)
- [Terminal](#terminal)
- [Browsers](#browser)
- [Video](#video)
- [Docker](#docker)
- [Javascript packages](#jspackage)
- [Comumunicators](#communicators)
- [CLI's](#cli)


<a id="system"></a>
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
sudo pacman -S netstat-nat
sudo pacman -S dstat
```

<a id="security"></a>
**Security**
```shell
sudo pacman -S rkhunter
rkhunter --propupd
sudo rkhunter --check
```

<a id="packages"></a>
**Packages Management**
```shell
#snapd
git clone https://aur.archlinux.org/snapd.git
cd snapd
makepkg -si

sudo systemctl enable --now snapd.socket
sudo ln -s /var/lib/snapd/snap /snap


# yaourt
sudo pacman -Sy yaourt
yaourt -Syu


# pkgfile
sudo pacman -S pkgfile
sudo pkgfile -u
```

**Login**

Hide user from login list

Edit /var/lib/AccountsService/users/**[username]**. Change the variable _SystemAccount_.
```
SystemAccount=true
```
<a id="git"></a>
**Git**
```
sudo pacman -S git tig

ssh key
ssh-keygen -t rsa -b 4096 -C "<your_email@example.com>"
cat ~/.ssh/id_rsa.pub
```

**Text Editors**
```
sudo pacman -S code
sudo snap install code --classic
pacaur -Sy sublime-text-dev
```

<a id="ides"></a>
**IDE's**
```
sudo pacman -S eclipse
sudo pacman -S arduino
```

<a id="games"></a>
**Games**
```shell
sudo pacman -S snes9x
sudo pacman -S stella
sudo pacman -S mame
```

<a id="databases"></a>
**Databases Clients**
```
sudo pacman -S mysql-clients
```

<a id="terminal"></a>
**Terminal**
```
sudo pacman -S tmux
```

<a id="browser"></a>
**Browsers**
```shell
sudo pacman -S curl wget
sudo pacman -S lynx
```

<a id="communicators"></a>
**Communicators**
```shell
sudo snap install skype --classic 
sudo snap install slack --classic 
sudo snap install zoom --classic 
```

```shell
sudo pacman -S dropbox 
```

<a id="video"></a>
**Video**
```shell
sudo pacman -S vlc
```

**Image Editor**
```
sudo pacman -S gimp
sudo pacman -S imagemagick
```

```
sudo pacman -S tar gzip bzip2 unzip unrar p7zip
```

**Languages**
```
sudo pacman -S jre8-openjdk
sudo pacman -S maven
```

For Ruby, follow the instructions on [Ruby Verion Manager](https://rvm.io/rvm/install)

**Git**
```
sudo pacman -S tig
```

<a id="docker"></a>
**Docker**
```shell
sudo pacman -S docker
sudo gpasswd -a ${USER} docker
sudo systemctl enable docker
sudo systemctl start docker
```

**Docker Compose**
```shell
sudo curl -L "https://github.com/docker/compose/releases/download/1.26.2/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose

sudo chmod +x /usr/local/bin/docker-compose
```

<a id="jspackage"></a>
**Yarn**
```shell
pacman -S yarn
```

**Node**

Using _Node Version Manager_
```shell
curl -o- https://raw.githubusercontent.com/nvm-sh/nvm/v0.35.3/install.sh | bash
```

Execute  `source ~/<profile-file>`

List the versions
```
nvm ls-remote
```

Choice the version to install
```
nvm install [x.x.x]
```

<a id="cli"></a>
**CLI's**
```shell
npm install -g heroku
npm install -g sfdx-cli
```

