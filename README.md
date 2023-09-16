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

- **Arduino Uno** The heart of the system, the Arduino Uno, manages all the components and ensures they work in harmony.
- **DHT22 Temperature and Humidity Sensor** The sensor responsible for monitoring temperature and humidity
- **HC-05 Bluetooth Module** The bluetooth module responsible for handling bluetooth commands
- **RTC_DS3231 Real-time Clock Module** The clock module that handles the cycle start times
- **Relay module or IOT power strip** The relay module or IOT power strip for controlling the cooler
- **Thermoelectric Cooler** A thermoelectric cooler offers precise temperature control, crucial for preserving the quality of the cannabis during the drying and curing process.
- **Analog Humidifier** Ensure you use a simple analog humidifier with a manual on/off switch. This allows the relay to control it without complications.
- **Centrifugal Fans** Centrifugal fans are recommended due to their orientation, which saves space inside the chamber and requires smaller ports.

# Step-by-Step Guide

## Powering the Arduino Uno
The Arduino Uno can be powered in multiple ways:
1. Via USB connection to a computer.
2. Using a 9-12V external power supply connected to its barrel jack.
3. Through the Vin pin using a regulated 7-12V.

## Preparing the Cooler
1. Mark the areas on the cooler where the fans and DHT22 sensor cables will be placed.
2. Using a jigsaw, carefully cut out the marked areas. Ensure you wear safety goggles and gloves.

## Fan Setup
1. The centrifugal fans should be powered independently using an external power supply.
2. Use a power supply with a +/- dongle. This allows for easy connection of multiple fan power and ground pins.
3. Ensure the fans' orientation is correct, with one serving as an intake and the other as an exhaust.

## Setting up the HC-05 and Real-Time Module
1. Place the HC-05 Bluetooth module and the real-time clock (RTC) module on your PCB (printed circuit board).
2. Follow the pinout diagrams for each module to ensure correct connections to the Arduino Uno.

## Wiring the Relay Module
1. The relay module serves as a switch, allowing the Arduino to control high-power devices like the cooler.
2. Wire the relay module to the cooler's power cable. Ensure the connections are secure and insulated.
3. Alternatively, you can use an IoT power strip to control the cooler, avoiding direct wiring. This might be preferable if you're hesitant about modifying the cooler.

## Additional Components
- Use silicone mats inside the cooler. They are food-grade safe and provide clean shelving for the cannabis.
- Depending on your setup, you might need a 3D printed 90-degree piece for the exterior intake fan to ensure efficient airflow.

# Setting Up the Arduino IDE
1. Download and install the Arduino IDE from the official Arduino website.
2. Connect the Arduino Uno to your computer using a USB cable.
3. Open the Arduino IDE, select the correct COM port, and choose "Arduino Uno" as the board.
4. Copy the provided code into the IDE.
5. Click on the upload button (arrow pointing right) to transfer the code to the Arduino.

**Note:** Always ensure that your connections are secure and insulated to prevent short circuits. It's also a good idea to test each component individually before integrating everything.

## Contributing

Feel free to fork this repository and submit pull requests. Any contributions, whether it's refining the code or improving the hardware setup, are highly appreciated!
