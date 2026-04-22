# LeaperKim Veteran Oryx - Technical Documentation

The Oryx (2025) is Leaperkim's flagship long-range performance cruiser. It features the highest voltage (176.4V), the largest battery (4,700Wh), the most powerful motor (4,200W), and the most advanced controller (48 MOSFETs) in the Veteran lineup. Built around a 22" wheel with FastAce suspension, it is designed for high-speed touring and long-distance commuting.

## ⚡ Technical Specifications

| Parameter | Value |
| :--- | :--- |
| **Voltage** | 176.4V Max (147V Nominal) |
| **Battery** | 4,700Wh (Samsung 50S 21700 cells) |
| **Motor** | 4,200W Nominal |
| **Peak Power** | 10,500W (10.5KW) |
| **No-Load Max RPM** | Equivalent to ~93 mph (not riding speed) |
| **Tire** | 22" | 3.5-16 (Tubeless, choice of knobby or hybrid) |
| **Cruising Speed** | 60+ mph |
| **Range** | ~150 miles at 20 mph |
| **Weight** | 127 lbs (58 kg) |
| **Max Load** | 330 lbs (150 kg) |
| **Suspension** | FastAce hydraulic, 90mm travel, floating piston design |
| **Charging** | Up to 20A rapid charge capable |
| **Controller** | 48x MOSFETs (1,120A peak instantaneous current / ~200kW) |
| **Frame** | Magnesium alloy |

## 🛠️ Key Components

### Electronics
* **Controller:** 48x MOSFETs — upgraded from 36 to 48 FETs (16 per motor phase, up from 12). Dual-layer PCB design:
  - **Lower layer:** Copper bus bars for power delivery — reduces temperatures.
  - **Upper layer:** Logic/signal section — isolated from power layer to minimize interference.
* **MCU:** GigaDevice GD32 series (ARM Cortex-M) — shared platform evolution from Lynx/Sherman-L.
* **BMS:** SmartBMS with individual cell monitoring, rated for 20A charge rate.
* **Hall-less Operation:** Inherited from Lynx-S — allows coming to a safe stop if hall sensors fail.
* **Display:** Interactive LCD display — speed, battery, mileage, and full settings adjustment.
* **BLE Module:** UART Bluetooth for companion app (iOS/Android), DarknessBot, EUC World.

### Motor
* **4,200W nominal** — Leaperkim's most powerful motor.
* **Magnesium alloy rim and motor covers** — less spinning mass = better acceleration, braking, and reduced gyro effect.
* **Larger stator core diameter** — moves the magnetic interaction point closer to the tire for more "leverage" (better torque and efficiency).

### Suspension
* **FastAce hydraulic shocks** — new design developed specifically for the Oryx.
* **90mm travel** — smooth on all terrain.
* **Floating piston design** — keeps hydraulic oil and air separate for consistent, predictable damping.
* **Adjustable:** Rebound, compression, and preload.
* **Spring Weights:** 62 lbs (<190 lbs rider) / 66 lbs (190-220 lbs) / 70 lbs (>220 lbs).

### Lighting
* **Headlight:** 25W / 3,000 lumens — all-new beam pattern with secondary daytime running lights. Improved visibility at night for high-speed cruising.
* **Taillight:** Turn signal capable rear light (WS2811-based architecture assumed, consistent with other Veteran models).

### Other Features
* **Folding Kickstand:** Reduces crash damage risk (from Lynx-S/NOSFET Apex lineage).
* **Adjustable Pedal Height:** Two factory mounting positions — lower for high-speed stability, higher for off-road clearance. Easier to switch than previous models (pedals don't need removal).
* **Locking Trolley Handle:** For rolling the wheel when not riding.
* **Adjustable Toe Pads:** For curb hops and emergency braking.

## 📊 Lineup Comparison

| Feature | Sherman-L | Lynx OG | Lynx-S | Oryx |
| :--- | :---: | :---: | :---: | :---: |
| Voltage | 151.2V | 151.2V | 151.2V | 176.4V |
| Battery | 4,000Wh | 2,700Wh | 2,700Wh | 4,700Wh |
| Motor | 3,200W | 3,200W | 3,800W | 4,200W |
| MOSFETs | 36 | 36 | 36 | 48 |
| Peak Power | 8KW | 8KW | 10KW | 10.5KW |
| Tire | 20" | 20" | 20" | 22" |
| Weight | ~110 lbs | ~95 lbs | 94 lbs | 127 lbs |
| Folding KS | No | No | Yes | Yes |
| Adj. Pedals | No | No | Yes | Yes |

## 📝 Notes

* Named after the Oryx antelope — a departure from the military naming theme (Sherman, Patton). The internal codename was "Onyx" during development.
* The 22" tire provides exceptional stability at high speed and rolls over road imperfections more smoothly than 20" wheels.
* At 127 lbs, this is Leaperkim's heaviest wheel — not ideal for technical off-road trails or frequent lifting.
* The 176.4V platform is currently unique to the Oryx (no other Veteran model shares this voltage).
* Priced at $4,999 USD (eWheels, 2025).

---

## 📑 Section Links
- [Hardware](./Hardware/) *(contributions needed)*
- [Mechanical](./Mechanical/) *(contributions needed)*
- [Software Protocol](./Software_Protocol/) *(contributions needed)*
- [Maintenance](./Maintenance/) *(contributions needed)*
