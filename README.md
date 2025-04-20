# Arduino-AIr-Quality-Monitor
Arduino-based environment monitor that displays temperature, humidity, and air quality on an OLED screen.

# 1.Description
This Arduino project measures temperature, humidity, and air quality, then displays the data on an OLED screen. It uses a DHT22 sensor for temperature and humidity, an MQ135 sensor for air quality (CO2, NH3, benzene, etc.), and an I2C OLED display to show real-time data. The microcontroller used is the Arduino Nano.

# 2.Components Used
- Arduino Nano
- DHT22(Temperature and Humidity Sensor)
- MQ135 (Air Quality Sensor)
- 0.96" I2C OLED Display (SSD1306)

# 3.How It Works
- The *DHT22 sensor* reads the temperature and humidity and sends the data to the Arduino.
- The *MQ135 sensor* provides analog readings of air quality.
- The *OLED display* is connected via I2C (SCL to A5, SDA to A4), and shows:
  - Temperature in Celsius
  - Humidity in %
  - Air quality level (raw analog value)
- The Arduino continuously reads all sensor data, formats it, and updates the screen every second.

# 4.Project outline
![Project outline](https://github.com/Akez76/Arduino-AIr-Quality-Monitor/blob/main/AIr%20n1.jpeg)

# 5.Wiring Summary
| Component     | Arduino Pin |
|---------------|-------------|
| DHT22 Data    | D2          |
| DHT22 VCC     | 5V          |
| DHT22 GND     | GND         |
| MQ135 Analog  | A0          |
| MQ135 VCC     | 5V          |
| MQ135 GND     | GND         |
| OLED VCC      | 5V          |
| OLED GND      | GND         |
| OLED SDA      | A4          |
| OLED SCL      | A5          |      


# 6.Photos
![Air Quality Monitor](https://github.com.jpg)

# 7.Skills Used / Learned
- Sensor integration (DHT22 and MQ135)
- OLED display via I2C
- Arduino programming (C++)
- Real-time data monitoring

# Author:
Akezhan Kurbanov
