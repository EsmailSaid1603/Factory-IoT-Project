# ESP32 DevKit V1 Documentation

## Overview
The ESP32 DevKit V1 is a powerful development board based on Espressif's ESP32 microcontroller. It features integrated Wi-Fi and Bluetooth connectivity, making it ideal for IoT applications such as air quality monitoring and sensor interfacing. This board is widely used in both hobbyist and professional projects due to its versatility and performance.

## Key Features
- **Processor:** Dual-core Tensilica LX6, up to 240MHz
- **Memory:** Typically 4MB flash memory (model-dependent)
- **Connectivity:** 
  - Wi-Fi 802.11 b/g/n
  - Bluetooth v4.2 (Classic and BLE)
- **GPIOs:** Multiple digital I/O pins, analog inputs, PWM outputs, and communication interfaces (UART, SPI, I2C)
- **USB-to-Serial Converter:** Facilitates programming and debugging
- **Operating Voltage:** 3.3V logic (ensure compatibility with peripherals)

## Specifications
- **Processor:** Dual-core 32-bit LX6 microprocessor
- **Clock Speed:** Up to 240MHz
- **Flash Memory:** 4MB (or as specified by your particular board version)
- **SRAM:** Approximately 520KB
- **Connectivity:** Integrated Wi-Fi and Bluetooth
- **Power Supply:** Can be powered via USB or an external 3.3V supply (with proper voltage regulation)

## Pin Layout & Wiring
The ESP32 DevKit V1 provides numerous GPIO pins that are used to interface with sensors and other peripherals. In this project, for example:
- **Analog Readings:** The MQ sensors are connected to the analog-capable pins.
- **Digital I/O:** Used for sensor control and status indications.

For detailed wiring information, refer to the [Wiring Diagram](../docs/wiring_diagram.png) in the `docs/` folder.

## Setup Instructions
1. **Install the Arduino IDE:**  
   Download and install from the [Arduino website](https://www.arduino.cc/en/software).

2. **Install ESP32 Board Support:**  
   - Open Arduino IDE and go to **File > Preferences**.
   - In the **Additional Boards Manager URLs** field, add:  
     `https://raw.githubusercontent.com/espressif/arduino-esp32/gh-pages/package_esp32_index.json`
   - Go to **Tools > Board > Boards Manager**, search for **ESP32**, and install the package.

3. **Configure the Arduino IDE:**  
   - Select **Tools > Board > ESP32 Dev Module**.
   - Choose the correct COM port under **Tools > Port**.

4. **Upload Your Sketch:**  
   - Open your project code (e.g., the `main.ino` in the `code/` folder).
   - Click **Upload** and use the Serial Monitor to verify the output.

## Additional Resources
- [Espressif ESP32 Official Website](https://www.espressif.com/en/products/socs/esp32)
- [ESP32 Datasheet](https://www.espressif.com/sites/default/files/documentation/esp32_datasheet_en.pdf)
- [ESP32 Arduino Core GitHub Repository](https://github.com/espressif/arduino-esp32)

## Conclusion
The ESP32 DevKit V1 is an excellent platform for developing IoT projects. Its robust processing power, integrated connectivity, and rich set of features make it a reliable choice for sensor-based applications and more. Use this document as a reference for understanding the board’s capabilities and for setting up your development environment.
