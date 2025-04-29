**Do the connections as shown in the figure**
- **For Infrared (IR) Sensors**
  - You are using two IR obstacle detection sensors.
  - IR Sensor 1
    - VCC → Arduino 5V
    - GND → Arduino GND
    - OUT → Arduino Digital Pin 8

  - IR Sensor 2
    - VCC → Arduino 5V (shared with Sensor 1)
    - GND → Arduino GND (shared with Sensor 1)
    - OUT → Arduino Digital Pin 9

- **For Servo Motor**
  - VCC (Red Wire) → Arduino 5V
  - GND (Brown Wire) → Arduino GND
  - Signal (Orange/Yellow Wire) → Arduino Digital Pin 10

- **For 16x2 LCD Display (with I2C module)**
  - This LCD uses I2C communication, requiring only two data lines:
  - GND → Arduino GND
  - VCC → Arduino 5V
  - SDA → Arduino Analog Pin A4
  - SCL → Arduino Analog Pin A5

**After the Connections**
- Upload LCD16x2_I2C_Scanner Code by selecting Arduino Uno from boards and selecting the port where you have connected the wire
- Then Open Serial Monitor to get your Hexadecimal Code (I2C Address)
- Then in Car_Parking_System search for the Change Hex Address Comment and replace the Hex Address

- You can change the slots depending on your total parking space
