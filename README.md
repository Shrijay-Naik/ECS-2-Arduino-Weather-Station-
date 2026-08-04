🌦️ Arduino Weather Station – ECS Project 1

A compact, real-time weather monitoring system designed to measure temperature and humidity using an Arduino-based embedded solution. The project also demonstrates atmospheric pressure and light intensity values for visualization purposes. The system provides instant weather updates on a 16×2 I2C LCD and supports future scalability for IoT-based weather monitoring applications.

🚀 Features
Core Functionality
🌡️ Real-Time Temperature Monitoring: Continuously measures ambient temperature using the DHT11 sensor.
💧 Humidity Measurement: Displays live humidity percentage.
📟 LCD Display Output: Shows weather parameters on a 16×2 I2C LCD.
🌤️ Pressure Display: Demonstrates atmospheric pressure values.
☀️ Light Intensity Display: Demonstrates ambient light intensity values.
🔄 Scrolling Display: Alternates between different weather parameters on the LCD.
🎯 Portable Design: Lightweight and powered directly through USB or an external 5V supply.
📊 Frontend Dashboard: Supports graphical visualization of weather parameters with history tracking.
🛠️ Technology Stack
Hardware
Microcontroller: Arduino Uno
Sensor: DHT11 Temperature & Humidity Sensor
Display: 16×2 LCD with I2C Interface
Communication Module: I2C Module
Power Supply: USB Cable / 5V Adapter
Additional Components: Breadboard, Jumper Wires
Software
Programming Language: Embedded C / Arduino C
IDE: Arduino IDE 1.8.19 or later
Libraries Used
LiquidCrystal_I2C.h
Wire.h
📦 Installation & Setup
Hardware Connections
DHT11 Data Pin → Arduino Digital Pin 11
DHT11 VCC → 5V
DHT11 GND → GND
LCD SDA → Arduino A4
LCD SCL → Arduino A5
LCD VCC → 5V
LCD GND → GND
Software Setup
Install Arduino IDE.
Install the LiquidCrystal_I2C library using Library Manager.
Connect the Arduino Uno to the computer using a USB cable.
Upload the Weather Station program.
Adjust the LCD contrast using the potentiometer on the I2C module.
Open the Serial Monitor if debugging is required.
🧪 Working Principle
The DHT11 sensor continuously measures the surrounding temperature and humidity.
The sensor sends digital data to the Arduino Uno.
The Arduino processes the received values and displays them on the LCD.
The display alternates between:
Temperature & Humidity
Atmospheric Pressure & Light Intensity
Atmospheric pressure and light intensity are currently displayed as demonstration values and can later be replaced with dedicated sensors.
The frontend dashboard visualizes all collected weather parameters with charts, history, notifications, and min/max tracking.
🏗️ System Architecture
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
📊 Outcomes
Successfully measured real-time temperature.
Successfully measured humidity.
Displayed atmospheric pressure values.
Displayed light intensity values.
Achieved smooth LCD scrolling between weather parameters.
Successfully integrated the Arduino with the LCD display.
Demonstrated a graphical weather dashboard for visualization.
🎯 Benefits
✅ Real-time weather monitoring
✅ Low-cost implementation
✅ Easy to understand and operate
✅ Portable and compact design
✅ Educational project for embedded systems
✅ Expandable for IoT applications
✅ Interactive dashboard with graphs and notifications
🧩 Testing & Troubleshooting
Tests Conducted
Temperature sensor testing
Humidity sensor testing
LCD readability test
LCD scrolling verification
Power supply stability test
I2C communication test
Issues Resolved
Incorrect I2C address detection
LCD displaying only square boxes
Low LCD brightness adjustment
COM port upload errors
Library compatibility issues
LCD contrast adjustment using potentiometer
🔮 Future Enhancements
🌐 IoT integration using ESP8266/ESP32
☁️ Cloud-based weather data storage
📱 Android application support
📈 Live weather analytics dashboard
🌧️ Rainfall sensor integration
🌬️ Wind speed sensor integration
🌡️ Actual atmospheric pressure measurement using BMP280/BME280
☀️ Actual light intensity measurement using BH1750 or LDR
🔔 SMS and Email weather alerts
📍 GPS-based location tracking
📚 Learning Outcomes
Arduino programming
Embedded C programming
DHT11 sensor interfacing
I2C communication protocol
LCD interfacing
Real-time data acquisition
Hardware–software integration
Embedded system debugging
Frontend visualization of sensor data
Team-based project development
👨‍💻 Team Members
Shrijay Pramod Naik – 23BCE8159
Smaran Thapliyal – 23BCE8292
Aniruddh Dwivedi – 23BCE8304
Dhrubajoti Das – 23BCE8259
Vema Likith Datta Reddy – 23BCE8311
Singanamala Faheem – 23BEC7127
📄 Conclusion

The Arduino Weather Station successfully demonstrates a compact and efficient embedded system for real-time environmental monitoring. The project accurately measures temperature and humidity while also demonstrating atmospheric pressure and light intensity values for enhanced visualization. The Arduino Uno processes sensor data and displays it on a 16×2 I2C LCD, while the frontend dashboard provides graphical representation, history tracking, notifications, and trend analysis. The project offers an excellent foundation for learning embedded systems and can be further enhanced with actual pressure and light sensors, IoT connectivity, cloud storage, and mobile applications, making it suitable for smart agriculture, environmental monitoring, and educational purposes.
