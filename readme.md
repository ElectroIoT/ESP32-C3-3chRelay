# 🔌 ESP32-C3 SuperMini 3-Channel Smart Relay Board

![PCB](assets/PCB.JPG)
![3D](assets/PCB_3D.JPG)

---

## 🧠 Overview

This DIY project is a **3-channel relay module** based on the **ESP32-C3 SuperMini**, perfect for controlling home appliances like **lights, fans, or AC sockets** over Wi-Fi using **Tasmota** firmware. It also supports **I2C sensors** like DHT11 or BMP280, enabling **environment-based smart switching**.

---

## 🧩 Key Features

✅ **3 Relay Outputs** (AC/DC load control)  
✅ **ESP32-C3 SuperMini** with Wi-Fi & BLE  
✅ **Tasmota Compatible** (Web UI + MQTT support)  
✅ **Voice Control** via **Alexa** and **Google Home**  
✅ **Onboard 5V Regulator** (220V AC via Hi-Link)  
✅ **I2C Expansion Header** for DHT11/BMP280/BH1750  
✅ **Power & Relay Status LEDs**  
✅ **Compact and reliable PCB layout**

---

## 🔧 Hardware Used

| Component                | Quantity |
|--------------------------|----------|
| ESP32-C3 SuperMini       | 1        |
| SRD-05VDC-SL-C Relays    | 3        |
| Hi-Link HLK-PM01 (5V)    | 1        |
| 7805 Voltage Regulator   | 1        |
| 1N4007 Diodes            | 3        |
| BC547 Transistors        | 3        |
| 10k Resistors, LEDs      | 3+       |
| Screw Terminals          | 5        |
| I2C Header (3-pin)       | 1        |
| DC Jack (optional)       | 1        |

---

## ⚙️ Schematic Design

📷 *Schematic Preview:*  
![Schematic](assets/Schematic_ESP32-C3-SUPERMini-3ch-relay.png)

### 🧾 Includes:

- Transistor driver circuits for each relay  
- Flyback diodes to protect against spikes  
- 7805 linear regulator for 9–12V DC input  
- Hi-Link 5V AC–DC module for direct 220V input  
- I2C breakout header for sensor expansion  

---

## 🖥️ PCB Layout and 3D Preview

### 🟨 Top View:
![PCB Top](assets/PCB.JPG)

### 🔵 3D Model:
![3D View](assets/PCB_3D.JPG)

### ✅ Design Highlights:
- Safe **AC/relay isolation**
- Clearly labeled terminals
- **Mounting area** for ESP32-C3 SuperMini
- Indicator LEDs for **power and relay status**

---

## 🌐 Firmware: Tasmota

This board is **100% compatible with Tasmota** for ESP32-C3.

### 🔌 GPIO Configuration:

| Function     | GPIO   |
|--------------|--------|
| Relay1       | GPIO10 |
| Relay2       | GPIO3  |
| Relay3       | GPIO21 |
| I2C SDA      | GPIO4  |
| I2C SCL      | GPIO5  |

### 🔧 Steps to Flash:

1. Use [Tasmota Web Installer](https://tasmota.github.io/install/)
2. Select `tasmota32c3.factory.bin`
3. Connect ESP32-C3 in boot mode and flash
4. Open Tasmota Web UI and configure the GPIOs
5. Connect Wi-Fi and control via **Web, MQTT, Alexa, or Google**

---

## 🌡️ Add-ons via I2C

Plug in I2C sensors to the 3-pin header:

| Sensor       | Function                  |
|--------------|---------------------------|
| DHT11/DHT22  | Temperature & Humidity    |
| BH1750       | Light Intensity           |
| BMP280/BME280| Temp / Pressure / Humidity|

Configure them in Tasmota's Web UI.

---

## 💡 Use Cases

- Turn **lights, fans, pumps** on/off remotely
- Automate switching based on **temperature or humidity**
- Integrate with **Home Assistant**, **Node-RED**, or **openHAB**
- Enable **voice control** via Alexa or Google Home

---

## 🛠️ Build Tips

- ✅ Maintain **isolation** between AC and low-voltage circuits
- ✅ Use **heat shrink** on exposed AC terminals
- ✅ Double-check Hi-Link input/output polarity
- ✅ Always **test with a multimeter** before applying AC power
- ✅ Add a **fuse** or varistor for additional safety

---
## 🙌 Credits

Designed with ❤️ by **ElectroIOT**  
Made to empower DIYers and smart home enthusiasts

Stay tuned on our channel:
- [YouTube - ElectroIoT](https://www.youtube.com/ElectroIoT)

## 🌐 More Projects

- Website: [https://electroiot.in](https://electroiot.in)
- GitHub: [ElectroIoT](https://github.com/ElectroIoT)

---

## 🙏 Special Thanks

A big thank you to the following platforms for their amazing tools and support in designing this open-source hardware project:

<p align="center">
  <img src="Image/EasyEDA.png" alt="EasyEDA Logo" width="100"/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
  <img src="Image/OSHWLab.png" alt="OSHWLab Logo" width="100"/>
</p>

- **[EasyEDA](https://easyeda.com/)** – for their powerful PCB design tools  
- **[OSHWLab](https://oshwlab.com/)** – for hosting open-source hardware projects

Their platforms made this project possible and easy to share with the maker community ❤️

## 📬 License

Open Source Hardware — OSHWA Certified

---

Happy Making! 💡
