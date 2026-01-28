<div align="center">

  <img src="https://user-images.githubusercontent.com/62047147/195847997-97553030-3b79-4643-9f2c-1f04bba6b989.png" alt="logo" width="100" height="auto" />

  <h1>RF-Clown</h1>
  <p>A fully open-source BLE and Bluetooth jammer</p>

</div>

---

## 📖 Documentation

Full original documentation and background can be found here:  
👉 https://cifertech.net/rf-clown-your-portable-ble-bluetooth-jamming-tool/

---

## ⭐ About the Project

RF-Clown is an open-source BLE and Bluetooth jammer inspired by similar projects in the RF security community.  
The project emphasizes transparency, education, and experimentation over closed or proprietary implementations.

It is intended **strictly for learning, research, and controlled testing environments**.

<div align="center"> 
  <img src="https://github.com/user-attachments/assets/7be8e9b4-07ea-4f39-9cd4-d8588a95a920" alt="screenshot" width="auto" />
</div>

---

## 🔧 Fork modifications

This repository is a fork of the original **RF-Clown** project developed by **cifertech**.

### Changes introduced in this fork
- Complete PCB redesign with components relocated to new positions  
- Simplified NeoPixel LED replaced by a discrete RGB LED  
- Firmware modifications to support RGB LED control  
- Added dedicated PCB space and mechanical mounting for a lithium battery  
- Improved layout for portable and standalone operation  

Core RF concepts and operating principles remain aligned with the original project.

🔗 Original repository:  
https://github.com/cifertech/RF-Clown

---
## 📂 Repository contents

This repository hosts a **hardware and firmware variant** of the original RF-Clown project.

### 🧱 Hardware
- Complete PCB redesign
- Battery integration and mechanical support
- Discrete RGB LED (NeoPixel removed)
- Gerber files for manufacturing

### 💻 Firmware
- Modified ESP32 firmware matching the redesigned hardware
- RGB LED signaling logic
- Not drop-in compatible with the original RF-Clown firmware


## 🎯 Features

- **Dual NRF24 modules** (GT24 Mini modules) for BLE/Bluetooth interference experiments  
- **External antennas** via IPEX connectors  
- **RGB LED feedback**: Discrete RGB LED for mode indication *(firmware adapted in this fork)*  
- **Portable design**: Battery-powered operation using Li-ion/Li-Po cell and TP4056 charger  
- **Custom PCB**: CP2102 USB-UART, LF33 voltage regulator, and supporting circuitry  
- **Open-source hardware and firmware**  

> ⚠️ **Note:** Hardware and firmware in this repository are **not compatible** with the original RF-Clown NeoPixel-based PCB.


---

## 🔋 Battery & PCB redesign details (Fork)

This fork introduces a **fully redesigned PCB** integrating battery support and updated LED signaling.

<div align="center">

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/bce4d634-b910-46ed-b72f-ca8a44866b1e" alt="PCB top view" width="400"/>
      <p><i>Top layer</i></p>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/bf6eca23-521a-4707-8545-668c2ddd23e8" alt="PCB bottom view" width="400"/>
      <p><i>Bottom layer</i></p>
    </td>
  </tr>
</table>

<p><i>Redesigned PCB layout with battery mounting and updated RGB LED placement</i></p>

</div>

### Mechanical & design notes
- PCB layout redesigned to integrate battery mounting without interfering with RF modules  
- NeoPixel replaced by a discrete RGB LED to simplify hardware and reduce component count  
- RGB LED placement optimized for visibility and mechanical clearance  
- RF-sensitive areas and antenna routing preserved during redesign  

---

## 🔗 Firmware upload (ESP32)

Firmware in this fork is **not drop-in compatible** with the original hardware due to the RGB LED change.

### Arduino IDE
- ESP32 Board Package version: **1.0.5**

### Precompiled firmware
If provided, `.bin` files can be flashed using Espressif Flash Download Tool:

- Start address: `0x1000`  
- Baud rate: `115200`

---

## ⚠️ DISCLAIMER — IMPORTANT

> **Legal & Regulatory Notice**
>
> This project is intended **for educational, research, and controlled testing purposes only**.
>
> BLE and Bluetooth jamming, interference, or disruption of radio communications may be **illegal** in many countries and jurisdictions.
>
> The author of this fork and the original project contributors **do not assume any responsibility** for misuse, illegal operation, or regulatory violations resulting from the use of this project.
>
> **Always comply with local laws and RF regulations** when working with radio frequency equipment.

---

## 📜 License

This project is distributed under the **MIT License**, following the same license terms as the original RF-Clown project.  
See `LICENSE.txt` for details.

---

## 🤝 Credits

Original project by **cifertech**  
https://github.com/cifertech/RF-Clown  

Forked hardware & firmware variant maintained by **Cristian Castro (CrissCCL)**

