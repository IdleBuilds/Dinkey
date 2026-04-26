# Dinkey

A series of split ergonomic keyboards designed and built out of a deep appreciation for efficiency. This started as a personal project to build a minimalistic and travel friendly keyboard with hot swappable micro-controllers, oleds, and switches. The PCBs were designed for use with low profile choc switches to create a smaller footprint and less spacing between keycaps without the need for a plate.

No coding is required! The wired QMK builds are ported with Vial and wireless ZMK builds are compatible with ZMK Studio for easy keymap changes.

Both boards are sold as kits and complete builds at [idlebuilds.com](https://idlebuilds.com).
---
### The Boards
<p align="center">
  <img src="docs/images/dinkey_32_30_32_key_config_zmk.png" width="49%">
  <img src="docs/images/dinkey_32_30_30_key_config_zmk.png" width="49%">
</p>
<p align="center">
  <img src="docs/images/dinkey_34_zmk.png" width="80%">
</p>
---
### Dinkey 34

34-key split running a 3×5+2 layout with a 3-key pinky column per side makes it easy to maintain a QWERTY layout without compromising. Good starting point if you're new to split keebs or if you just want something that works well without overthinking the key count and mapping.

→ [ZMK firmware repo](https://github.com/IdleBuilds/zmk-config-dinkey_34)

---

### Dinkey 32|30

This one is different. The PCB has a modular 4th pinky column that accepts one or two switches. No firmware change, no reflash, just populate what you want. 32 keys with both switches, 30 with one, nothing in the column if you want to go full minimal.

There's nothing else out there quite like it. Most keyboards commit you to a key count. This one doesn't. It's the board I built for myself after years of trying everything else, and the 30-key configuration is the one I keep coming back to.

→ [ZMK firmware repo](https://github.com/IdleBuilds/zmk-config-dinkey_32_30)

---

## Built to be Modular

Every component on these boards is swappable:

- **Switches** — Kailh Choc hotswap sockets, no soldering required to swap
- **Microcontroller** — hotswap socket, drop in whatever you want
- **Display** — nice!view slots in and out without tools

This matters more than it sounds. You can order the wired kit, throw in a Pro Micro, and get up and running for well under $100. When you're ready to go wireless, pull the Pro Micro, drop in a nice!nano and a nice!view, and flash ZMK. Same board, different build. Nothing wasted.

---

## Firmware

Both boards support multiple firmware options depending on your microcontroller:

**ZMK (wireless, recommended for nice!nano)** Full Bluetooth support, ZMK Studio for remapping without any code. Pre-flashed on all complete builds.

**QMK (wired, for Pro Micro)** Standard QMK, no frills. Good if you want wired-only or are working with an existing Pro Micro.

**Vial (wired, QMK-based)** Real-time keymap editing via the Vial desktop app. No code required.

The 34 and 32|30 have **separate firmware** due to different PCB routing and pin assignments. The repos are not interchangeable — use the repo that matches your board.

---

## Kits vs. Complete Builds

**Complete builds** come pre-flashed and ready to use. Plug in and go.

**Kits** ship unflashed. Flashing instructions are in each firmware repo.

---

## Repos

| Board | ZMK | QMK |
|---|---|---|
| Dinkey 34 | [zmk-config-dinkey\_34](https://github.com/IdleBuilds/zmk-config-dinkey_34) | [QMK PR pending] |
| Dinkey 32\|30 | [zmk-config-dinkey\_32\_30](https://github.com/IdleBuilds/zmk-config-dinkey_32_30) | [QMK PR pending] |

---

## Build Guide

Full step-by-step assembly instructions including soldering, flashing, and troubleshooting are at [idlebuilds.com/build-guide](https://idlebuilds.com/build-guide).

---

## Hardware

| Folder | Contents |
|---|---|
| kicad/ | PCB design files (KiCad) |
| qmk/ | QMK keyboard definition files |
| vial-qmk/ | Vial keyboard definition files |
| zmk/ | ZMK config files (legacy, see standalone repos above) |
| docs/ | Images, schematics, reference files |

---

## Specs

|  | Dinkey 34 | Dinkey 32\|30 |
|---|---|---|
| Keys | 34 | 32 or 30 |
| Switches | Kailh Choc V1 | Kailh Choc V1 |
| MCU socket | Mill-Max low profile | Mill-Max low profile |
| Switch sockets | Kailh Choc hotswap | Kailh Choc hotswap |
| Wireless controller | Nice!Nano v2 | Nice!Nano v2 |
| Wired controller | Pro Micro | Pro Micro |
| Wireless display | Nice!View | Nice!View |
| Wired display | 128×32 OLED (optional) | 128×32 OLED (optional) |
| Battery | 110mAh LiPo | 110mAh LiPo |
| Case | 3D printed | 3D printed |

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

## About

I'm Clayton. I design and build these keyboards myself out of Iowa. Idle Builds is a small side project. I'm not a company, just someone who got too into mechanical keyboards and wanted to share what I've made.

[idlebuilds.com](https://idlebuilds.com) · [GitHub](https://github.com/IdleBuilds)  
Questions, build help, or custom orders: clayton@idlebuilds.com
