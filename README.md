# About
This is an emacs config that uses the elpaca package manager and evil mode. So, if you like broken pinkies this isn't for you.

I know this README is lengthy, but if you don't read it, this config might not work. 

This config is a slightly modified fork of DT's config, 
with the only major differences being is that it uses nerd-icons instead of all-the-icons. I did this so that I could use the symbols included with nerd fonts with my emacs config. And also it has avy-go-to char and evil-mc for added productivity benefits. 

It also has evil-surround, which is the same as vim-surround and I also fixed the CTRL + U vim keybinding which doesn't work right in the original config made by DT for some reason. 

All the configuration is done inside of the config.org file, with the exception of three scripts that are required by the config.org file. They can be found in the scripts folder. The early-init.el and init.el files are only used to start the config.org file. 

This config is quite heavy, around 65 packages. The load times are not the best because of this. But this isn't a problem if you start emacs as a daemon, which I will teach you how to do during the installation process.

# Dependencies
## Emacs
You can install emacs using your favourite package manager.

Arch linux:
```
sudo pacman -S emacs
```
## Cmake
You can get cmake from your package manager.
cmake is required to compile vterm (the terminal emulator inside emacs)

Arch linux:
```
sudo pacman -S cmake
```
## Nerd Fonts
You also need to have a nerd font for the icons to render correctly.


You can also install the fonts manually from [Nerd Fonts](https://www.nerdfonts.com) but I find that it's just easier to use the package manager for this. 

# Installation
Clone this repo into your ~/.config directory, rename it to emacs and then run emacs.
```
cd ~/.config
git clone https://github.com/abdulsarhan/emacsconfig
mv emacsconfig emacs
```

If you want faster load times, I suggest running emacs as a daemon. This is also know as "starting an emacs server". You could do this manually by typing the following into your terminal or an application launcher: 
```
emacs --daemon
```
After that, you can connect to this local daemon/server by running emacsclient, which is a separate binary from emacs that is included in the emacs package when you installed emacs.

If you want emacs to automatically start as a daemon when you log in, add the following to your bashrc:
```
emacs --daemon
```
If that doesn't work, there are other ways to start emacs as a daemon automatically.

https://www.emacswiki.org/emacs/EmacsAsDaemon

# Keybindings
The keybindings are under the general-keybindings section of the config.org file. 

You're probably not going to use most of the keybindings, I don't either. I copied a lot of them from dt's config and I am just too lazy to remove them right now.

Some of the keybindings are commented out becuase I don't use them anymore, but they would work just fine if you remove the comments. 

# Features
This config has a lot of features.

If you just want a basic text editor, this config is not for you. 

Even for those of you who like having a few extra features on top of your basic emacs experience, you still might want to disable a LOT of features. 

Just remove the packages that you don't like by removing the "use-package" statement for the package(s) that you want to remove and remove their associated keybindings under general keybindings. 

Some of these features include: 
- An RSS reader.
- Two terminals (vterm and eshell)
- An application launcher.
- A dashboard that shows you your recent files, projects and bookmarks.
- General, for general keybindings.
- Evil mode, for vim keybindings.
- Some Evil mode related plugins for added productivity.
- Avy-go-to char, which is like [nvim.leap](https://github.com/ggandor/leap.nvim). Easily the best way to move your cursor exactly where you want on the screen.
- Evil-mc. Multiple-cursors plugin that plays well with Evil mode.
- A few org mode pluggins which make org mode better.
  
And a few more that I either can't remember, or I will be adding in the future. This config is a work in progress for me, so I will be changing it bit by bit to suit my needs better. You will be informed of all the changes. 

Happy editing!
