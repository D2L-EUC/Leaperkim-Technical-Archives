# LeaperKim Veteran Sherman (Original) - Technical Documentation

The Sherman was LeaperKim's debut product (~2020), the wheel that put the Veteran brand on the map. It was one of the first EUCs designed for high-speed street riding, with a massive battery and a rugged steel roll cage body.

## ⚡ Technical Specifications

| Parameter | Value |
| :--- | :--- |
| **Voltage** | 100.8V Max (84V Nominal) |
| **Battery** | 3,200Wh (LG/Samsung 21700 cells, 24S configuration) |
| **Motor** | 2,500W Nominal |
| **Peak Power** | ~5,000W (estimated) |
| **Tire** | 20" × 2.5" (Tubeless) |
| **Top Speed** | ~45 mph (72 km/h) |
| **Range** | ~80-128 miles (depending on speed) |
| **Weight** | ~77 lbs (35 kg) |
| **Max Load** | 330 lbs (150 kg) |
| **Suspension** | None (rigid frame) |
| **Charging** | Dual GX20 charging ports |
| **Frame** | Steel roll cage design |

## 🛠️ Key Components

### Electronics
* **Controller:** Early MOSFET design, pre-dates the 36-FET layout used in later models.
* **BMS:** Basic BMS with cell-group monitoring.
* **Display:** Onboard LCD control panel (speed, battery %, mileage, settings).
* **BLE Module:** UART-based Bluetooth for DarknessBot / EUC World app connectivity.

### Mechanical
* **Body:** Utilitarian steel roll cage — extremely durable but heavy.
* **Pedals:** Long foot pedals (can scrape during aggressive turns).
* **Trolley Handle:** Retractable trolley handle for rolling when not riding.
* **Headlight:** Bright front projector headlight.
* **Taillight:** Rear light with turn signal functionality.

## 📝 Notes

* The Sherman was the first Veteran model and introduced many design elements carried forward (dual charge ports, roll cage frame concept, GX20 connectors).
* No suspension — this was a rigid-frame design. Suspension was introduced with the Sherman-S.
* Known for its range and straight-line speed stability on paved roads.
* Internal access and tire changes are complex due to the roll cage design.
* No spin-kill button on the original model.

## ⚠️ Known Issues

* Heavy weight limits off-road and technical trail usage.
* Low roll cage clearance can be problematic on curbs/obstacles.
* Tire changes require significant disassembly.
* Being a first-generation product, early batches had various QC refinements over production runs.

---

## 📑 Section Links
- [Hardware](./Hardware/) *(contributions needed)*
- [Mechanical](./Mechanical/) *(contributions needed)*
- [Software Protocol](./Software_Protocol/) *(contributions needed)*
- [Maintenance](./Maintenance/) *(contributions needed)*
