# Idle Builds — Dinkey Keyboard Series

Open source low-profile wireless split keyboards designed and built by [Idle Builds](https://idlebuilds.com).

<div align="center">
<img src="docs/images/dinkey_32_30_32_key_config_zmk.png" alt="Dinkey Series" width="900"/>
</div>

---

## The Lineup

| Board | Keys | Status |
|---|---|---|
| **Dinkey 34** | 34 | Available |
| **Dinkey 32\|30** | 32 or 30 | Available |
| **Dinkey 36** | 36 | Coming soon |
| **Dinkey 42** | 42 | Coming soon |
| **Dinkey 52** | 52 | Coming soon |

The Dinkey 34 is the entry point — a comfortable, approachable 34-key split that shares its PCB footprint with the 32|30. The 32|30 is the refined endgame: same board, fewer keys, more intentional layout. Both run identical firmware logic, differing only in PCB design and pin assignments.

---

## Dinkey 34

<div align="center">

| ZMK Build | QMK Build |
|:---:|:---:|
| <img src="docs/images/dinkey_34_zmk.png" width="420"/> | <img src="docs/images/dinkey_34_qmk.png" width="420"/> |

</div>

A 34-key column-staggered wireless split. 3 pinky column keys and 2 thumb keys per side. The gateway into the Dinkey lineup.

**[→ ZMK Config](https://github.com/IdleBuilds/zmk-config-dinkey_34)** | **[→ Buy](https://idlebuilds.com)**

---

## Dinkey 32|30

<div align="center">

| 32-key config | 30-key config |
|:---:|:---:|
| <img src="docs/images/dinkey_32_30_32_key_config_zmk.png" width="420"/> | <img src="docs/images/dinkey_32_30_30_key_config_zmk.png" width="420"/> |

| No case | Side profile |
|:---:|:---:|
| <img src="docs/images/dinkey_32_30_32_key_no_case.png" width="420"/> | <img src="docs/images/dinkey_32_30_32_key_side.png" width="420"/> |

| Case | PCB (back) |
|:---:|:---:|
| <img src="docs/images/dinkey_32_30_case.png" width="420"/> | <img src="docs/images/dinkey_32_30_naked.png" width="420"/> |

</div>

The endgame. Modular pinky column accommodates 1 or 2 switches without firmware changes — you choose your key count. Same PCB as the 34, tighter layout.

**[→ ZMK Config](https://github.com/IdleBuilds/zmk-config-dinkey_32_30)** | **[→ Buy](https://idlebuilds.com)**

---

## Firmware

Both the Dinkey 34 and 32|30 support three firmware options:

### ZMK — Wireless (recommended)

ZMK runs on the Nice!Nano v2 and supports Bluetooth 5.0, ZMK Studio for real-time keymap editing, and deep sleep for long battery life.

| Board | Config Repo |
|---|---|
| Dinkey 34 | [zmk-config-dinkey_34](https://github.com/IdleBuilds/zmk-config-dinkey_34) |
| Dinkey 32\|30 | [zmk-config-dinkey_32_30](https://github.com/IdleBuilds/zmk-config-dinkey_32_30) |

Fork the relevant repo, customize your keymap, and GitHub Actions builds your firmware automatically.

### QMK — Wired

QMK runs on the Pro Micro and supports USB-C wired operation. See the [QMK README](qmk/README.md) for compile and flash instructions.

### Vial — Wired with GUI remapping

Vial is a QMK fork that adds a real-time GUI keymap editor over USB. See the [Vial README](vial-qmk/README.md) for setup instructions.

---

## Build Guide

Full step-by-step assembly instructions including soldering, flashing, and troubleshooting are at [idlebuilds.com/build-guide](https://idlebuilds.com/build-guide).

---

## Hardware

| Folder | Contents |
|---|---|
| `kicad/` | PCB design files (KiCad) |
| `qmk/` | QMK keyboard definition files |
| `vial-qmk/` | Vial keyboard definition files |
| `zmk/` | ZMK config files (legacy, see standalone repos above) |
| `docs/` | Images, schematics, reference files |

---

## Specs

| | Dinkey 34 | Dinkey 32\|30 |
|---|---|---|
| **Keys** | 34 | 32 or 30 |
| **Switches** | Kailh Choc V1 | Kailh Choc V1 |
| **Wireless sockets** | Mill-Max Low Profile | Mill-Max Low Profile |
| **Wired sockets** | Kailh Choc hotswap | Kailh Choc hotswap |
| **Wireless controller** | Nice!Nano v2 | Nice!Nano v2 |
| **Wired controller** | Pro Micro | Pro Micro |
| **Wireless display** | Nice!View | Nice!View |
| **Wired display** | 128×32 OLED (optional) | 128×32 OLED (optional) |
| **Battery** | 110mAh LiPo | 110mAh LiPo |
| **Case** | 3D printed TPU | 3D printed TPU |
| **PCB** | JLCPCB | JLCPCB |

---

## Purchasing

Kits and complete builds available at [idlebuilds.com](https://idlebuilds.com).

| Option | Price |
|---|---|
| Kit — Wired | from $80 |
| Kit — Wireless | from $195 |
| Complete Build — Wired | from $175 |
| Complete Build — Wireless | from $275 |

Prices subject to change due to component availability and tariffs.

---

## Contact

Questions, build help, or custom orders — reach out at [clayton@idlebuilds.com](mailto:clayton@idlebuilds.com)

---

## License

Hardware and firmware are open source. See individual folders for license details.

MIT © Idle Builds
