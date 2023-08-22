# st-0.9.0

This is my patched version of st. The base version is directly from suckless.org.
This belongs to my larbs installation script, but does not directly depend on it.
It is supposed to work in the environment after the larbs-base-installation.

## Patches

The list below shows the currently applied patches to the master branch.

- st-anysize-20220718-baa9357.diff (st leaves no gaps if the height/width doesn't match a multiple of
  character height)
- st-ligatures-scrollback-20230105-0.9.diff (scrollback compatible addition of ligatures)
- st-scrollback-0.8.5.diff (add scrollback functionality)

## Hotkeys

There are various shortcuts and hotkeys used in this version. Included in my build are the following.

| ModKey | Shift | Key             | Function        |
| ------ | ----- | --------------- | --------------- |
| Alt    |       | Break           | Send break      |
| Alt    |       | Print           | Toggle printer  |
| Alt    |       | Print           | Print screen    |
|        | Shift | Insert          | Clipboard paste |
| Alt    |       | c               | Clipboard copy  |
| Alt    |       | v               | Clipboard paste |
| Alt    |       | p               | Selected paste  |
| Alt    |       | NumLock         | Toggle Numlock  |
| Alt    |       | k               | Scroll up       |
| Alt    |       | j               | Scroll down     |
|        |       | MouseScrollUp   | Scroll up       |
|        |       | MouseScrollDown | Scroll down     |
| Alt    | Shift | u               | Zoom in         |
| Alt    | Shift | i               | Zoom out        |

## Installation

To install this package you can run several commands.
If you want to use st with colored emojis make sure to install `libxft-bgra`
(`yay -S libxft-bgra` on arch based systems`).

The most basic way is to clone the repository and then invoke make.

- `git clone https://github.com/tiyn/st-0.9.0`
- `make clean install`
