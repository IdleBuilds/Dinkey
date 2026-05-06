# Dinkey

Open-source split keyboard series by [Idle Builds](https://idlebuilds.com). Column-staggered, low-profile, wireless-first. Built around Kailh Choc V1 switches and the nice!nano v2.

---

<p align="center">
  <img src="docs/images/dinkey_3230_30key.png" width="49%">
  <img src="docs/images/dinkey_3230_32key.png" width="49%">
</p>
<p align="center">
  <em>Dinkey 32|30 — 30-key config (left) and 32-key config (right). Same PCB, same firmware.</em>
</p>
<p align="center">
  <img src="docs/images/dinkey_34_zmk.png" width="80%">
</p>
<p align="center">
  <em>Dinkey 34 — 34-key wireless split. 3×5 column stagger + 2 thumb keys per side.</em>
</p>

---

## Boards

| Board | Keys | Layout |
|---|---|---|
| Dinkey 34 | 34 | 3×5 column stagger + 2 thumb keys per side |
| Dinkey 32\|30 | 30–32 | 3×5 column stagger + 2 thumb keys + modular 4th pinky column |
| Dinkey 36 | 36 | 3×6 column stagger + 2 thumb keys per side *(not currently listed)* |
| Dinkey 42 | 42 | 3×6 column stagger + 3 thumb keys per side *(not currently listed)* |
| Dinkey 52 | 52 | 4×6 column stagger + 4 thumb keys per side *(not currently listed)* |

### Dinkey 32|30 — Modular Pinky Column

The 32|30 PCB has a 4th pinky column wired to accept one or two switches. Populate both for 32 keys, one for 30 — no firmware changes, no reflash. The firmware matrix handles both configurations identically.

---

## Firmware

| Board | ZMK (wireless) | QMK (wired) | Vial (wired) |
|---|---|---|---|
| Dinkey 34 | [zmk-config-dinkey_34](https://github.com/IdleBuilds/zmk-config-dinkey_34) | [`qmk/dinkey34/`](./qmk/dinkey34) | [`vial-qmk/dinkey34/`](./vial-qmk/dinkey34) |
| Dinkey 32\|30 | [zmk-config-dinkey_32_30](https://github.com/IdleBuilds/zmk-config-dinkey_32_30) | [`qmk/dinkey32_30/`](./qmk/dinkey32_30) | [`vial-qmk/dinkey32_30/`](./vial-qmk/dinkey32_30) |
| Dinkey 36–52 | [`zmk/`](./zmk) | [`qmk/`](./qmk) | [`vial-qmk/`](./vial-qmk) *(not currently listed)* |

The 34 and 32|30 have separate firmware — different PCB routing produces different physical layout definitions for ZMK Studio. The repos are not interchangeable.

ZMK config repos (34 and 32|30) include GitHub Actions CI — fork and push to build firmware without a local toolchain. See each repo's README for flashing instructions.

**QMK PR status:** Pending upstream merge. Until merged, copy the board folder from `qmk/` into your local QMK installation under `keyboards/idlebuilds/`. Full instructions: [`qmk/README.md`](./qmk/README.md).

**Vial PR status:** Pending upstream merge. Same process from `vial-qmk/`. Full instructions: [`vial-qmk/README.md`](./vial-qmk/README.md).

---

## Schematics

Schematic reference images are in [`kicad/`](./kicad). KiCad source files are not included in this repo.

| Board | Schematic |
|---|---|
| Dinkey 34 | [`kicad/dinkey_34/schematic.png`](./kicad/dinkey_34/schematic.png) |
| Dinkey 36 | [`kicad/dinkey_36/schematic.png`](./kicad/dinkey_36/schematic.png) |
| Dinkey 42 | [`kicad/dinkey_42/schematic.png`](./kicad/dinkey_42/schematic.png) |
| Dinkey 52 | [`kicad/dinkey_52/schematic.png`](./kicad/dinkey_52/schematic.png) |

---

## Hardware Specs

|  | Dinkey 34 | Dinkey 32\|30 |
|---|---|---|
| Keys | 34 | 30 or 32 |
| MCU (wireless) | nice!nano v2 (nRF52840) | nice!nano v2 (nRF52840) |
| MCU (wired) | Pro Micro (ATmega32U4) | Pro Micro (ATmega32U4) |
| MCU socket | Mill-Max low profile (hotswap) | Mill-Max low profile (hotswap) |
| Switches | Kailh Choc V1 (hotswap) | Kailh Choc V1 (hotswap) |
| Display (wireless) | nice!view (hotswap) | nice!view (hotswap) |
| Display (wired) | 128×32 OLED (optional) | 128×32 OLED (optional) |
| Battery | 110mAh LiPo | 110mAh LiPo |
| Split (wireless) | BLE, no TRRS | BLE, no TRRS |
| Split (wired) | TRRS | TRRS |
| Handedness | `MASTER_LEFT` | `MASTER_LEFT` |

---

## Repo Structure

```
kicad/
  dinkey_34/          ← Schematic PNG
  dinkey_36/          ← Schematic PNG
  dinkey_42/          ← Schematic PNG
  dinkey_52/          ← Schematic PNG
qmk/
  README.md           ← Setup and flashing instructions
  dinkey34/           ← QMK keyboard definition
  dinkey32_30/        ← QMK keyboard definition
  dinkey36/           ← (not currently listed)
  dinkey42/           ← (not currently listed)
  dinkey52/           ← (not currently listed)
vial-qmk/
  README.md           ← Setup and flashing instructions
  dinkey34/           ← Vial keyboard definition
  dinkey32_30/        ← Vial keyboard definition
  dinkey36/           ← (not currently listed)
  dinkey42/           ← (not currently listed)
  dinkey52/           ← (not currently listed)
zmk/
  zmk-config-dinkey_34/     ← ZMK source (see standalone repo above)
  zmk-config-dinkey_32_30/  ← ZMK source (see standalone repo above)
  zmk-config-dinkey_36/     ← (not currently listed)
  zmk-config-dinkey_42/     ← (not currently listed)
  zmk-config-dinkey_52/     ← (not currently listed)
docs/images/          ← Board photos
assets/               ← ZMK Studio screenshots
```

---

## Build Guide

Full assembly instructions at [idlebuilds.com/build-guide](https://idlebuilds.com/build-guide).

---

## Links

- [idlebuilds.com](https://idlebuilds.com)
- [zmk-config-dinkey_34](https://github.com/IdleBuilds/zmk-config-dinkey_34)
- [zmk-config-dinkey_32_30](https://github.com/IdleBuilds/zmk-config-dinkey_32_30)
- [ZMK docs](https://zmk.dev/docs) · [ZMK Studio](https://studio.zmk.dev)
- [QMK docs](https://docs.qmk.fm) · [QMK Toolbox](https://github.com/qmk/qmk_toolbox/releases)
- [Vial](https://get.vial.today)

---

## License

Firmware: GPL-2.0
