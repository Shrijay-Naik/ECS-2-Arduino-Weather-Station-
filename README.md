🌤️ Arduino Weather Station – ECS Project 2

A compact, Arduino-based embedded weather monitoring system designed to measure and display essential environmental parameters in real time. The project monitors temperature, humidity, atmospheric pressure, and light intensity, providing users with an easy-to-understand interface for basic weather observation. Built using affordable hardware components, the system serves as a foundation for future smart weather monitoring and IoT-based environmental applications.

🚀 Features
Core Functionality
🌡️ Real-Time Temperature Monitoring

Continuously measures the ambient temperature using the DHT11 sensor and displays the value in degrees Celsius (°C).

💧 Humidity Detection

Measures the relative humidity of the surrounding environment and displays the percentage (%) in real time.

🌤️ Atmospheric Pressure Display

Displays atmospheric pressure values (in hPa) through software simulation, demonstrating the capability to integrate real pressure sensors such as the BMP280 in future versions.

☀️ Light Intensity Display

Displays light intensity values (in lux) using simulated data, illustrating the expandability of the weather station to support ambient light sensing through sensors such as an LDR or BH1750.

📟 LCD Display Interface

Displays all environmental parameters on a 16×2 I2C LCD with automatic switching between different parameter screens for improved readability.

🔄 Continuous Monitoring

The Arduino continuously reads environmental data and updates the display in real time, ensuring uninterrupted monitoring.

🔔 Alert Notifications (Software)

The system can generate notifications for abnormal weather conditions such as:

High Temperature
High Humidity
Low Atmospheric Pressure
Low Light Intensity
📊 Data Visualization Dashboard

A web-based frontend dashboard was developed to visualize weather parameters through:

Live parameter cards
Temperature vs Time graph
Humidity vs Time graph
Measurement history
Min–Max parameter tracking
Weather alerts
Live clock and location display
🛠️ Technology Stack
Hardware

Microcontroller

Arduino Uno (ATmega328P)

Sensor

DHT11 Temperature and Humidity Sensor

Display

16×2 LCD Display with I2C Interface

Communication

I2C Protocol (SDA & SCL)

Power Supply

USB Cable / 5V External Supply

Additional Components

Breadboard
Jumper Wires
USB Cable
Resistors (if required)
Software

Programming Language

Arduino C / Embedded C

Development Environment

Arduino IDE 1.8.19

Frontend

HTML5
CSS3
JavaScript
Chart.js (for graphical visualization)

Libraries Used

Wire.h
LiquidCrystal_I2C.h
📦 Installation & Setup
Hardware Connections
DHT11 Sensor
VCC → Arduino 5V
GND → Arduino GND
DATA → Digital Pin 11
LCD Display (I2C)
SDA → Arduino A4
SCL → Arduino A5
VCC → Arduino 5V
GND → Arduino GND
Software Setup
Install Arduino IDE.
Install the LiquidCrystal_I2C library using Library Manager.
Connect the Arduino Uno to the computer using a USB cable.
Upload the Weather Station program.
Adjust the LCD contrast using the potentiometer on the I2C module.
Open the Serial Monitor (optional) for debugging.
🧪 Working Principle

The DHT11 sensor continuously measures the surrounding temperature and humidity using its internal sensing elements.

The sensor transmits digital pulse signals to the Arduino Uno, where the program decodes the data, verifies it using checksum validation, and extracts the temperature and humidity values.

The processed data is then displayed on the 16×2 LCD through I2C communication.

In addition to sensor readings, the system also displays atmospheric pressure and light intensity values through software simulation, demonstrating how additional environmental sensors can be integrated into the weather station architecture.

The frontend dashboard further visualizes the collected information by presenting numerical values, graphical trends, measurement history, and weather notifications.

🏗️ System Architecture
                 Temperature
                 Humidity
                     │
                 DHT11 Sensor
                     │
            Digital Signal Output
                     │
             Arduino Uno (ATmega328P)
                     │
      ┌──────────────┼───────────────┐
      │                              │
      ▼                              ▼
16×2 I2C LCD Display        Frontend Dashboard
                                   │
        ┌───────────────┬───────────┴─────────────┐
        ▼               ▼                         ▼
 Parameter Cards   Line Graphs           History & Alerts
📊 Frontend Dashboard Features

The developed frontend dashboard provides an enhanced visualization of weather data.

Dashboard includes:
Live temperature display
Live humidity display
Atmospheric pressure display
Light intensity display
Live system clock
Current location indicator
Temperature vs Time graph
Humidity vs Time graph
Historical measurements
Minimum and maximum parameter tracking
Automatic weather notifications
📈 Outcomes
Successfully measured real-time temperature.
Successfully measured real-time humidity.
Displayed atmospheric pressure values.
Displayed light intensity values.
Successfully interfaced DHT11 with Arduino Uno.
Successfully interfaced I2C LCD with Arduino.
Developed an interactive weather dashboard.
Generated graphical visualization of weather trends.
Implemented notification-based weather monitoring.
Successfully maintained historical weather records.
🎯 Benefits
Real-Time Weather Monitoring

Provides continuous environmental monitoring.

Low Cost

Uses inexpensive hardware suitable for educational purposes.

Portable Design

Compact and lightweight for indoor or outdoor demonstrations.

Interactive Dashboard

Provides graphical visualization instead of simple numerical values.

Easy Expansion

Supports future integration of:

BMP280
LDR
BH1750
Rain Sensor
Wind Speed Sensor
ESP8266 Wi-Fi Module
Educational Value

Provides practical understanding of:

Embedded Systems
Sensor Interfacing
Arduino Programming
Data Visualization
Frontend Development
🧩 Testing & Troubleshooting
Tests Conducted
Sensor Testing

Verified temperature and humidity measurements under different environmental conditions.

LCD Testing

Verified character visibility and I2C communication.

Frontend Testing

Verified graph generation, history tracking, and notification system.

Power Testing

Ensured stable operation using USB power.

Issues Resolved
LCD showing only black boxes.
Incorrect I2C address detection.
Low LCD brightness adjustment.
DHT11 communication timing issues.
COM port detection during Arduino upload.
Library compatibility problems.
Frontend synchronization issues.
🔮 Future Enhancements
Integration of BMP280 for actual atmospheric pressure measurement.
Integration of BH1750 or LDR for actual light intensity measurement.
Rainfall sensing.
Wind speed measurement.
GPS-based automatic location detection.
IoT integration using ESP8266/ESP32.
Cloud-based weather data logging.
Mobile application support.
AI-based weather prediction using historical data.
Email/SMS alerts during extreme weather conditions.
📚 Learning Outcomes

Through this project, the team gained practical knowledge in:

Arduino programming
Embedded C programming
DHT11 sensor interfacing
I2C communication
LCD interfacing
Sensor data acquisition
Real-time embedded systems
Hardware debugging
Frontend dashboard development
Graphical data visualization
Weather monitoring concepts
Team collaboration and project management

👨‍💻 Team Members
•	Shrijay Pramod Naik – 23BCE8159 
•	Smaran Thapliyal – 23BCE8292 
•	Aniruddh Dwivedi – 23BCE8304 
•	Dhrubajoti Das – 23BCE8259 
•	Vema Likith Datta Reddy – 23BCE8311 
•	Singanamala Faheem – 23BEC7127

📄 Conclusion
The Arduino Weather Station project successfully demonstrates a reliable and user-friendly environmental monitoring system capable of displaying temperature, humidity, atmospheric pressure, and light intensity in real time. By combining embedded hardware with an interactive frontend dashboard, the project provides both numerical and graphical visualization of environmental data, making weather monitoring more intuitive and informative.

The project meets the objectives of developing a low-cost, portable, and scalable weather monitoring solution while providing hands-on experience in embedded systems, sensor interfacing, hardware–software integration, and data visualization. Its modular architecture also allows future integration of additional sensors, IoT connectivity, cloud-based analytics, and intelligent weather prediction, making it a strong foundation for advanced smart weather monitoring applications.
