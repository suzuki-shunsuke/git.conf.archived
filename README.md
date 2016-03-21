# git.conf

hubが導入済みとする

```
$ git clone suzuki-shunsuke/git.conf ~/gh/ss/git.conf
$ ln -s ~/gh/ss/git.conf/.gitconfig ~/.gitconfig
```


## gnome-keyringについて

http://stackoverflow.com/questions/13385690/how-to-use-git-with-gnome-keyring-integration/13390889#13390889
https://github.com/shugo/git-credential-gnomekeyring/issues/2
https://wiki.archlinuxjp.org/index.php/GNOME_Keyring

```
$ pacman -S libgnome-keyring
$ cd /usr/share/git/credential/gnome-keyring
$ make
$ git config --global credential.helper /usr/share/git/credential/gnome-keyring/git-credential-gnome-keyring
```
