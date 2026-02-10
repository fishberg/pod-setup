# pod-setup

```bash
set -ex    # exit on error + verbose
sudo apt purge -y 'nvidia*'
sudo apt autoremove -y
sudo apt upgrade -y
sudo apt update -y
sudo apt install -y git
git clone https://github.com/fishberg/dotfiles ~/.dotfiles
cd ~/.dotfiles/install
./01_ubuntu-24.04_essentials-install.bash
./02_bashrc-install.bash
./10_ssh-server.bash
reboot
```

