# 🍟 Fresh Mate Fries Case

[简体中文](README.md) · [Fresh Mate Software Repository][main-repo]

![Fresh Mate fries-shaped enclosure render](images/freshmate-fries-case-render.png)

This is a 3D-printable fries-shaped enclosure for the Fresh Mate hardware edition, designed around the ESP32-S31-Korvo-1. The PWA, backend, and firmware live in the separate main software repository.

## 🧩 Compatibility

- Target board: ESP32-S31-Korvo-1.
- Target display: the matching 800×480 LCD.
- Other boards, displays, speakers, and camera combinations are untested.
- Verify port positions and physical dimensions against your own board revision before printing.

## 📦 Files

| File | Purpose |
|---|---|
| `models/freshmate-fries-front.stl` | Printable front shell |
| `models/freshmate-fries-back.stl` | Printable back shell |
| `models/freshmate-fries-accent.stl` | Separate fries/accent-color part |
| `models/freshmate-fries-case.3mf` | Combined print project |
| `source/freshmate-fries-case.blend` | Editable Blender source |

## 🖨️ Before Printing

You need slicing software, an FDM or compatible printer that accepts STL/3MF, and enclosure-appropriate material.

This release has not been validated across printers, so fixed values are intentionally not claimed yet:

- Nozzle diameter: `TBD — pending physical validation`
- Layer height: `TBD — pending physical validation`
- Wall thickness and infill: `TBD — pending physical validation`
- Supports and print orientation: `TBD — pending physical validation`
- Assembly tolerances: `TBD — pending physical validation`
- Material and thermal settings: `TBD — pending physical validation`

Inspect dimensions, thin walls, overhangs, and connector openings in your slicer before choosing orientation and supports.

## 🧱 Suggested Assembly Flow

1. Print the front, back, and accent parts; remove supports and burrs.
2. Test-fit the ESP32-S31-Korvo-1 without power and confirm that USB, speakers, microphones, and buttons remain accessible.
3. Place the board and display into the back shell and inspect cable and ventilation clearance.
4. Test-fit the front and accent parts without pressing on the display or connectors.
5. Complete fastening only after fit is confirmed, then perform a powered test.

Exact screws, snap fits, and adhesive choices are pending physical validation. Do not force the enclosure closed.

## ✏️ Editing the Source

Open the source in Blender:

```text
source/freshmate-fries-case.blend
```

Redistributed adaptations must retain attribution, identify changes, and follow the non-commercial license.

## 🔗 Software and Firmware

The PWA, backend, AI provider interfaces, and ESP32 firmware are available at:

**[Fresh Mate Open Source][main-repo]**

## 🤝 Feedback

Issues with tested printers, materials, layer heights, supports, fit, and finished photos are welcome. Do not upload photos or logs containing network passwords, device keys, or personal information.

## 📄 License

Original models in this repository are licensed under [Creative Commons Attribution-NonCommercial 4.0 International](LICENSE) (CC BY-NC 4.0): sharing and adaptation with attribution are allowed; commercial use is not.

This license does not cover the ESP32-S31-Korvo-1 board, Espressif trademarks, or third-party hardware designs. The Fresh Mate software repository uses the separate Apache-2.0 license.

[main-repo]: https://github.com/choul798188551-tech/freshmate-open-source
