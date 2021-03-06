## Fork of st - simple terminal

st is a simple terminal emulator for X which sucks less.

## Requirements

In order to build st you need the Xlib header files.

## Installation

Edit config.mk to match your local setup (st is installed into
the `/usr/local` namespace by default).

Afterwards enter the following command to build and install st (if
necessary as root):

```bash
make clean install
```

## Running st

If you did not install st with make clean install, you must compile
the st terminfo entry with the following command:

```bash
tic -sx st.info
```

See the man page for additional details.

## Credits

Based on Aurélien APTEL `aurelien dot aptel at gmail dot com` bt source code.

## Patches

- [vertcenter](https://st.suckless.org/patches/vertcenter/)
- [scrollback + mousescrolling with shift](https://st.suckless.org/patches/scrollback/)
- [externalpipe](https://st.suckless.org/patches/externalpipe/) + [openurl, copyurl, copyoutput by Luke Smith](https://github.com/lukesmithxyz/st)
- [ligature support, compatibility with scrollback](https://st.suckless.org/patches/ligatures/)
- [Xresources support](https://st.suckless.org/patches/xresources/)

## st Terminal Hotkey Configuration

| Keybinding                     | Effect                            |
| ------------------------------ | --------------------------------- |
| Control + Shift + Page Up      | Zoom in                           |
| Control + Shift + Page Down    | Zoom out                          |
| Control + Shift + Home         | Reset zoom                        |
| ------------------------------ | --------------------------------- |
| Control + Shift + v            | Paste primary clipboard content   |
| Control + Shift + y            | Paste X clipboard content         |
| ------------------------------ | --------------------------------- |
| Shift + Page Up                | Scroll up                         |
| Shift + Page Down              | Scroll down                       |
| ------------------------------ | --------------------------------- |
| Super + l                      | Select URL to open                |
| Super + y                      | Select URL to copy                |
| Super + o                      | Select output to copy             |
