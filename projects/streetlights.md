### Auto Lighting System for Street Lights
 
<p align="justify">
This project implements a smart street lighting system that improves energy efficiency through automatic light detection and control. It features IoT-based monitoring by sending real-time data to a cloud dashboard for visualization and analysis.
</p>

---

## Problem
<p align="justify">
Traditional street lighting systems often rely on manual control or fixed timers, leading to unnecessary energy consumption and inefficiency. These systems also lack real-time monitoring, making maintenance and performance tracking difficult.
</p>

---

## Proposed Solution
<p align="justify">
This project proposes an automated street lighting system that adjusts lighting based on ambient light intensity using an LDR sensor. It also integrates IoT capabilities to enable real-time monitoring and data visualization through a cloud platform.
</p>

---

## System Architecture
<p align="justify">
The system consists of an LDR sensor connected to the STM32F446RE, which processes light intensity data and controls the lighting output. An ESP8266 ESP-01 is used to transmit data to the ThingSpeak for remote monitoring and analysis.
</p>
<p align="center">
  <img src="../images/StreetConcept.png" width="500">
</p>

---

## Implementation
### Hardware
<p align="justify">
The LDR sensor is connected to an ADC pin of the STM32F446RE, utilizing its 12-bit ADC to convert analog light intensity into digital values. LEDs are driven through GPIO pins to simulate street lighting, while the ESP8266 ESP-01 communicates with the microcontroller via UART (e.g., 115200 baud rate) for wireless data transmission.
</p>
<p align="center">
  <img src="../images/StreetPrototype.jpeg" width="300">
</p>

### Software
<p align="justify">
Embedded C firmware is developed in STM32CubeIDE to continuously sample ADC data, apply threshold-based decision logic, and control the lighting states. UART communication is configured to send formatted sensor data at regular intervals to the ThingSpeak, enabling real-time data logging and visualization.
</p>
<p align="center">
  <img src="../images/StreetSW1.png" width="350">
  <img src="../images/StreetSW2.png" width="320">
  <img src="../images/StreetSW3.png" width="320">
  <img src="../images/StreetPing.jpeg" width="430">
  <img src="../images/StreetTeraTerm.jpeg" width="280">
  <img src="../images/StreetTroubleshoot.jpeg" width="470">
  <img src="../images/StreetDashboard.jpeg" width="375">
</p>
  
---

## Results
<p align="justify">
The system successfully automates street lighting control, turning lights on during low-light conditions and off during daylight. Real-time data visualization on the IoT dashboard demonstrates reliable system performance and remote accessibility.
</p>
<p align="center">
  <img src="../images/StreetThingSpeak1.png" width="400">
  <img src="../images/StreetThingSpeak2.png" width="370">
  <img src="../images/StreetResults.jpeg" width="320">
</p>

---

## Key Skills Demonstrated

- Embedded system design using STM32F446RE
- Microcontroller programming in Embedded C (ADC, GPIO, UART configuration)
- Sensor integration and analog signal processing (LDR with 12-bit ADC)
- IoT system integration with wireless communication using ESP8266 ESP-01
- Real-time data acquisition, formatting, and cloud transmission
- System debugging and testing using serial communication and live data monitoring
- Basic hardware prototyping and circuit integration

## Technologies Used

- Development Tools: STM32CubeIDE
- Programming Language: Embedded C
- Communication Protocols: UART (MCU ↔ ESP8266)
- IoT Platform: ThingSpeak
- Networking: Wi-Fi (via ESP8266 module)
