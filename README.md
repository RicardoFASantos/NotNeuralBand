## 🎥 Vintage Video gallery

### General Pre-trained gestures based on muscle and motion signals
[![Assembly Tutorial](https://img.youtube.com/vi/8NtrBwCGjhw/hqdefault.jpg)](https://www.youtube.com/watch?v=8NtrBwCGjhw)

### Assembly of a 3D printed bracelet with a PCB board and sensors
[![Assembly Tutorial](https://img.youtube.com/vi/L2T6ioK4wVY/hqdefault.jpg)](https://www.youtube.com/watch?v=L2T6ioK4wVY)

---

## ✨ Features

- **Analog Front-End:** TI ADS1294 – 4-channel, 24-bit ADC with integrated EMG front-end  
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
  - Biosignal AFE (EMG)  
  - Microcontroller control  
  - Bluetooth module  
  - LED indicators  

---

## 🛠️ Manufacturing

To order PCBs:

1. Use the **Gerber files** in `/hardware`.  
2. Upload to a PCB manufacturer (e.g., JLCPCB, PCBWay, OSH Park).  
3. Provide BOM to source components.  
4. Assemble manually or via pick-and-place.

---

## ⚠️ Design Notes

- This design uses a **virtual ground electrode** implementation.  
  No physical ground electrode is required for operation, as the ADS1294 reference (RLD) is internally stabilized.  
  This simplifies assembly and makes the device more wearable.  

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
- Migrating schematics into KiCad for wider community use  

---

## 📧 Contact

Developed originally by **Ricardo Santos** with his friends from college Andreia Dias, Dora Inácio, Eduardo e Rui Santos.
For questions, suggestions, or collaborations:  
- Email: ricardo.santos.eb@gmail.com 
- LinkedIn: [ricardofasantos](https://www.linkedin.com/in/ricardofasantos/)  
- Twitter/X: [@RicardoSan43564](https://twitter.com/RicardoSan43564)
Open-sourced by the community for further research and prototyping.  
