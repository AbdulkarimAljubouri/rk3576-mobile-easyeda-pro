# RK3576 Android Mobile — EasyEDA Pro Skeleton

This repository contains an EasyEDA Pro project skeleton for a Rockchip RK3576 Android-ready mobile board:
- RK806-2 PMIC + IP2726 charger
- 8 GB LPDDR4/4X, eMMC 256 GB (mandatory)
- USB-C (USB2 + PD sink), Micro HDMI Type-D
- Wi-Fi/BT: BL-M8852BS2
- DSI/Touch, dual CSI cameras, audio codec ES8388
- Android keys + LEDs, debug UART/JTAG
- ESD and power-tree placeholders

Import options:
- EasyEDA Pro: File → Import → Project and select the ZIP built from this repo’s rk3576-mobile-easyeda-pro folder
- Or rename the ZIP to .epro and open directly in EasyEDA Pro

Project structure:
- project.json — EasyEDA Pro project descriptor
- sheets/ — 18 schematic placeholder pages (frames + notes)
- docs/ — design notes: sheet plan, net naming, layout rules, power sequence, decisions, changelog
- bom/BOM_LCSC_MATCH.csv — BOM with LCSC references, SPECIAL-PROC tags
- firmware/rk3576-mobile.dts — DT starter for Android/Linux enablement

Next steps:
1) Attach your symbol/footprint libraries for RK3576, RK806-2, LPDDR4X, eMMC, BL-M8852BS2.
2) Place parts and wire nets using the docs’ net naming.
3) Replace TBD-LCSC with chosen in-stock parts in the BOM.
4) Follow the bring-up notes and layout guidelines.

License: MIT
