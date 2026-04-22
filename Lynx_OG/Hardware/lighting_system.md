# Lighting System - LeaperKim Lynx

The Lynx uses a modular lighting system connected via **3.5mm TRS (Jack) connectors**. This allows for easy replacement but requires specific pinout knowledge for custom mods.

---

## 🔌 Connector Specifications
Both front and rear lights use a **3.5mm 3-pole (TRS) Jack**.

### Front Light Pinout (Projector)
* **Voltage:** 24V DC
* **Maximum Power:** Original is ~10-15W (documented mod: *Cyclop Halo by mrmyart* operates at 20W).
* **Pinout:**
    * **Tip:** +24V (Power)
    * **Ring:** Signal (PWM/Data) - Controls the internal beeper and Projector ON/OFF.
    * **Sleeve:** GND

### Rear Light Pinout (Tail Light)
The tail light is an addressable LED system.
* **Voltage:** 5V DC
* **Driver IC:** Worldsemi **WS2811** (3-channel LED driver).
* **Pinout (Internal PCB labels):**
    * **Red Wire (红):** +5V (VCC)
    * **White Wire (白):** Signal (S) - Data line for WS2811.
    * **Black Wire (黑):** GND (-)

---

## 🔬 Component Analysis: Original Rear Light
Based on PCB inspection of the OEM unit:
* **IC:** WS2811 8-bit LED driver. This indicates that the main controller sends a serial data stream to control brightness and patterns (Brake, Turn signals, Idle).
* **Wiring:** The PCB uses standard Chinese color coding (Red/White/Black).
* **Modding Potential:** Since it uses WS2811, one could theoretically intercept the signal with an Arduino/ESP32 to create custom light shows or synchronize with external LED strips.


---

## ⚡ Power Supply (DCDC Converter)
The lighting and accessory system is powered by an internal DC-DC converter stepping down the main battery voltage (151.2V).

* **Estimated Total Capacity:** ~48W to 60W (TBC).
* **Warning:** Running high-power front lights (like 40W+ "Aggressor" style lights) alongside the display and cooling fans may approach the limit of the OEM DCDC converter. 

> **Status:** ⚠️ *Inquiry needed. We need to locate the DCDC module on the mainboard to identify the exact chip and its rated amperage.*