# 🦝 RACCOON: The Ultimate ESP8266 MultiTool

> Unlocking the **full potential** of the ESP8266 with an all-in-one, budget-friendly toolkit for WiFi, IR, and RF hacking — plus games and OTA updates.  

---

## 🚀 Features

### 🌐 WiFi Attacks
- **Deauth Attack** – Fast and effective network disconnection  
- **Beacon Flood** – Flood the airwaves with fake networks  
- **Deauth Flood** – Disrupt multiple devices simultaneously  

### 📡 IR Attacks
- **TV-B-Gone** – Turn off most TVs with a single click  
- **IR Jammer** – Block standard infrared communication  
- **ProjectorGone** – Target projector systems for shutdown  

### 📻 433MHz Attacks
- **Jammer** – Block signals on the 433 MHz frequency  
- **BruteForce** – Attempt control code brute-forcing  
- **Custom Code Sender** – Transmit your own signals  

### 🎮 Games & Fun
- 🐤 **Flappy Bird**  
- ⚽ **Ping Ball**  
- 🐍 **Snake**  
- ❌⭕ **Tic Tac Toe**

### 🧠 Bonus Features
- **OTA (Over-the-Air) Updates**  
- **Sleep Mode Support**  
- **Flipper Zero-style animations**  
- **Custom UI & Animations**  

---

## 🛠️ Wiring & Pinout

### 📌 ESP8266 Pinout
![ESP8266 Pinout](https://github.com/user-attachments/assets/e1b7faf9-27c6-490c-99c0-0af797f61002)

---

### 📺 OLED Display  
| Pin   | GPIO | Note     |
|-------|------|----------|
| SDA   | 4    | Data     |
| SCL   | 5    | Clock    |
| VCC   | —    | 3.3V / 5V |
| GND   | —    | Ground   |

---

### 🔘 Buttons  
| Action | GPIO |
|--------|------|
| Up     | 14   |
| Down   | 12   |
| Select | 13   |

---

### 📀 IR LED  
![IR LED](https://github.com/user-attachments/assets/782368fe-18b2-45e9-a29c-d174afcab2f9)  
- **VCC** = 3.3V / 5V  
- **GND** = GND  
- **Signal** = GPIO 15  

ℹ️ Use the same IR LED diagram from the *PoisonBerry* project, just change the GPIO.

---

### 📡 433 MHz Transmitter
- **Signal** = GPIO 0  
- **VCC** = 3.3V / 5V  
- **GND** = GND  

---

## 💾 Flashing RACCOON to ESP8266

### Step-by-step using NodeMCU Flasher:

1. Open the correct version of NodeMCU Flasher for your OS (32/64-bit)  
2. Select the **COM port** from Device Manager  
3. In the **Advanced** tab, set SPI Mode to `DOUT`  
4. In the **Config** tab, select the `.bin` file  
5. Go to **Operation** and click **Flash**  
6. Once done, reset the ESP8266  

> 📸 Visual Guide:  
> ![Flashing Steps](https://github.com/user-attachments/assets/e476ccc7-1d8c-4cff-8fe8-2f64e09590bf)

---

## 📡 OTA (Over-the-Air) Update Guide

### 🔧 Setup Instructions

1. Create a folder named `OTA`  
2. Inside `OTA`, create a file named `version` and write the version (e.g. `1.7`)  
3. Place the new `.bin` firmware file in the `OTA` folder  
4. Start a local server using Python:
   ```bash
   cd Desktop/OTA
   python -m http.server 80


📸 Example:
![OTA Python Server](https://github.com/user-attachments/assets/6a345ee6-0c60-456b-9cca-38feeee44152)

---

### 📱 Device-Side Update

1. Go to: `Settings` → `Update` → `Select`
2. Connect to your **WiFi** (must be open/no password)
3. Enter your **PC’s IP address** when prompted
4. Your device will start updating!

⚠️ Ensure no other WiFi networks are interfering in the area.
💡 That's it! You're OTA-updated.

---

## 📷 Preview

![Screenshot](https://github.com/user-attachments/assets/d0ca6ab5-a11d-41ea-bf0c-da73c878aca6)

---

## 🔗 Follow for Updates

📸 Instagram: [@ashwin\_hhhhh](https://www.instagram.com/ashwin_hhhhh)

---

## 📜 License

MIT License – Feel free to use, modify, and contribute responsibly.

```

---

Let me know if you want a **dark-themed version**, emojis removed, or split into sections like `README.md`, `PINOUT.md`, etc.  
Also, I can create a **TOC (table of contents)** with anchor links if you're publishing this for a larger audience.
```
