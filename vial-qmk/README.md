# Vial Firmware — Dinkey Series

Vial wired firmware for the Dinkey keyboard series by [Idle Builds](https://idlebuilds.com).

Vial is a QMK fork that adds a real-time GUI keymap editor over USB — remap keys without reflashing, directly from the [Vial app](https://get.vial.today).

> For wireless operation, see the ZMK config repos: [Dinkey 34](https://github.com/IdleBuilds/zmk-config-dinkey_34) | [Dinkey 32|30](https://github.com/IdleBuilds/zmk-config-dinkey_32_30)

---

## Status

Vial PRs for the Dinkey 34 and Dinkey 32|30 are pending merge into the main Vial-QMK repository. Once merged, the keyboards will be available natively in Vial without any additional setup.

In the meantime, the keyboard definition files are in this folder and can be used by copying them into your local Vial-QMK installation.

---

## Supported Boards

| Board | Vial Path |
|---|---|
| Dinkey 34 | `keyboards/idlebuilds/dinkey34` |
| Dinkey 32\|30 | `keyboards/idlebuilds/dinkey32_30` |

---

## Prerequisites

1. Clone the Vial QMK fork:
```bash
git clone https://github.com/vial-kb/vial-qmk.git
cd vial-qmk
make git-submodule
```

2. Set up the QMK build environment: [docs.qmk.fm/newbs](https://docs.qmk.fm/newbs)
3. Copy the keyboard folders from this directory into `keyboards/idlebuilds/` in your Vial-QMK installation

---

## Compiling

```bash
# Dinkey 34
make idlebuilds/dinkey34:vial

# Dinkey 32|30
make idlebuilds/dinkey32_30:vial
```

---

## Flashing

### Via QMK Toolbox (recommended)

1. Download [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases)
2. Open your compiled `.hex` file
3. Double-tap reset on your Pro Micro to enter bootloader mode
4. Click **Flash**
5. Repeat for the other half

---

## Using Vial

1. Download the [Vial app](https://get.vial.today) for your OS
2. Connect your keyboard via USB
3. Open Vial — your keyboard will be detected automatically
4. Remap keys, configure layers, and save — changes apply instantly

---

## Build Guide

Full assembly instructions at [idlebuilds.com/build-guide](https://idlebuilds.com/build-guide).

---

## Contact

[clayton@idlebuilds.com](mailto:clayton@idlebuilds.com)

---

## License

GPL-2.0 (Vial/QMK license requirement)
