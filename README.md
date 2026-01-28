<div align="center">

  <img src="https://user-images.githubusercontent.com/62047147/195847997-97553030-3b79-4643-9f2c-1f04bba6b989.png" alt="logo" width="100" height="auto" />

  <h1>RF-Clown</h1>
  <p>A fully open-source BLE and Bluetooth jammer</p>

  <!-- Badges -->
  <a href="https://github.com/YOUR_USERNAME/RF-Clown">
    <img src="https://img.shields.io/github/stars/YOUR_USERNAME/RF-Clown?style=social" alt="stars">
  </a>
  <a href="https://github.com/YOUR_USERNAME/RF-Clown">
    <img src="https://img.shields.io/github/forks/YOUR_USERNAME/RF-Clown?style=social" alt="forks">
  </a>

</div>

---



## 📖 Documentation

Full original documentation and background can be found here:  
👉 https://cifertech.net/rf-clown-your-portable-ble-bluetooth-jamming-tool/

<div>&nbsp;</div>

---

## ⭐ About the Project

RF-Clown is an open-source BLE and Bluetooth jammer inspired by similar projects in the RF security community.  
The project emphasizes transparency, education, and experimentation over closed or proprietary implementations.

It is intended **strictly for learning, research, and controlled testing environments**.

<div align="center"> 
  <img src="https://github.com/user-attachments/assets/7be8e9b4-07ea-4f39-9cd4-d8588a95a920" alt="screenshot" width="auto" />
</div>

<div>&nbsp;</div>

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

<div>&nbsp;</div>

---

## 🎯 Features

- **Triple NRF24** (GT24 Mini modules) for increased RF coverage  
- **External antennas**: IPEX connectors + high-gain antennas  
- **OLED display** + **3 tactile switches** for user navigation  
- **RGB LED feedback**: Discrete RGB LED for mode indication *(firmware adapted in this fork)*  
- **Portable design**: Battery-powered operation using Li-ion/Li-Po cell and TP4056 charger  
- **Custom PCB**: CP2102 USB-UART, LF33 voltage regulator, and supporting circuitry  
- **Open-source firmware and hardware**  

<div>&nbsp;</div>

---

## 🔋 Battery & PCB redesign details (Fork)

This fork introduces a **fully redesigned PCB** integrating battery support and updated LED signaling.

<div align="center">
  <img src="docs/pcb_redesign_overview.png" alt="PCB redesign overview" width="600"/>
  <p><i>Redesigned PCB layout with battery mounting and updated RGB LED placement</i></p>
</div>

### Mechanical & design notes
- PCB layout redesigned to integrate battery mounting without interfering with RF modules  
- NeoPixel replaced by a discrete RGB LED to simplify hardware and reduce component count  
- RGB LED placement optimized for visibility and mechanical clearance  
- RF-sensitive areas and antenna routing preserved during redesign  

<div>&nbsp;</div>

---

## 🔗 Firmware upload (ESP32)

Firmware in this fork is **not drop-in compatible** with the original hardware due to the RGB LED change.

### Arduino IDE
- ESP32 Board Package version: **1.0.5**

### Precompiled firmware
If provided, `.bin` files can be flashed using Espressif Flash Download Tool:

- Start address: `0x1000`  
- Baud rate: `115200`

<div>&nbsp;</div>

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

<div>&nbsp;</div>

---

## 📜 License

This project is distributed under the **MIT License**, following the same license terms as the original RF-Clown project.  
See `LICENSE.txt` for details.

<div>&nbsp;</div>

---

## 🤝 Credits

Original project by **cifertech**  
https://github.com/cifertech/RF-Clown  

Forked hardware & firmware variant maintained by **YOUR_NAME**

<div>&nbsp;</div>


