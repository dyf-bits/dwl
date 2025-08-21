# dwl - dwm for Wayland

This is my build and customizations of [dwl](https://codeberg.org/dwl/dwl), the wayland tiling window manager.

## Patches Applied:

- [alwayscenter](https://codeberg.org/dwl/dwl-patches/src/branch/main/patches/alwayscenter): start floating windows at the center of screen
- [attachbottom](https://codeberg.org/dwl/dwl-patches/src/branch/main/patches/attachbottom): attach new windows to the bottom of stack
- [follow](https://codeberg.org/dwl/dwl-patches/src/branch/main/patches/follow): transition to tag moved by window
- [ipc](https://codeberg.org/dwl/dwl-patches/src/branch/main/patches/ipc): provides ipc for clients to get and set dwl state.
- [vanitygaps](https://codeberg.org/dwl/dwl-patches/src/branch/main/patches/vanitygaps): adds gaps between client windows

## Installation

Clone the repository and install with make:

```sudo make clean install```

*Dependencies:*
- libinput
- wayland
- wlroots
- xkbcommon
- wayland-protocols
- pkg-config

## Optional Packages

- [btrbar](https://github.com/dyf-bits/btrbar) or any bar of your choosing 
- Fonts: ```Ubuntu Nerd Font``` and/or ```BitstromWera Nerd Font Mono``` 

## Notes
- default Mod key is ```super```
- do your customizations in ```config.def.h``` because ```make clean``` deletes config.h
