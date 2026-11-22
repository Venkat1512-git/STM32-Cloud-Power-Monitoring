# Cloud-Based Power and Condition Monitoring System

### Embedded Systems | STM32F407 | ESP32 | IoT

## Project Overview

This project focuses on developing an embedded monitoring system using the STM32F407 microcontroller and ESP32 Wi-Fi module.

The system is designed to monitor electrical parameters and environmental conditions, process sensor measurements, identify abnormal operating conditions and transmit monitoring data to a cloud-based platform.

## Hardware Components

| Component | Purpose |
|---|---|
| STM32F407G-DISC1 | Main microcontroller |
| ESP32 | Wireless communication |
| DHT11 | Temperature and humidity sensing |
| Voltage sensing circuit | Voltage measurement |
| Current sensing circuit | Current measurement |

## Software and Technologies

- Embedded C
- STM32CubeIDE
- STM32CubeMX
- STM32 HAL Library
- ADC
- UART communication
- GPIO programming
- JSON data formatting
- ESP32 Wi-Fi
- MQTT / IoT integration (planned)

## System Architecture

```text
Voltage and Current Sensors
           |
           v
      STM32F407
           |
    Data Processing
           |
      UART (USART1)
           |
           v
          ESP32
           |
        Wi-Fi
           |
           v
    Cloud Dashboard
```

DHT11 will provide temperature and humidity measurements to the STM32 controller.

## STM32 Configuration

| Peripheral | Configuration |
|---|---|
| System Clock | 168 MHz |
| ADC1 | PA0, PA1, PA2 |
| USART1 TX | PA9 |
| USART1 RX | PA10 |
| GPIO LED | PD12 |

## Implemented Features

- STM32F407 project configuration.
- ADC channel configuration and individual channel testing.
- GPIO LED control.
- USART1 configuration at 115200 baud.
- Embedded C firmware development.
- JSON data formatting.
- Initial fault-status logic.

## Development Roadmap

- [x] STM32CubeMX configuration
- [x] GPIO testing
- [x] Individual ADC channel testing
- [x] USART1 configuration
- [x] Initial JSON data formatting
- [ ] DHT11 sensor integration
- [ ] ESP32 UART integration
- [ ] Wi-Fi connectivity
- [ ] MQTT communication
- [ ] Cloud dashboard development
- [ ] Complete hardware testing

## Repository Structure

```text
STM32-Cloud-Power-Monitoring/
|
|-- Core/
|   |-- Inc/
|   |-- Src/
|
|-- Drivers/
|
|-- Startup/
|
|-- Cloud_Monitoring_STM32F4.ioc
|
|-- STM32F407VGTX_FLASH.ld
|-- STM32F407VGTX_RAM.ld
|
|-- README.md
```

## Project Objective

To develop a reliable embedded IoT monitoring system that combines microcontroller-based data acquisition, electrical parameter monitoring, environmental sensing and cloud connectivity.

## Author

**Venkat1512-git**

Embedded Systems | Electrical and Electronics Engineering

GitHub: https://github.com/Venkat1512-git
