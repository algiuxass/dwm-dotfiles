# dwm-dotfiles
My DWM tiling window manager dotfiles


## Requirements
- Some MATE desktop environment packages (mate-terminal).


## Optional
- Some knowledge about programming with C, if you want to customize DWM.
- Running this in Arch/Manjaro.


## Add dwm desktop entry
Create a new file to here: /usr/share/xsessions/dwm.desktop

Usage: `sudo nano /usr/share/xsessions/dwm.desktop`

```
[Desktop Entry]
Encoding=UTF-8
Name=dwm
Comment=Dynamic Window Manager
Exec=~/.config/dwm/login
Type=Application
```


## Upload this git content to ~/.config/dwm
It shouldn't be that hard


## Go to ~/.config/dwm/main and compile it
Write this command: `sudo make install`

This should compile dwm so you could run it.

## Install required stuff
- dmenu

## Install optional stuff
You have to change ~/.config/dwm/main/config.h and ~/.config/dwm/login to not use these programs.

Otherwise you will have problems.
- unclutter (will hide mouse when you don't use it)
- xorg-xsetroot (can set background color and image but only works when compton is not running)
- hsetroot (same as xsetroot but only works when compton is running)
- xinput (settings for my laptop trackpad, you can customize it for yours)
- upower (for getting battery levels)
- discord (chat for gamers, it will autostart on 3rd tab)
- firefox (browser)
- xinput (used for my laptop trackpad fix)
- mate-settings-daemon (it's in ~/.config/dwm/login, disable it if you don't want MATE theme)
- polkit-gnome-authentication-agent (popups for auth, programs which need root privileges will have some problems if this doesn't exist)
- mate-terminal (it's the terminal I've set in config.h)
- mate (for those three above)

`yay -S unclutter xorg-xsetroot hsetroot xinput upower discord firefox mate mate-terminal`
