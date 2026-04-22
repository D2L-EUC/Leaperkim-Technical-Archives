# Lynx OG - BLE Protocol & Software

## 📡 BLE Communication

The Lynx communicates with rider apps (DarknessBot, EUC World) over a BLE (Bluetooth Low Energy) connection using a UART-based protocol.

### Hardware
* **BLE Module:** 4-pin UART interface on the mainboard.
* **Pinout:** VCC, GND, TX, RX (standard UART).
* **Baud Rate:** *Needs verification* — likely 115200 bps (common for EUC BLE modules).

### App Compatibility
| App | Platform | Status |
| :--- | :--- | :--- |
| DarknessBot | iOS | ✅ Supported |
| EUC World | Android | ✅ Supported |
| Leaperkim App | iOS / Android | ✅ Official companion app |

### Data Available via BLE
The following telemetry data is typically available through the BLE interface:
- Speed (km/h or mph)
- Battery voltage (total pack)
- Battery percentage
- Current draw (amps)
- Temperature (controller, motor if supported)
- Trip distance / total odometer
- PWM / load percentage
- Tilt angle (pitch)
- Alarm settings

### Protocol Details
> ⚠️ **Contributions needed:** The exact BLE packet structure has not been fully decoded yet. If you have BLE sniff logs from the Lynx, please contribute them via a PR.

From community observations:
* The protocol is likely similar to other Veteran/Leaperkim models (Sherman-L shares the same platform).
* Data is transmitted as binary frames over the UART BLE bridge.
* The companion app can also adjust ride settings (speed limits, tilt-back, pedal mode, lighting modes).

## 🖥️ Onboard Display

The Lynx features an integrated LCD display that provides:
- Real-time speed
- Battery voltage and percentage
- Individual cell group voltages (via SmartBMS)
- Current draw (amperage)
- Trip and total odometer
- Ride mode settings
- Alarm/tilt-back configuration

All settings can be adjusted directly on the display without needing the app.

## 🔧 Firmware

* **MCU:** GigaDevice GD32F103 or GD32F303 (ARM Cortex-M, 108-120MHz).
* Firmware updates are typically provided by Leaperkim and flashed via the companion app or a dedicated tool.
* The Lynx uses a **hall-less motor control** algorithm — the MCU estimates rotor position from back-EMF rather than relying on hall sensors. This is a safety feature: the wheel continues to balance even if a hall sensor fails.

---

*This section needs community contributions. If you have decoded BLE packet captures, firmware analysis, or protocol documentation, please submit a Pull Request.*
