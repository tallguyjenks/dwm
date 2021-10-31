# Bryan's build of dwm

## Installation

---

```ba   sh
git clone https://github.com/tallguyjenks/dwm
cd dwm
sudo make install
```

---

## Dependencies

---

This build of dwm does not block color emoji in the status/info bar, so you must install [libxft-bgra][13] from the AUR, which fixes a libxft color emoji rendering problem, otherwise dwm will crash upon trying to render one. Hopefully this fix will be in all libxft soon enough.

---

## Patches and features

---

| Link             | Description                                                                                                                        |
| ---------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| [dwmblocks][0]   | Clickable statusbar with my build of **dwmblocks**.                                                                                |
| [xResources][1]  | Reads **xresources** colors/variables (i.e. works with `pywal`, etc.).                                                             |
| [Scratchpad][2]  | **scratchpad**: Accessible with `mod+shift+enter`.                                                                                 |
|                  | New **layouts**: [bstack][3], [fibonacci][4], [deck][5], [centered master][6] and more. All bound to keys `super+(shift+)t/y/u/i`. |
| [Full Screen][7] | True **fullscreen** (`super+f`) and prevents focus shifting.                                                                       |
| [Sticky][8]      | Windows can be made **sticky** (`super+s`).                                                                                        |
| [Stacker][9]     | **stacker**: Move windows up the stack manually (`super-K/J`).                                                                     |
| [Shiftview][10]  | **shiftview**: Cycle through tags (`super+g/;`).                                                                                   |
| [Vanitygaps][11] | **vanitygaps**: Gaps allowed across all layouts.                                                                                   |
| [Swallow][12]    | **swallow** patch: if a program run from a terminal would make it inoperable, it temporarily takes its place to save space.        |

---

## Keybindings

---

Check out [config.h](config.h).

[0]: https://github.com/tallguyjenks/dwmblocks
[1]: https://dwm.suckless.org/patches/xresources/
[2]: https://dwm.suckless.org/patches/scratchpad/
[3]: https://dwm.suckless.org/patches/bottomstack/
[4]: https://dwm.suckless.org/patches/fibonacci/
[5]: https://dwm.suckless.org/patches/deck/
[6]: https://dwm.suckless.org/patches/centeredmaster/
[7]: https://dwm.suckless.org/patches/fullscreen/
[8]: https://dwm.suckless.org/patches/sticky/
[9]: https://dwm.suckless.org/patches/stacker/
[10]: shiftview.c
[11]: https://dwm.suckless.org/patches/vanitygaps/
[12]: https://dwm.suckless.org/patches/dynamicswallow/
[13]: https://aur.archlinux.org/packages/libxft-bgra/
