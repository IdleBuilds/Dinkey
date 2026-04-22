# QMK Firmware — Dinkey Series

QMK wired firmware for the Dinkey keyboard series by [Idle Builds](https://idlebuilds.com).

> For wireless operation, see the ZMK config repos: [Dinkey 34](https://github.com/IdleBuilds/zmk-config-dinkey_34) | [Dinkey 32|30](https://github.com/IdleBuilds/zmk-config-dinkey_32_30)

---

## Status

QMK PRs for the Dinkey 34 and Dinkey 32|30 are pending merge into the main QMK firmware repository. Once merged, the keyboards will be available natively in QMK without any additional setup.

In the meantime, the keyboard definition files are in this folder and can be used by copying them into your local QMK installation.

---

## Supported Boards

| Board | QMK Path |
|---|---|
| Dinkey 34 | `keyboards/idlebuilds/dinkey34` |
| Dinkey 32\|30 | `keyboards/idlebuilds/dinkey32_30` |

---

## Prerequisites

1. Set up the QMK build environment: [docs.qmk.fm/newbs](https://docs.qmk.fm/newbs)
2. Clone QMK firmware:
```bash
git clone https://github.com/qmk/qmk_firmware.git
cd qmk_firmware
qmk setup
```
3. Copy the keyboard folders from this directory into `keyboards/idlebuilds/` in your QMK installation

---

## Compiling

```bash
# Dinkey 34
qmk compile -kb idlebuilds/dinkey34 -km default

# Dinkey 32|30
qmk compile -kb idlebuilds/dinkey32_30 -km default
```

---

## Flashing

### Via QMK Toolbox (recommended)

1. Download [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases)
2. Open your compiled `.hex` file
3. Double-tap reset on your Pro Micro to enter bootloader mode
4. Click **Flash**
5. Repeat for the other half

### Via command line

```bash
qmk flash -kb idlebuilds/dinkey34 -km default
qmk flash -kb idlebuilds/dinkey32_30 -km default
```

> Flash both halves — left first, then right.

---

## Handedness

Both boards use `#define MASTER_LEFT` in `config.h`. The left half must always be connected via USB.

---

## Customizing Your Keymap

1. Navigate to `keyboards/idlebuilds/dinkey34/keymaps/default/` (or `dinkey32_30`)
2. Edit `keymap.c`
3. Recompile and flash

Refer to the [QMK documentation](https://docs.qmk.fm/) for keymap syntax and available features.

---

## Build Guide

Full assembly instructions at [idlebuilds.com/build-guide](https://idlebuilds.com/build-guide).

---

## Contact

[clayton@idlebuilds.com](mailto:clayton@idlebuilds.com)

---

## License

GPL-2.0 (required for QMK contributions)
