
---

## ✨ Features

- **Analog Front-End:** TI ADS1294 – 4-channel, 24-bit ADC with integrated ECG/EMG front-end  
- **MCU:** ATmega1284P – 8-bit AVR, 128KB Flash, 16KB SRAM  
- **Motion Sensing:** NXP MMA8652 3-axis accelerometer  
- **Wireless:** BR-LE4.0-D2A Bluetooth Low Energy module  
- **LED Driver:** IS31FL3199 with RGB LED indicators  
- **Power Management:**
  - MCP73831 Li-Ion/Li-Po charger  
  - TPS78233 LDO regulator  
  - NCP300L voltage detector  

- **Connectivity:**
  - Micro-USB charging & power  
  - 2x pin headers for expansion/debugging  
  - UART/SPI/I²C exposed  

---

## 🔧 Hardware Overview

- **PCB Material:** FR4, 1.6mm, 0.35µm Cu  
- **Board Layers:** 2-layer design  
- **Main Blocks:**
  - Power supply & battery charging  
  - Biosignal AFE (EMG/ECG)  
  - Microcontroller control  
  - Bluetooth module  
  - LED indicators  

📖 Full schematic prints: [`docs/Minerva_Projrct.pdf`](docs/Minerva_Projrct.pdf)

---

## 📋 Bill of Materials (BOM)

See [`hardware/BOM.pdf`](hardware/BOM.pdf) for the full part list.  
Highlights include:

- **U1:** ADS1294IPAG – 4-ch 24-bit ADC  
- **U2:** ATmega1284P-MUR – 8-bit AVR MCU  
- **U3:** MMA8652FCR1 – 3-axis accelerometer  
- **U4:** IS31FL3199 – LED driver  
- **U5:** TPS78233 – LDO regulator  
- **U6:** MCP73831 – Li-ion charger  
- **U7:** NCP300L – voltage detector  

---

## 🛠️ Manufacturing

To order PCBs:

1. Use the **Gerber files** in `/gerbers` (or `/hardware/` folder).  
2. Upload to a PCB manufacturer (e.g., JLCPCB, PCBWay, OSH Park).  
3. Provide BOM to source components.  
4. Assemble manually or via pick-and-place.  

---

## 🚀 Getting Started

1. **Assemble the board** following the BOM.  
2. **Program the ATmega1284P** using ISP or bootloader (Arduino-compatible toolchains supported).  
3. **Power via Li-Ion battery or micro-USB**.  
4. **Connect via Bluetooth** to stream biosignals.  

---

## 📜 License

This project is released under the **CERN Open Hardware License v2**.  
You are free to **study, modify, produce, and distribute** this hardware, provided modifications and derivatives remain open.  

See [LICENSE](LICENSE) for details.

---

## 🤝 Contributing

Pull requests are welcome!  
You can help with:
- Firmware development examples  
- Better assembly guides  
- Testing & validation reports  
- Schematics migration to KiCad for broader accessibility  

---

## 📸 Gallery

*(Add board photos, assembled PCB pictures, or diagrams in `docs/README_assets/` and link them here.)*  

---

## 📧 Contact

Developed originally by **Ricardo Santos** (Portugal).  
Open-sourced by the community for further research and prototyping.  
