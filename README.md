# colemak-win

Adds Colemak-DH to the available keyboard layouts under Windows. The layout is installed
at the OS-level and should work in all applications and even before signing in. No 3rd
party apps are required to use the layout.

## Default layout

The precompiled binaries install Colemak-DH for standard ANSI keyboards using a en-us
language profile. Alternative language profiles and ISO variants can be obtained with a
minor modification to the source file (see the "building from source" section below).

![](Colemak.jpg)

## Installation

To install, download the binaries folder and run `setup.exe`. This will add Colemak to
the list of available keyboards. It can be selected from the language bar (`Ctrl +
Shift`) or set as system default in the language settings.

## Building from source

To build the binaries from source, download the source file and use Microsoft Keyboard
Layout Creator (MSKLC) to build the binaries. 

*Note:* While some customization can be done in MSKLC itself, it is recommended to
directly edit the source file instead. Editing keys in MSKLC will only remap them to a
different output, but won't change the underlying key event, creating inconsistencies in
combination with modifiers.

## Why not use AHK/kmonad?

Because installing the keyboard layout at the OS-level is more robust. I wanted a
solution that works across applications and also works at the login screen. (I still use
AHK and kmonad to implement additional goodies on top of this configuration such as
[home row mods](https://precondition.github.io/home-row-mods), `backspace` on right alt
and `esc`/`ctrl` on capslock.
