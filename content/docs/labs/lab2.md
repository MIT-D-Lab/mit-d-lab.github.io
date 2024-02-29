---
title: Lab 2 — Sensors and Input Devices
next: lab3
---

Lab 2 (sensors and input devices)
- analog vs digital input
- ADCs and the concept of discretiation 
- nyquist and sampling frequency 
- familiarity with various sensors 
- basic moving average filters
- hardware filters such as RC filters and debounce **do a debounce filter!!!**
  - we will also use INTERRTUPTS here!!! 
- I2C, serial, and digital communications sensors
- calculate communications speed for data streamed to the computer or the cloud 


*Also learn to...*
- REMBER BACK TO READING 1 and RATINGS
- CHECK POLARITY AND CONTINUITY
- Read from a sensor and print to serial terminal (printing variables as well)
- Then print to serial plotter

**Calibration and TRUSTING your sensors!!!! --> how to know when you trust your sensor!**




### Lab Planning

Essentially THIS [Connecting Sensors](https://docs.arduino.cc/tutorials/mkr-wifi-1010/connecting-sensors/) but with more info.

- Types of GPIOs
  - analog 
  - INPUT PULLUP and PULLDOWN for digital input 
- At least (1x) analog sensor
  - manually reading an analog sensor with a multimeter
  - ADC discretization ( datatypes from AnalogRead() )
- At least (1x) button, an RC de-bounce filter (this IS a digital sensor)
  - this is the debounce circuit - show WITH and WITHOUT
- At least (1x) digital sensor, like an ENCODER, or I2C, or SPI sensor
  - Moving Average Filters (smoothing show WITH and WITHOUT)
- Samping and the Nyquist Frequency
  - How fast *should you read*
  - How fast *can you read*
  - (this is DIFFERENT for Analog and Digital)
- Techniques
  - Using an Analog Sensor with a Digital Input (automated thresholding) ???
  - Hardware filtering for analog sensors 
  - triggering **interrupts** with digital sensors
  - triggering **interrupts** with timers

### List of Sensors

*Environmental / Chemical / Water Quality*
- Ph Sensor
- CO2 Gas
- Electrical Conductivity 
- Formaldehyde Sensor
- Capacitive Soil Moisture Sensor
- Oxygen Sensor 
- Ozone Sensor
- Air Quality Sensor
- Barometer
- Dust Sensor
- Humidity Sensor (Air)
- Humidity Sensor (Soil)
- Oxidation Reduction Potential Sensors

*General*
- Liquid Level Sensor
- Accelerometer (3-6 Axis)
- IR Proximity Sensors
- Digital IR Temperature Sensor
- Hall (magnetic field) Sensor
- IR Emitter/Reciever Breakbeam
- Reflectivity Sensor
- Light Sensor
- Line Finder
- PIR Motion Sensor
- Sound Sensor
- Touch Sensor / Button
- Ultrasonic Distance Sensors

*Energy Sensors*
- Current Sensor
- Voltage Sensor

*Specialized Sensors Robotics*
- Guesture Sensor
- AI Machine Vision Sensor
- Microwave Motion Radar
- NFC/RFID Reader

*Switches and Joysticks*
- Thumb Joystick
- Potentiometer 
- Magnetic Switch 
- Momentary Switch 
- Pushbutton Switch
- Latching Switch 

*Specialzied Gas Sensors*
- Alcohol Breathalyzer Sensor
- Combustible Gas Sensor (MQ2/MQ3/MQ9)

*Specialized Interfaces (Shields)* 
- Display / Touchscreen 
- GPS Shields
- CAN Bus
- Ethernet
- Inertial Measurement Unit (IMU)
- SD Card 
- GSM/Cellular
- DAQ/ADC
- Signal Amplifiers
- etc.

*Places to Look for Sensors*
- [Adafruit](https://www.adafruit.com/category/35)
- [Seed Studio Grove](https://www.seeedstudio.com/category/Grove-c-1003.html)
- [DF Robot](https://www.dfrobot.com/topic-277-36.html)
- [DF Robot Shields](https://www.dfrobot.com/topic-277-156.html)
- [Environmental Monitoring - Arduino](https://store-usa.arduino.cc/collections/environment-monitoring)
- [Arduino Shields - Arduino](https://store-usa.arduino.cc/collections/shields-carriers)
- [Sensors - Arduino](https://store-usa.arduino.cc/collections/sensors)