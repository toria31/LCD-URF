# LCDUltrasonicRangefinder
Ultrasonic rangefinder with LCD using Arduino Uno

Required Hardware and Components
--------------------------------
- Arduino Uno
- Ultrasonic Sensor
- LCD 16x2
- 10K Ohm Potentiometer 
- Breadboard
- Jumper Wires

Connections
-----------
Ultrasonic:
  - VCC to 5V
  - GND to GND
  - Trig to Arduino Digital Pin 8 
  - Echo to Arduino Digital pin 9

LCD:
  - VSS to GND
  - VDD to 5V
  - VO to 10K Ohm Potentiometer Center Pin
  - RS to Arduino digital pin 1
  - RW to GND
  - E to Arduino digital pin 2
  - D4 to Arduino digital pin 4
  - D5 to Arduino digital pin 5
  - D6 to Arduino digital pin 6
  - D7 to Arduino digital pin 7
  - A to 5V
  - K to GND

Formula Explanation
-------------------
(S = T * V)
-> distanceCm = duration * 0.034 / 2
  
- S = distanceCm
- T = duration
- V = sound speed (0.034)

NOTE. We are dividing result because when the ultra sound reaches the object, it reflects back on the same distance and distnace value is doubled.
