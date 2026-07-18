Arduino Nano Digital Temperature Monitor

This project uses an Arduino Nano, a DS18B20 digital temperature sensor, and a 16x2 HD44780 LCD display to create a simple real-time temperature monitoring system. The DS18B20 sensor measures ambient temperature and sends the data to the Arduino Nano through the OneWire communication protocol. The Nano processes the temperature reading and displays it on the LCD in degrees Celsius while also sending the data to the Serial Monitor for debugging and logging.

The system updates the temperature reading every second, providing accurate and reliable measurements suitable for home monitoring, weather stations, electronics projects, and educational demonstrations. The DS18B20 sensor offers high accuracy and digital noise immunity, making it an excellent choice for temperature sensing applications.

Features:

Real-time temperature measurement using the DS18B20 sensor
Temperature display on a 16x2 HD44780 LCD
Serial Monitor output for debugging and data logging
Updates every second
Simple and low-cost Arduino Nano project
Suitable for indoor temperature monitoring and learning about digital sensors

Components Used:

Arduino Nano
DS18B20 Digital Temperature Sensor
16x2 HD44780 LCD Display
4.7kΩ pull-up resistor (for DS18B20 data line)
Breadboard and jumper wires

This project demonstrates how to interface a digital temperature sensor with an Arduino and display live sensor data on a character LCD.

Components:    
Arduino Nano    DS18B20 Temperature Sensor    16x2 LCD Display    10kΩ Potentiometer (optional, for contrast adjustment)    4.7kΩ Resistor (for DS18B20 data line)    
Jumper Wires    BreadboardWiring Diagram:1. DS18B20 Sensor:    GND → Arduino Nano GND    VCC → Arduino Nano 5V    
Data Pin → Arduino Nano D8 (with a 4.7kΩ pull-up resistor between the data pin and VCC)2. LCD with 6 pins (using 4-bit mode):    
RS (Register Select) → Arduino Nano Pin 12    E (Enable) → Arduino Nano Pin 11    D4 → Arduino Nano Pin 5    D5 → Arduino Nano Pin 4    
D6 → Arduino Nano Pin 3    D7 → Arduino Nano Pin 2    VSS (GND) → Arduino Nano GND    VDD (Power) → Arduino Nano 5V    
Contrast (V0) → Middle pin of a 10kΩ potentiometer (connect the other two ends to GND and 5V)
1. Install Required Libraries:    OneWire: For communication with the DS18B20.    DallasTemperature: For reading temperature from the DS18B20.    LiquidCrystal: For handling the LCD display.
