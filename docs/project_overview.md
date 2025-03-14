# Graduation Project: IoT-based Air Quality Monitoring System

## Introduction
Air quality monitoring in industrial and urban environments is critical to ensuring health and safety. This project leverages an ESP32 DevKit V1 in conjunction with MQ sensors (MQ-2 and MQ-135) to detect and monitor various gas levels. The system outputs sensor readings to a serial monitor, and it can be extended for real-time cloud integration.

## Objectives
- **Develop an IoT solution:** Build a system that continuously monitors air quality using readily available sensors.
- **Integrate Hardware and Software:** Interface MQ-2/MQ-135 sensors with the ESP32 for real-time data acquisition.
- **Provide Actionable Data:** Output sensor readings for immediate monitoring and potential data logging.

## System Overview
The system is comprised of the following key components:
- **ESP32 DevKit V1:** Acts as the central microcontroller, providing Wi-Fi and Bluetooth connectivity.
- **MQ-2/MQ-135 Sensors:** These sensors detect a range of gases. Their analog outputs are read by the ESP32.
- **Circuit and Wiring:** The sensors are connected to the ESP32 via its analog input pins. Refer to the wiring diagram for details.

## Hardware Components
- **ESP32 DevKit V1** – A versatile microcontroller with integrated Wi-Fi and Bluetooth.
- **MQ-135 Sensor** – Detects gases like CO₂, NH₃, and benzene.
- **MQ-2 Sensor** – Detects LPG, CO, and methane.
- Additional items such as a breadboard, jumper wires, and a power supply are required for assembly.

## Circuit Diagram
A detailed wiring diagram (`wiring_diagram.png`) is provided in this repository to illustrate how the ESP32 and sensors are interconnected. Make sure to review it before assembling the hardware.

## Software Implementation
The project includes a simple Arduino sketch (located in the `code/` folder) that reads sensor values and prints them to the Serial Monitor. This code can serve as a baseline for further development, such as integrating Wi-Fi connectivity or advanced sensor calibration.

## Testing & Results
- **Initial Testing:** The uploaded code successfully displays sensor readings on the Arduino Serial Monitor.
- **Observations:** The sensors provide a combined reading of gas concentration. Future improvements may involve better calibration to differentiate between gas types.

## Future Improvements
- **Data Logging:** Consider integrating data logging to an SD card or a cloud service.
- **Real-time Dashboard:** Develop a web or mobile dashboard for real-time monitoring.
- **Enhanced Calibration:** Implement more sophisticated calibration methods to isolate individual gas readings.

## Conclusion
This project demonstrates a cost-effective method for air quality monitoring using widely available sensors and a robust microcontroller. It serves as a foundation for more complex IoT applications in environmental monitoring.

## References
- [ESP32 DevKit V1 Datasheet](https://www.espressif.com/en/products/socs/esp32)
- [MQ-135 Sensor Datasheet](#)
- [MQ-2 Sensor Datasheet](#)
