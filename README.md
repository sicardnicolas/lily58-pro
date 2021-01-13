Lily58 Pro keymap
=================

## Description

This is a keymap for the Lily58 Pro to use with QMK firmware.

Left screen displays only the layer currently used.

Right screen displays the standard Lily58 logo.

## Layout

Standard layer:
```
,-----------------------------------------.                    ,-----------------------------------------.
| ESC  |   1  |   2  |   3  |   4  |   5  |                    |   6  |   7  |   8  |   9  |   0  |  -   |
|------+------+------+------+------+------|                    |------+------+------+------+------+------|
| Tab  |   Q  |   W  |   E  |   R  |   T  |                    |   Y  |   U  |   I  |   O  |   P  |  =   |
|------+------+------+------+------+------|                    |------+------+------+------+------+------|
|LCTRL |   A  |   S  |   D  |   F  |   G  |-------.    ,-------|   H  |   J  |   K  |   L  |   ;  |  '   |
|------+------+------+------+------+------|   [   |    |    ]  |------+------+------+------+------+------|
|LShift|   Z  |   X  |   C  |   V  |   B  |-------|    |-------|   N  |   M  |   ,  |   .  |   /  |  \   |
`-----------------------------------------/       /     \      \-----------------------------------------'
                  | LAlt | LGUI |LOWER | /Space  /       \Enter \  |LOWER |BackSP| RGUI |
                  |      |      |      |/       /         \      \ |      |      |      |
                  `----------------------------'           '------''--------------------'

```

Lower layer:
```
,-----------------------------------------.                    ,-----------------------------------------.
|  `   |  F1  |  F2  |  F3  |  F4  |  F5  |                    |  F6  |  F7  |  F8  |  F9  |  F10 |  F11 |
|------+------+------+------+------+------|                    |------+------+------+------+------+------|
| Tab  |      |  Up  |      |      |      |                    |      |      |      |  Up  |      | F12  |
|------+------+------+------+------+------|                    |------+------+------+------+------+------|
|LCTRL | Left | Down |Right |      | PgUp |-------.    ,-------| PgDn |      | Left | Down |Right |      |
|------+------+------+------+------+------| Home  |    |  End  |------+------+------+------+------+------|
|LShift| Prev | Play | Next | Vol- | Vol+ |-------|    |-------|      |      |      |      |      |      |
`-----------------------------------------/       /     \      \-----------------------------------------'
                  | LAlt | LGUI |      | /Space  /       \Enter \  |      |BackSP| RGUI |
                  |      |      |      |/       /         \      \ |      |      |      |
                  `----------------------------'           '------''--------------------'

```

## How to use

Copy the content of this folder to your `qmk_firmware` directory inside `keyboards/lily58/keymaps/your_keymap_name`.

Then, flash your keyboard (one part at a time), here for a elite-c controller (note the `-bl dfu`):
```
sudo qmk flash -kb lily58 -km your_keymap_name -bl dfu
```
