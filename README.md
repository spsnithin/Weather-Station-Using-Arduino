🌦️ Weather Station using BMP180 and DHT11 
📌 Overview
This project is a basic weather monitoring system built using an Arduino UNO, BMP180 barometric pressure sensor, DHT11 temperature and humidity sensor, and a 16x2 I2C LCD display. It continuously displays:

Ambient temperature (from both DHT11 and BMP180)

Humidity (from DHT11)

Atmospheric pressure (from BMP180)

This real-time data is useful for learning about sensors and IoT applications.

🛠️ Components Required
Component	Quantity	Description
Arduino UNO	1	Microcontroller board
DHT11	1	Digital Temperature & Humidity Sensor
BMP180	1	Barometric Pressure and Temperature Sensor
I2C LCD (16x2)	1	For displaying output
Jumper Wires	10+	Male-to-Female and Male-to-Male
Breadboard	1	For prototyping

🔌 Circuit Connections
🟦 DHT11 Sensor
Pin	Arduino Pin
VCC	5V
GND	GND
Data	D2

🔷 BMP180 Sensor (I2C)
Pin	Arduino Pin
VCC	3.3V
GND	GND
SDA	A4
SCL	A5

🟩 I2C LCD
Pin	Arduino Pin
VCC	5V
GND	GND
SDA	A4
SCL	A5

⚙️ Functionality
DHT11 measures temperature and humidity.

BMP180 measures barometric pressure and temperature.

LCD displays the values in a clean two-line format.

Example LCD Output:

makefile
Copy code
Temp:25.0C Hum:60%
Pres:1005.2hPa
💻 Code Features
Uses Adafruit_BMP085 library for BMP180

Uses DHT library for DHT11

Uses LiquidCrystal_I2C library for the LCD

All sensor values are printed to both Serial Monitor and LCD

📚 Learning Outcomes
Interfacing multiple sensors with Arduino

Using I2C for LCD and sensors

Reading and displaying sensor data

Understanding basic weather parameters

✅ Future Improvements
Add SD card logging

Add WiFi (ESP8266/ESP32) for IoT cloud integration

Use OLED/TFT for better visuals

Build a case or enclosure

