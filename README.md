# LeaperKim Technical Archives 🛠️⚡

Welcome to the **LeaperKim Technical Archives**. This is a collaborative, open-source project dedicated to the technical documentation and reverse engineering of LeaperKim (Veteran) electric unicycles (EUC).

The goal is to provide a central "Source of Truth" for riders, repair shops, and modders to understand, maintain, and improve these machines.

---

## ⚠️ MANDATORY DISCLAIMER

**PROCEED WITH EXTREME CAUTION.**

1. **SAFETY:** LeaperKim wheels operate at extremely high voltages (up to **176.4V DC** on the Oryx). Improper handling can result in **fire, explosion, severe injury, or death**.
2. **LIABILITY:** This repository is for educational purposes only. The contributors are not responsible for any damage to your wheel or yourself.
3. **WARRANTY:** Opening your motor or controller housing can void your manufacturer warranty.
4. **INDEPENDENCE:** This project is not affiliated with, authorized, or endorsed by LeaperKim.

---

## 🏭 About LeaperKim

LeaperKim (brand name: **Veteran**) is a Chinese electric unicycle manufacturer that entered the EUC market around 2020 with the original Sherman. They are known for their robust build quality, reliable controller designs, and FastAce suspension partnerships. Their product line spans from mid-size commuters to high-performance long-range cruisers.

---

## 🚲 Documented Models

| Model | Year | Voltage | Battery | Motor | Tire | Status |
| :--- | :---: | :---: | :---: | :---: | :---: | :--- |
| [**Lynx (OG)**](./Lynx_OG) | 2023 | 151.2V | 2,700Wh | 3,200W | 20" | 🟢 Active |
| [**Lynx-S**](./Lynx_S) | 2025 | 151.2V | 2,700Wh | 3,800W | 20" | 🟡 Specs |
| [**Sherman (OG)**](./Sherman_OG) | 2020 | 100.8V | 3,200Wh | 2,500W | 20" | 🟡 Specs |
| [**Sherman-S**](./Sherman_S) | 2022 | 100.8V | 3,500Wh | 2,800W | 20" | 🟡 Specs |
| [**Sherman-L**](./Sherman_L) | 2023 | 151.2V | 4,000Wh | 3,200W | 20" | 🟡 Specs |
| [**Patton-S**](./Patton_S) | 2024 | 134.4V | 2,220Wh | 3,000W | 17" | 🟡 Specs |
| [**Oryx**](./Oryx) | 2025 | 176.4V | 4,700Wh | 4,200W | 22" | 🟡 Specs |

**Legend:** 🟢 Active (hardware teardown data) · 🟡 Specs (specifications only) · 🔴 Pending

---

## 📂 Project Structure

Each model folder follows this standardized structure:
* `/Hardware`: PCB photos, MOSFET specs, BMS pinouts, and fuse ratings.
* `/Mechanical`: CAD files (STL/STEP), bearing sizes, and suspension tuning.
* `/Software_Protocol`: BLE packet analysis and error code definitions.
* `/Maintenance`: Torque specs and step-by-step disassembly.

---

## 🤝 How to Contribute

We rely on the community to grow. You can help by:
- Providing high-resolution photos of internal components.
- Sharing decoded BLE logs from your own testing.
- Uploading 3D printable designs for protective gear or mods.

*Please use the **Issue** tracker for discussions or submit a **Pull Request** for data updates.*

---

## 📜 License

This project is licensed under **Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International (CC BY-NC-SA 4.0)**.
