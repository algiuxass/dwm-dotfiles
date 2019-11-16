# dwm-dotfiles
My DWM tiling window manager dotfiles

## Requirements
- Some MATE desktop environment packages (mate-terminal).

## Optional
- Some knowledge about programming with C, if you want to customize DWM.
- Running this in Arch.

## Add DWM desktop entry

Create a new file to here: /usr/share/xsessions/dwm.desktop

Usage: `sudo nano /usr/share/xsessions/dwm.desktop`
```
[Desktop Entry]
Encoding=UTF-8
Name=dwm
Comment=Dynamic Window Manager
Exec=~/.config/dwm/dwm/dwm
Type=Application
```
