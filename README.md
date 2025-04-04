# Arduino-Rocket-Transmitter-Library
A short library for SpaceFish members or engineers to use in the OrionX OS V1.0 Galileo rocket

# Arduino Rocket Transmitter Library

## Overview

When using the code, make sure to use the C++ file or use the Micropython Lab as this is designed for Arduino not a Pyboardvbut at request I will make a pyboard modified code.
The Arduino Rocket Transmitter Library is designed specifically for SpaceFish members and engineers working on the OrionX OS V1.0 Galileo rocket. This library provides essential functionalities for transmitting data from the rocket to ground stations, ensuring reliable communication and telemetry during rocket launches and operations.

## Features

- **Data Transmission**: Reliable data transmission from the rocket to ground stations.
- **Telemetry**: Real-time telemetry data for monitoring rocket status.
- **Compatibility**: Compatible with various Arduino boards and modules.
- **Compliance**: Adheres to EU standards for radio communication and electronic devices.

## Installation

1. **Download the Library**: You can download the latest version of the library from the GitHub repository. https://github.com/lukeandwoofy/Arduino-Rocket-Transmitter-Library. 
2. **Add to Arduino IDE**:
   - Open the Arduino IDE.
   - Go to `Sketch` > `Include Library` > `Add .ZIP Library`.
   - Select the downloaded ZIP file to add the library to the Arduino IDE.

## Usage

Here is a basic example to get started with the Arduino Rocket Transmitter Library:

```cpp
#include <RocketTransmitter.h>

RocketTransmitter rocketTransmitter;

void setup() {
    Serial.begin(9600);
    rocketTransmitter.initialize();
}

void loop() {
    rocketTransmitter.transmitTelemetry();
    delay(1000); // Transmit data every second
}
