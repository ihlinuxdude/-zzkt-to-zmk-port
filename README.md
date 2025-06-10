# zzkt-to-zmk-port

This repository contains a ZMK port of the zzkt QMK keymap for the **Charybdis 4x6** split keyboard with a **Nice!Nano** controller and built-in trackball support.

---

## ✅ Features
- Fully ported `BASE`, `NUMERIC`, `MOVE`, `EMACS`, `HYPM`, and `MOUSE` layers
- Left/Right Click via `&mkp LCLK` and `&mkp RCLK`
- Bluetooth clear (`&bt BT_CLR`) on NUMERIC layer `1`
- Sniper and scroll-mode mouse behaviors
- Designed for ZMK GitHub Actions CI workflow

---

## 🧰 Hardware
- **Keyboard**: Charybdis 4x6
- **MCU**: Nice!Nano (both sides)
- **Pointer**: Trackball (center-mounted)

---

## 📁 Folder Structure
```
config/
├── keymap.keymap              # YAML ZMK keymap
├── shields/
│   ├── charybdis_4x6_left/
│   │   └── shield.overlay     # Mouse behaviors
│   └── charybdis_4x6_right/
│       └── shield.overlay     # Mouse behaviors
build.yaml                     # Build config for GitHub Actions
```

---

## 🚀 Building Firmware (GitHub CI)
1. Fork this repo to your GitHub account
2. Push changes or edit `keymap.keymap`
3. GitHub Actions will build:
   - `firmware-charybdis_4x6_left-nice_nano.uf2`
   - `firmware-charybdis_4x6_right-nice_nano.uf2`
4. Download artifacts from the Actions tab

---

## 💡 Notes
- Pointer behavior (`&mkp`) may need tuning based on your firmware speed/trackball type
- If you want to add logo animations or OLED output, see ZMK display documentation

---

## 📎 Credit
Originally based on [`zzkt/charybdis`](https://github.com/zzkt/charybdis)
Ported to ZMK by [you] using ChatGPT automation.

---

## License
MIT or same license as original QMK repo (if derivative).
# -zzkt-to-zmk-port
This is a port of zzkt's keymap with some minor tweaks from QMK to ZMK
