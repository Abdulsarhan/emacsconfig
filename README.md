# About
This is an emacs config that uses the elpaca package manager and evil mode. So, if you like broken pinkys this isn't for you. 
This config is a slightly modified fork of DT's config. 
With the only major difference being is that it uses nerd-icons instead of all-the-icons. I did this so that I could use the symbols included with nerd fonts with my emacs config. 

# Dependencies
You need to have a nerd font for the icons to render correctly. 
If you're using a good linux distro, you can just type "sudo pacman -Ss nerd fonts library", and you will get a list of all the nerd fonts that work with this config and you could install them just by running "sudo pacman -S * *FONT_NAME* *". On inferior distros, you could do the same thing, but I don't know the commands on those distros; I don't use them. You can also install the fonts manually from [Nerd Fonts](https://www.nerdfonts.com), but I find that it's just easier to use the package manager for this. 

## Keybindings
The keybindings should be fairly easy to understand. Just read the config file. You're probably not going to use most of the bindings, I don't either. I copied a lot of them from dt's config and I am just too lazy to remove them right now.
some of the keybindings are commented out becuase I don't use them anymore, but they would work just fine if you remove the comments. 

## Features
This config has a lot of features.
If you just want a basic text editor, this config is not for you. 
Even for those of you who like having a few extra features on top of your basic emacs experience, you still might want to disable a LOT of features. 
Just remove the packages that you don't like by removing the "use-package" statement for the package(s) that you want to remove and remove their associated keybindings under general keybinidings. 
some of these features include: 
- An RSS reader.
- A terminal.
- An application launcher.
- A dashboard that shows you your recent files, projects and bookmarks.
- general, for general keybindings.
- evil mode, for vim keybindings.
and many more that I just can't remember.

Happy editing!
