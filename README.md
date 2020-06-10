# ergodox-keymap
This is keymap for ErgodoxZx.

# How to Compile

## clone qmk_firware repository

https://github.com/qmk/qmk_firmware

```
cd qmk_firmware
```

## make directory for customize and copy default keymap

```
cd keyboards/ergodox_ez/keymaps
mkdir customize
cp default/keymap.c customize
```

## compile

```
teensy_loader_cli -mmcu=atmega32u4 -w ergodox_ez_customize.hex
make ergodox_ez:customize
```
