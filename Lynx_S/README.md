# LeaperKim Veteran Lynx-S - Technical Documentation

The Lynx-S (2025) is the updated version of the original Lynx, featuring a new higher-output motor, redesigned suspension, and several quality-of-life improvements. It shares the same battery and controller hardware platform as the Lynx OG but with significant firmware optimization and mechanical refinements.

## ⚡ Technical Specifications

| Parameter | Value |
| :--- | :--- |
| **Voltage** | 151.2V Max (126V Nominal) |
| **Battery** | 2,700Wh (Samsung 50S 21700 cells, 36S configuration) |
| **Motor** | 3,800W Nominal (C42 motor — wider 42mm stator/magnet width) |
| **Peak Power** | 10,000W (10KW) |
| **Tire** | 20" | 80/90-14 (Tubeless, choice of knobby or street) |
| **Top Speed** | ~60 mph (96 km/h) |
| **Range** | ~60 miles (96 km) |
| **Weight** | 94 lbs (43 kg) |
| **Max Load** | 330 lbs (150 kg) |
| **Suspension** | Cylindrical shocks, 80/90mm travel, air chamber + compression/rebound |
| **Charging** | Dual GX20/5-pin (Max 20A total — up from 15A on OG) |
| **Controller** | 36x MOSFETs with thicker bus bars |
| **Frame** | Magnesium alloy |

## 🛠️ Key Components

### Electronics
* **Controller:** Same 36-MOSFET hardware platform as Lynx OG, but with thicker bus bars for improved efficiency and more stable power delivery. Firmware optimized for the new C42 motor.
* **MCU:** GigaDevice GD32 series (ARM Cortex-M) — inherited from Lynx platform.
* **BMS:** SmartBMS with individual cell monitoring, rated for 20A charge rate.
* **Motor Temperature Sensor:** New addition — monitors motor temperature as a safety feature.
* **Display:** LCD display with updated app version support.
* **BLE Module:** UART Bluetooth for DarknessBot / EUC World / companion app.
* **Hall-less Operation:** Revised mode that keeps the wheel balancing even if hall sensors fail (safety feature).

### Mechanical
* **Motor:** C42 — widest magnets of any EUC released so far (42mm stator/permanent magnet width). Provides significantly more torque than the OG Lynx motor, enabling higher field weakening speeds.
* **Suspension:** All-new design vs. OG Lynx. Both shocks now use identical cartridge design with:
  - Adjustable rebound & compression on *both* sides (OG had these split across shocks).
  - Inflatable air chamber (replaces the older spring-tension preload adjustment).
  - Separation of air and oil for improved damping performance.
* **Spring Weights:** 62 lbs (<190 lbs rider) / 66 lbs (190-220 lbs) / 70 lbs (>220 lbs).
* **Pedals:** Larger Oryx-style pedals with replaceable studs and **three adjustable height placements**.
* **Kickstand:** Folding design (from Oryx) — reduces damage risk in crashes.
* **Frame:** Improved rigidity through better suspension tolerances.

### Lighting
* **Headlight:** 25W / 3,000 lumens (from Oryx design) — up from 20W / 2,500 lumens on OG.
* **Taillight:** Revised WS2811-based rear light with triple-zone turn signals (same architecture as Lynx S Rear Light documented in Lynx_OG).

## 🔄 Differences from Lynx OG

| Feature | Lynx OG | Lynx-S |
| :--- | :--- | :--- |
| Motor | 3,200W | 3,800W (C42) |
| Peak Power | 8KW | 10KW |
| Top Speed | ~55 mph | ~60 mph |
| Suspension | Split compression/rebound | Identical dual shocks + air chamber |
| Max Charge Rate | 15A | 20A |
| Headlight | 20W / 2,500 lm | 25W / 3,000 lm |
| Kickstand | Fixed | Folding |
| Pedal Height | Fixed | Adjustable (3 positions) |
| Motor Temp Sensor | No | Yes |

## 📝 Notes

* The Lynx-S suspension is a **drop-in replacement** for the Lynx OG — available separately for OG owners who want to upgrade.
* The C42 motor is physically compatible with the OG Lynx but the firmware won't be optimized, leaving performance on the table. The controller tray is also physically larger, making a full swap complex and expensive.
* Battery pack is **identical** to the Lynx OG (Samsung 50S, 2,700Wh, 151.2V).
* Priced at $3,699 USD (eWheels, 2025).

---

## 📑 Section Links
- [Hardware](./Hardware/) *(contributions needed — see [Lynx OG Hardware](../Lynx_OG/Hardware/) for shared platform reference)*
- [Mechanical](./Mechanical/) *(contributions needed)*
- [Software Protocol](./Software_Protocol/) *(contributions needed — likely similar to Lynx OG BLE protocol)*
- [Maintenance](./Maintenance/) *(contributions needed)*
