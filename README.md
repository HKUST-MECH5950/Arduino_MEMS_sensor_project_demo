# Arduino Sensors using Omron D6T Non-contact Thermal MEMS sensor array 
This repository provides sample projects for integrating **OMRON D6T MEMS Thermal Sensors** with the evaluation kits **2JCIE-EV01-AR1**, **2JCIE-EV01-FT1**, and various Arduino boards.

**How the Omron D6T Sensor Works: From First Principles**
The Omron D6T MEMS Thermal Sensor is an advanced non-contact temperature sensor that detects the surface temperature of objects or stationary human presence. Its operation is rooted in the first principle of heat transfer—the concept that all objects emit **thermal radiation** proportional to their temperature.

The **D6T sensor series** enables high-sensitivity detection, including the ability to sense stationary human presence. This is achieved through:

- **OMRON's unique MEMS and ASIC technology** for high Signal-to-Noise Ratio (SNR).
- **Superior noise immunity** with a digital output interface.
- **High-precision area temperature detection** with minimal cross-talk field-of-view characteristics.
---
## Features
- Supports multiple D6T sensor types and pixel configurations.
- Compatible with Arduino boards like the **MKR WiFi 1010** and **Adafruit Feather ESP32**.
- Outputs sensor data to USB-Serial ports for easy monitoring.
---
## Description
This project provides Arduino sample code for acquiring and displaying sensor data from OMRON D6T thermal sensors using the 2JCIE-EV01 evaluation kits. Each example outputs data in a readable format via USB-Serial.
### Supported Configurations

| **Example** | **Sensor Type**            | **Pixel Configuration** | **Supported Boards**                           |
|:-----------:|:---------------------------|:------------------------:|:----------------------------------------------:|
| `d6t-1a`    | D6T-1A-01 / D6T-1A-02      | 1x1                     | Arduino MKR WiFi 1010 / Adafruit Feather ESP32 |
| `d6t-8l`    | D6T-8L-09                  | 1x8                     | Arduino MKR WiFi 1010 / Adafruit Feather ESP32 |
| `d6t-8lh`   | D6T-8L-09H                 | 1x8                     | Arduino MKR WiFi 1010 / Adafruit Feather ESP32 |
| `d6t-44l`   | D6T-44L-06 / D6T-44L-06H   | 4x4                     | Arduino MKR WiFi 1010 / Adafruit Feather ESP32 |
| `d6t-32l`   | D6T-32L-01A                | 32x32                   | Arduino MKR WiFi 1010 / Adafruit Feather ESP32 |

## DEMO Output
Below is a sample output for the **D6T-32L** sensor. The data includes the PTAT (Proportional To Absolute Temperature) value followed by an array of pixel temperatures in degrees Celsius.

```
17:55:54.514 -> PTAT:35.4
17:55:54.514 -> 24.0,26.6,25.1,24.9,25.7,25.9,25.0,25.5,25.4,26.8,25.5,25.4,24.1,25.3,25.6,25.2,25.0,25.2,24.2,24.2,25.1,25.4,23.2,26.1,26.4,25.3,27.3,26.4,24.4,26.8,23.4,22.0 [degC]
17:55:54.514 -> 26.7,26.5,26.6,25.1,26.5,26.2,25.8,25.0,26.2,25.7,26.8,25.5,24.1,25.6,25.6,25.3,25.1,25.3,24.2,24.5,25.0,23.2,23.9,24.1,25.4,27.3,24.8,25.8,26.8,23.4,25.1,23.1 [degC]
17:55:54.514 -> 26.4,26.7,26.5,26.0,27.0,26.2,26.2,26.2,26.6,25.8,25.9,25.8,26.9,26.3,26.8,25.6,25.6,25.9,25.4,25.4,24.8,23.9,24.1,25.3,25.8,24.8,26.0,25.2,26.9,25.2,23.1,24.6 [degC]

```

## Installation
see `https://www.arduino.cc/en/guide/libraries`

### Install from Arduino IDE
1. download .zip from this repo [releases](releases)
    or [master](archive/master.zip) .
2. Import the zip from Arduino IDE

    ![install-ide-import-lib](https://user-images.githubusercontent.com/48547675/55043017-9a34e980-5077-11e9-885d-03f9f82e3491.JPG)

    ![install-select-zip](https://user-images.githubusercontent.com/48547675/55043034-a7ea6f00-5077-11e9-99d5-26423fb652b5.JPG)

3. Then, you can see the samples in `File >> Examples` menu.

    ![install-select-examples](https://user-images.githubusercontent.com/48547675/55043028-a28d2480-5077-11e9-8365-6745cda417ff.JPG)

4. Select examples for your favorite sensors, build and program to boards.

### Manual install
1. download this repo

    ```shell
    $ git clone https://github.com/omron-devhub/d6t-2jcieev01-arduino
    ```

2. launch Arduino-IDE and select our sketch to load.
3. build and program to boards.


## Dependencies
None

## Links
- [Arduino samples for 2JCIE-01-AR1/FT1](https://github.com/omron-devhub/2jcieev01-arduino)
- [RaspberryPi samples for 2JCIE-01-RP1](https://github.com/omron-devhub/2jcieev01-raspberrypi)
- [RaspberryPi sample for D6T on 2JCIE-01-RP1](https://github.com/omron-devhub/d6t-2jcieev01-raspberrypi)
- [Arduino sample for D6F on 2JCIE-01-AR1/FT1](https://github.com/omron-devhub/d6f-2jcieev01-arduino)
- [RaspberryPi sample for D6F on 2JCIE-01-RP1](https://github.com/omron-devhub/d6f-2jcieev01-raspberrypi)
- [Arduino sample for B5W on 2JCIE-01-AR1/FT1](https://github.com/omron-devhub/b5w-2jcieev01-arduino)

projects by another authors.

- [d6t-grove-tinkerboard project](https://github.com/omron-devhub/d6t-grove-tinkerboard)
- [d6t-grove-m5stack project](https://github.com/omron-devhub/d6t-grove-m5stack)
- [d6t-grove-arduino project](https://github.com/omron-devhub/d6t-grove-arduino)  
    only for element 4x4 type, but libralized.

**References**
[OMRON D6T Datasheet ](url)

Licensed under the MIT License.

