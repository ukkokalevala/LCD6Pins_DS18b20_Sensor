Components:    
Arduino Nano    DS18B20 Temperature Sensor    16x2 LCD Display    10kΩ Potentiometer (optional, for contrast adjustment)    4.7kΩ Resistor (for DS18B20 data line)    
Jumper Wires    BreadboardWiring Diagram:1. DS18B20 Sensor:    GND → Arduino Nano GND    VCC → Arduino Nano 5V    
Data Pin → Arduino Nano D8 (with a 4.7kΩ pull-up resistor between the data pin and VCC)2. LCD with 6 pins (using 4-bit mode):    
RS (Register Select) → Arduino Nano Pin 12    E (Enable) → Arduino Nano Pin 11    D4 → Arduino Nano Pin 5    D5 → Arduino Nano Pin 4    
D6 → Arduino Nano Pin 3    D7 → Arduino Nano Pin 2    VSS (GND) → Arduino Nano GND    VDD (Power) → Arduino Nano 5V    
Contrast (V0) → Middle pin of a 10kΩ potentiometer (connect the other two ends to GND and 5V)
1. Install Required Libraries:    OneWire: For communication with the DS18B20.    DallasTemperature: For reading temperature from the DS18B20.    LiquidCrystal: For handling the LCD display.
