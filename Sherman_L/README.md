# LeaperKim Veteran Sherman-L - Technical Documentation

The Sherman-L (~2023) is the long-range flagship successor to the Sherman-S. It jumped to the 151.2V platform (shared with the Lynx), gained a much larger battery, and introduced the SmartBMS and 36-MOSFET controller design.

## ⚡ Technical Specifications

| Parameter | Value |
| :--- | :--- |
| **Voltage** | 151.2V Max (126V Nominal) |
| **Battery** | 4,000Wh (Samsung 50S 21700 cells, 36S configuration) |
| **Motor** | 3,200W Nominal |
| **Peak Power** | 8,000W (8KW) |
| **Tire** | 20" | 80/90-14 (Tubeless) |
| **Top Speed** | ~55 mph (88 km/h) |
| **Range** | ~100-130 miles (depending on speed) |
| **Weight** | ~110 lbs (~50 kg) |
| **Max Load** | 330 lbs (150 kg) |
| **Suspension** | FastAce hydraulic shocks |
| **Charging** | Dual GX20/5-pin connectors |
| **Controller** | 36x MOSFETs (200V rated, TO-263 package) |
| **Frame** | Magnesium alloy |

## 🛠️ Key Components

### Electronics
* **Mainboard:** 36x MOSFETs — same proven controller architecture as the Lynx OG.
* **MCU:** GigaDevice GD32F103 or GD32F303 (ARM Cortex-M, 108-120MHz) — likely shared platform with Lynx.
* **BMS:** SmartBMS with individual cell monitoring via the display.
* **Display:** High-brightness LCD showing real-time amperage, voltage, and cell data.
* **BLE Module:** 4-pin UART communication for DarknessBot / EUC World apps.

### Mechanical
* **Suspension:** FastAce hydraulic shocks with adjustable preload, rebound, and compression.
* **Spring Weights:** 62 lbs (Soft) / 66 lbs (Medium) / 70 lbs (Hard).
* **Frame:** Magnesium alloy (lighter than the steel roll cage of Sherman OG/S).
* **Pedals:** Standard pedals with fixed height (aftermarket lowering brackets common).
* **Trolley Handle:** Locking retractable trolley handle.
* **Kickstand:** Fixed kickstand (not folding).
* **Toe Pads:** Adjustable-height toe pads for curb hopping and emergency braking.

### Lighting
* **Headlight:** ~20W / 2,500 lumens projector light.
* **Taillight:** WS2811-based addressable LED rear light with turn signal functionality.

## 📝 Notes

* The "L" stands for **Long range** — the 4,000Wh pack is one of the largest in the 20" class.
* Shares the 151.2V / 36-MOSFET platform with the Lynx OG (many parts are interchangeable).
* The magnesium alloy frame was a major upgrade over the steel roll cage — lighter and better heat dissipation.
* eWheels best-selling Leaperkim model as of 2025.
* Popular aftermarket mod: pedal lowering brackets (later built into the Oryx and Lynx-S natively).

---

## 📑 Section Links
- [Hardware](./Hardware/) *(contributions needed)*
- [Mechanical](./Mechanical/) *(contributions needed)*
- [Software Protocol](./Software_Protocol/) *(contributions needed)*
- [Maintenance](./Maintenance/) *(contributions needed)*
