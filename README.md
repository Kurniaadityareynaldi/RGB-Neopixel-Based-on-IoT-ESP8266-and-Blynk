# 🌈 IoT RGB LED Controller using ESP8266, WS2812B, and Blynk

An IoT-based RGB LED controller built with ESP8266 (NodeMCU), WS2812B NeoPixel LEDs, and Blynk. This project enables users to remotely control LED colors and animations through a smartphone application.

## ✨ Features

* 📱 Remote control using Blynk
* 🎨 RGB color selection
* 🔘 Push-button mode switching using interrupt
* 📟 LCD display via Blynk Widget LCD
* 🌈 Multiple LED animation effects
* 📡 WiFi-enabled IoT connectivity

---

## 🛠 Hardware Requirements

| Component        | Description          |
| ---------------- | -------------------- |
| NodeMCU ESP8266  | Main microcontroller |
| WS2812B NeoPixel | Addressable RGB LEDs |
| Push Button      | Mode switching       |
| Smartphone       | Blynk application    |
| WiFi Network     | IoT connectivity     |

---

## 📌 Pin Configuration

| Function         | GPIO        |
| ---------------- | ----------- |
| NeoPixel DIN     | GPIO15 (D8) |
| Button Interrupt | GPIO0 (D3)  |

---

## 🎨 Available LED Modes

| Mode | Description           |
| ---- | --------------------- |
| 0    | Manual RGB Control    |
| 1    | Theater Chase         |
| 2    | Color Wipe            |
| 3    | Rainbow               |
| 4    | Rainbow Cycle         |
| 5    | Theater Chase Rainbow |

Modes can be changed using the push button connected to the interrupt pin.

---

## 📱 Blynk Virtual Pins

| Virtual Pin | Function                |
| ----------- | ----------------------- |
| V0          | Red Value               |
| V1          | Green Value             |
| V2          | Blue Value              |
| V3          | RGB Color Picker        |
| V4          | Interrupt Configuration |
| V5          | LCD Widget              |

---

## 🚀 Installation

1. Install required libraries:

   * Blynk
   * Adafruit NeoPixel
   * ESP8266 Board Package

2. Replace the following credentials:

```cpp
#define BLYNK_AUTH_TOKEN "YOUR_TOKEN"

char ssid[] = "YOUR_WIFI";
char pass[] = "YOUR_PASSWORD";
```

3. Upload the code to your NodeMCU ESP8266.

4. Configure the Blynk dashboard according to the virtual pins listed above.

---

## 📂 Project Structure

```text
├── src/
│   └── main.ino
├── README.md
├── LICENSE
└── LICENSE-GPLv2
```

---

## ⚠️ Important Note

This project was developed using an older version of Blynk. Migration to the latest Blynk IoT platform may be required.

---

## 📜 License

This project is dual-licensed under:

* GNU General Public License v2 (GPLv2)
* Commercial License

See the LICENSE file for details.

---

## 👨‍💻 Author

Kurnia Aditya Reynaldi

Contributions, issues, and pull requests are welcome.
