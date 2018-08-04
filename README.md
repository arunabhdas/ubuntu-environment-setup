# ubuntu-environment-setup

## 1) Install vim

==> sudo apt -y update && sudo apt -y install vim
## 2) Copy .vimrc to $HOME

==> cp dotfiles/vimrc.txt $HOME

## 3) Copy .Xmodmap to $HOME
Please note that this steps is only necessary for remapping Super to Ctrl
==> cp dotfiles/Xmodmap.txt $HOME/.Xmodmap

## 4) Ensure ~/.Xmodmap is sourced in .bashrc as follows

==> echo "xmodmap ~/.Xmodmap" >> ~/.bashrc

## 5) Install Java 8
http://www.webupd8.org/2014/03/how-to-install-oracle-java-8-in-debian.html


## 6) Install Android Studio as described here :
https://developer.android.com/studio/install.html


## 7) Install VSCode as follows :

Download VSCode from 

https://code.visualstudio.com/docs?dv=linux64

Extract it: unzip VSCode-linux-x64.zip -d ~/vscode/VSCode-linux-x64

Run the code executable to open Visual Studio Code

(Optional) Create a symbolic link to conveniently run code from the terminal:
sudo ln -s ~/vscode/VSCode-linux-x64/code /usr/local/bin/code

## 8) Install python2

==> sudo apt install python-minimal

==> python --version

## 9) Install pip

==> sudo apt update

==> sudo apt install python-pip

==> pip --version
