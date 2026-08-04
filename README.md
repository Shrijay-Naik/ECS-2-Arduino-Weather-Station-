# 🌦️ Arduino Weather Station – ECS Project 2

A compact, real-time weather monitoring system designed to measure **temperature** and **humidity** using an Arduino-based embedded solution. The project also demonstrates **atmospheric pressure** and **light intensity** values for visualization purposes. The system provides instant weather updates on a **16×2 I2C LCD** and supports future scalability for IoT-based weather monitoring applications.

---

# 🚀 Features

## Core Functionality

- 🌡️ **Real-Time Temperature Monitoring** – Continuously measures ambient temperature using the DHT11 sensor.
- 💧 **Humidity Measurement** – Displays live humidity percentage.
- 📟 **LCD Display Output** – Shows weather parameters on a 16×2 I2C LCD.
- 🌤️ **Atmospheric Pressure Display** – Demonstrates atmospheric pressure values.
- ☀️ **Light Intensity Display** – Demonstrates ambient light intensity values.
- 🔄 **Scrolling Display** – Alternates between different weather parameters on the LCD.
- 📊 **Frontend Dashboard** – Displays weather data with graphs, history, notifications, and min/max tracking.
- 🎯 **Portable Design** – Powered using USB or an external 5V supply.

---

# 🛠️ Technology Stack

## Hardware

- **Microcontroller:** Arduino Uno
- **Sensor:** DHT11 Temperature & Humidity Sensor
- **Display:** 16×2 LCD with I2C Interface
- **Communication Module:** I2C Module
- **Power Supply:** USB Cable / 5V Adapter
- **Additional Components:** Breadboard, Jumper Wires

## Software

- **Programming Language:** Embedded C / Arduino C
- **IDE:** Arduino IDE 1.8.19

## Libraries Used

- `Wire.h`
- `LiquidCrystal_I2C.h`

---

# 📦 Installation & Setup

## Hardware Connections

| Component | Arduino Pin |
|-----------|-------------|
| DHT11 Data | Digital Pin 11 |
| DHT11 VCC | 5V |
| DHT11 GND | GND |
| LCD SDA | A4 |
| LCD SCL | A5 |
| LCD VCC | 5V |
| LCD GND | GND |

## Software Setup

1. Install Arduino IDE.
2. Install the `LiquidCrystal_I2C` library using Library Manager.
3. Connect the Arduino Uno using a USB cable.
4. Upload the Weather Station sketch.
5. Adjust LCD contrast using the I2C module potentiometer.

---

# 🧪 Working Principle

- The DHT11 sensor continuously measures **temperature** and **humidity**.
- Sensor data is transmitted to the Arduino Uno.
- The Arduino processes the readings and displays them on the LCD.
- The LCD alternates between:
  - Temperature & Humidity
  - Atmospheric Pressure & Light Intensity
- Atmospheric pressure and light intensity are currently displayed as demonstration values and can be replaced by dedicated sensors in future versions.
- A frontend dashboard visualizes the weather parameters with graphs, history, alerts, and statistics.

---

# 🏗️ System Architecture

```text
Environment
      │
      ▼
DHT11 Sensor
      │
      ▼
Arduino Uno
      │
      ▼
Data Processing
      │
      ▼
16×2 I2C LCD Display
      │
      ▼
Frontend Dashboard (Optional)
```

---

# 📊 Outcomes

- Successfully measured real-time temperature.
- Successfully measured humidity.
- Displayed atmospheric pressure values.
- Displayed light intensity values.
- Achieved smooth LCD scrolling.
- Successfully integrated Arduino with the LCD display.
- Developed a graphical dashboard for weather visualization.

---

# 🎯 Benefits

- ✅ Real-time weather monitoring
- ✅ Low-cost implementation
- ✅ Portable design
- ✅ Easy to operate
- ✅ Educational embedded systems project
- ✅ Expandable for IoT applications
- ✅ Interactive frontend dashboard

---

# 🧩 Testing & Troubleshooting

## Tests Conducted

- Temperature sensor testing
- Humidity sensor testing
- LCD readability testing
- LCD scrolling verification
- Power supply stability testing
- I2C communication testing

## Issues Resolved

- LCD displaying square boxes
- Low LCD brightness
- I2C address detection
- Arduino upload (COM Port) issues
- Library compatibility problems
- LCD contrast adjustment

---

# 🔮 Future Enhancements

- IoT integration using ESP8266/ESP32
- Cloud-based weather logging
- Android/mobile application
- Live analytics dashboard
- Rain sensor integration
- Wind speed monitoring
- BMP280/BME280 pressure sensor
- BH1750/LDR light sensor
- SMS/Email alerts
- GPS-based location tracking

---

# 📚 Learning Outcomes

- Arduino Programming
- Embedded C Programming
- DHT11 Sensor Interfacing
- LCD Interfacing
- I2C Communication
- Real-Time Data Acquisition
- Hardware–Software Integration
- Embedded System Debugging
- Frontend Data Visualization
- Team Collaboration

---

# 👨‍💻 Team Members

| Name | Registration Number |
|------|---------------------|
| **Shrijay Pramod Naik** | 23BCE8159 |
| **Smaran Thapliyal** | 23BCE8292 |
| **Aniruddh Dwivedi** | 23BCE8304 |
| **Dhrubajoti Das** | 23BCE8259 |
| **Vema Likith Datta Reddy** | 23BCE8311 |
| **Singanamala Faheem** | 23BEC7127 |

---

# 📄 Conclusion

The **Arduino Weather Station** successfully demonstrates a compact embedded system capable of monitoring environmental conditions in real time. The project measures **temperature** and **humidity** while demonstrating **atmospheric pressure** and **light intensity** for enhanced visualization. The Arduino Uno processes the sensor data and displays it on a **16×2 I2C LCD**, while an optional frontend dashboard provides graphical visualization, historical trends, notifications, and min/max tracking. The project offers a strong foundation for embedded systems learning and can be extended with IoT connectivity, cloud integration, additional sensors, and mobile applications for smart environmental monitoring.

---

## 📜 License

This project is developed as part of **ECS Project 2** for educational purposes.

---
**Made with ❤️ using Arduino Uno**
