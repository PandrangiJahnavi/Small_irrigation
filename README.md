# Smart Irrigation System using ESP32 and Blynk IoT

## Overview

This project is an IoT-based Smart Irrigation System developed using ESP32, Soil Moisture Sensor, Rain Sensor, DHT11 Sensor, Relay Module, and Blynk Cloud Platform.

The system continuously monitors soil moisture, temperature, humidity, and rainfall conditions. Based on the soil moisture level and rain detection status, the irrigation pump is automatically controlled to optimize water usage and improve agricultural efficiency.

## Features

* Automatic irrigation control
* Soil moisture monitoring
* Rain detection
* Temperature monitoring
* Humidity monitoring
* Real-time cloud dashboard
* Remote monitoring using Blynk Mobile App
* Water conservation through intelligent automation

## Components Required

* ESP32 Development Board
* Soil Moisture Sensor
* Rain Sensor Module
* DHT11 Temperature & Humidity Sensor
* Relay Module
* Water Pump
* Breadboard
* Jumper Wires

## Pin Connections

| Component            | ESP32 Pin |
| -------------------- | --------- |
| DHT11 Data           | GPIO 4    |
| Soil Moisture Sensor | GPIO 34   |
| Rain Sensor          | GPIO 35   |
| Relay Module         | GPIO 26   |

## Blynk Virtual Pins

| Virtual Pin | Function            |
| ----------- | ------------------- |
| V0          | Soil Moisture (%)   |
| V1          | Temperature (°C)    |
| V2          | Humidity (%)        |
| V3          | Rain Status         |
| V4          | Pump Status         |
| V5          | Manual Pump Control |

## Working Principle

1. The soil moisture sensor measures soil water content.
2. The DHT11 measures temperature and humidity.
3. The rain sensor detects rainfall.
4. Sensor data is uploaded to the Blynk dashboard.
5. If soil moisture falls below 30% and rain is not detected:

   * Pump turns ON automatically.
   * Irrigation starts.
6. If sufficient moisture is available or rain is detected:

   * Pump turns OFF.
7. Users can monitor data remotely through the Blynk mobile application.

## Automation Logic

### Pump ON

Condition:

```text
Soil Moisture < 30%
AND
No Rain Detected
```

Action:

```text
Pump ON
Irrigation Active
```

### Pump OFF

Condition:

```text
Soil Moisture ≥ 30%
OR
Rain Detected
```

Action:

```text
Pump OFF
Water Saved
```

## Dashboard Parameters

* Soil Moisture Percentage
* Temperature
* Humidity
* Rain Status
* Pump Status

## Applications

* Smart Agriculture
* Precision Farming
* Greenhouse Automation
* Garden Irrigation
* Water Conservation Systems
* IoT-Based Farming Solutions

## Technologies Used

* ESP32
* Blynk IoT
* DHT11 Sensor
* Soil Moisture Sensor
* Rain Sensor
* Relay Module
* Arduino IDE
* Wi-Fi Communication

## Future Improvements

* ThingSpeak Data Logging
* AWS Cloud Integration
* SMS Alerts
* Mobile Notifications
* AI-Based Irrigation Prediction
* Solar-Powered Irrigation System
* Water Flow Monitoring

## Project Level

### Level 1

Sensor-based soil moisture monitoring.

### Level 2

Cloud monitoring using Blynk IoT.

### Level 3

Automatic irrigation and intelligent pump control.

OUTPUT
https://github.com/PandrangiJahnavi/Small_irrigation/blob/main/WhatsApp%20Image%202026-06-16%20at%2011.22.21%20AM.jpeg
https://github.com/PandrangiJahnavi/Small_irrigation/blob/main/WhatsApp%20Image%202026-06-16%20at%2011.24.48%20AM.jpeg


## Author

**Pandrangi Jahnavi**

B.E. Electronics and Communication Engineering (ECE)

AWS Certified Cloud Practitioner

IoT | Embedded Systems | Smart Agriculture | Cloud Computing
