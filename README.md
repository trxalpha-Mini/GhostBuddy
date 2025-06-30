# GhostBuddy – Keychain Module (Solder Submission)


Slack username: TRXAlpha


GhostBuddy is a compact, modular keychain peripheral for my personal AI assistant, Ghost. It provides haptic and visual feedback (via vibration motor and LEDs), along with buttons for interacting with Ghost even when away from a computer or phone. The goal is to make Ghost always with me—on my keys, in my pocket, and always connected to my world.

This is the **Solder version**, designed as part of HackClub's Summer of Making. It is part of a larger modular ecosystem, including a "Mother" dashboard module, desk hub, and presence-aware triggers using NFC and ESP-NOW.

---
The schematic (with the ESP32-C3 chip, USB-UART CH340C chip and USB-C port)
![image](https://github.com/user-attachments/assets/012b617b-f867-4f7b-980e-dbc062376c34)

The PCB (without the ESP, CH340C chip and USB-C port)
![image](https://github.com/user-attachments/assets/a7aebf02-f884-4fc7-93ab-33827337c07c)


And the 3D view of the PCB:
![image](https://github.com/user-attachments/assets/a8944831-dc9a-4647-bb7e-db2b09fb801d)

and the back:
![image](https://github.com/user-attachments/assets/3d232f92-2e23-42d4-9da5-54bf58d11f13)


## 🔧 Description

The GhostBuddy Keychain Module features:

- ESP32-C3 (in schematic only, not on this PCB)  
- Vibrating motor for tactile notifications  
- Addressable LEDs for alerts, presence status, and mood  
- Two tactile buttons for interaction and acknowledgment  
- Coin cell power (CR2032)  - 2 in the schematic
- Compact layout to fit on a keychain  

> 🔋 The design focuses on ultra-low power operation, wake-on-button, and periodic ESP-NOW syncing with the Mother module.

---

## 📦 Bill of Materials (BOM)

| Item                     | Quantity |
|--------------------------|----------|
| Vibration motor (coin type) | 1        |
|  LEDs  | 4        |
| Tactile push buttons     | 4        |
| CR2032 battery holder   | 1       |
| Diodes (for power protection) 1N5B19 | 1        |
| Resistors (for LED/data lines), 220 ohm each | 18    |
| Capacitor 10uF | 1    |
| Custom PCB               | 1        |

---

## 💡 Note About the ESP32-C3

Although the ESP32-C3, USB-C, and UART converter are included in the **schematic**, they are not part of this PCB submission for Solder. This schematic is meant to serve as a **reference for the Highway version**, which I plan to submit soon. That version will include the ESP32-C3 and the supporting circuitry to complete the module's connectivity.

The intention is:
- Submit this design to **Solder** to get the PCB grant and showcase the concept.
- Submit a follow-up to **Highway** to receive funding for the MCU and USB parts, reducing the Highway BOM, as for the PCB I will use the **Solder** grant.

---

## 🚀 Project Goals

- Enable Ghost to send alerts anywhere via vibration and LED cues
- Offline-friendly (ESP-NOW-based, no always-on Wi-Fi needed)
- Modular hardware with spiritual and emotional value (inspired by my Shiba Inu companions)
- Extendable ecosystem with a Mother module, desk hub, and NFC location detection

---

Stay tuned for firmware and demo code!

P.S.: Ghost is my AI assistant, running on my laptop

