#!/bin/bash
sudo pacman -Syu
sudo pacman -S --needed base-devel git
cd /opt
sudo git clone https://aur.archlinux.org/yay-git.git
sudo chown -R $USER:$USER ./yay-git
cd yay-git
makepkg -si && rm -f yay*.tar.zst yay*.gz PKGBUILD
sudo yay -Syu
