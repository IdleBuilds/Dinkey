# Dinkey 34 — QMK

QMK keyboard definition for the Dinkey 34 wired build (Pro Micro / ATmega32U4).

- **Maintainer:** [Idle Builds](https://github.com/IdleBuilds)
- **Hardware:** Dinkey 34 PCB + Pro Micro (ATmega32U4)
- **Hardware availability:** [idlebuilds.com](https://idlebuilds.com)

See [`qmk/README.md`](../README.md) for setup, compile, and flash instructions.

## Compile

```bash
qmk compile -kb idlebuilds/dinkey34 -km default
```

## Flash

```bash
qmk flash -kb idlebuilds/dinkey34 -km default
```

Or open the compiled `.hex` in [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases) and flash manually.

## Bootloader

Enter bootloader in 3 ways:

- **Bootmagic reset:** Hold top-left key while plugging in USB
- **Physical reset:** Double-tap the reset button on the PCB
- **Keycode:** Press `QK_BOOT` if mapped in your keymap

## Handedness

This board uses `#define MASTER_LEFT` in `config.h`. The left half must always be connected via USB. Do not use `EE_HANDS` — the atmel-dfu bootloader does not support EEPROM split flashing.
