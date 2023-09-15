# DIY Cannabis Drying and Curing Chamber

## Overview

This project leverages the power of Arduino Uno to create a controlled environment for drying and curing cannabis. By maintaining precise temperature and humidity levels, this chamber ensures optimal preservation of terpenes and cannabinoids, leading to a superior end product.

## Features

- **Thermoelectric Cooler Control:** The Arduino Uno manages a relay switch to control the cooler, ensuring the temperature remains within the desired range.

- **Humidifier Control:** An external humidifier is controlled via a relay switch to maintain the desired humidity level inside the chamber.

- **Fan Speed Management:** Intake and exhaust fan speeds are dynamically adjusted based on the current humidity level.

- **Bluetooth Commands:** The system integrates an HC-05 Bluetooth module, allowing for remote management and monitoring.

- **Real-time Clock:** With the RTC_DS3231 module, the system tracks the drying and curing cycles' progression.

## Components

- **Arduino Uno**
- **DHT22 Temperature and Humidity Sensor**
- **HC-05 Bluetooth Module**
- **RTC_DS3231 Real-time Clock Module**
- **Relay Modules**
- **Thermoelectric Cooler**
- **Analog Humidifier**
- **Centrifugal Fans**

# Setup

### Thermoelectric Cooler

A thermoelectric cooler offers precise temperature control, crucial for preserving the quality of the cannabis during the drying and curing process.

### Humidifier

Ensure you use a simple analog humidifier with a manual on/off switch. This allows the relay to control it without complications.

### Centrifugal Fans

Centrifugal fans are recommended due to their orientation, which saves space inside the chamber and requires smaller ports.

### Arduino Uno

The heart of the system, the Arduino Uno, manages all the components and ensures they work in harmony.

## Wiring and Connections

- **Powering the Arduino:** The Arduino can be powered via a USB connection or an external power supply.

- **DHT22 Sensor:** Connect the sensor's data pin to A3 on the Arduino.

- **Relay Modules:** Wire the cooler and humidifier to their respective relay modules and connect them to the Arduino pins as defined in the code.

- **Centrifugal Fans:** These are powered independently using an external power supply. Connect the fans' power and ground pins to a +- dongle.

- **HC-05 Bluetooth Module:** Connect the RX and TX pins to pins 10 and 11 on the Arduino, respectively.

- **RTC_DS3231 Module:** Connect this module to the Arduino using the I2C pins.

## Chamber Modifications

- Use a jigsaw to cut ports for the centrifugal fans and to route the DHT22 sensor cables.

- Consider using 3D printed 90-degree pieces for the exterior intake fan.

- Silicon mats can be used for food-grade safe shelving inside the chamber.

## Software Setup

- Install the Arduino IDE.

- Load the provided code into the IDE.

- Upload the code to the Arduino.

## Contributing

Feel free to fork this repository and submit pull requests. Any contributions, whether it's refining the code or improving the hardware setup, are highly appreciated!
