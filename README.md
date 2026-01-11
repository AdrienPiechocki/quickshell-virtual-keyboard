# quickshell-virtual-keyboard

I made a virtual keyboard for accessibility purposes.

## Requirements
`quickshell`
`ydotool`

Tested on ArchLinux, with Hyprland (should work in any Wayland environment where quickshell works)

## Features
- A virtual keyboard you can drag around anywhere on your screen (works with multiple screens)
- Modifier keys work as intended (SUPER + B opens my browser for example)
- QWERTY and AZERTY keyboard layouts with the possibility of adding your own.
- Virtual keyboard size settings. Either `compact` or `full` (with or without Fn and numpad keys)

## Installation 
```
git clone https://github.com/AdrienPiechocki/quickshell-virtual-keyboard.git ~/.config/quickshell/virtual-keyboard/
```

## Using the plugin
```
./~/.config/quickshell/virtual-keyboard/virtual-keyboard.sh &
```

**Change the settings by editing this file:** `~/.config/quickshell/virtual-keyboard/settings.json`\
**Replace colors by changing this file:** `~/.config/quickshell/virtual-keyboard/colors.json`

## About keyboard layouts

Pre-installed keyboard layouts are : QWERTY and AZERTY

You can add your own layout by adding a `layoutname.json` in `~/.config/quickshell/virtual-keyboard/layouts/` and configuring it to your liking.\
Then, put the `layoutname` in "layout"'s value in the settings file. (WITHOUT the .json extension)\
Check pre-installed layouts for examples.

## Known issues
- Drag n' drop is messy
- Virtual keyboard always starts at 0x0 global coordinates on your screens (center of the main screen)


## Showcase

This showcase is the Noctalia-Shell plugin I made. Wich is almost the same as this repo.

https://github.com/user-attachments/assets/df076aac-dda9-42ce-9f60-40705195b89f
