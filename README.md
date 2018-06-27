# TADA68 Keyboard Layout

A TADA68 layout designed for use with macOS.

### Layout

Differences from the stock layout:
- Layer 1
  - Swapped `LALT` and `LGUI`
  - Replaced `RALT` with `RGUI`
- Layer 2
  - Removed mouse movement keys
    - `Fn+Left` now maps to `Home`
    - `Fn+Right` now maps to `End`
  - Volume controls are shifted over one key
    - `KC_COMM` maps to `KC_VOLD`
    - `KC_DOT` maps to `KC_VOLU`
    - `KC_SLSH` maps to `KC_MUTE`
  - Custom `MAC_LCK` key
    - Macro for `Ctrl+Alt+F19`
    - Intended for use with an Automator service to start the screensaver
      - https://apple.stackexchange.com/a/256747
    - Macro can be mapped to the default lock shortcut instead if a blank screen/suspend is desired instead: `LCTL(LSFT(KC_POWER))`

### Usage
```
git clone https://github.com/qmk/qmk_firmware.git
cd qmk_firmware/keyboards/tada68/keymaps
git clone https://github.com/stevenmirabito/layout-tada68.git steven
cd ../../../
make tada68:steven:flashbin
```

Flashing instructions can be found in the [QMK TADA68 readme](https://github.com/qmk/qmk_firmware/blob/master/keyboards/tada68/readme.md).
