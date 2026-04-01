### Taekwondo Poomsae Scoring System
 
<p align="justify">
A real-time Taekwondo poomsae scoring system that captures judges’ inputs via hardware devices and processes them in a Python-based application to compute accurate final scores and display results.
</p>

---

## Problem
<p align="justify">
Manual scoring in poomsae competitions is susceptible to human errors such as miscalculation, inconsistent judging, and incorrect recording of scores. Additionally, the process is often slow and lacks transparency, making it difficult to track scoring history and ensure fairness in real time.
</p>

---

## Proposed Solution

- A low-cost automated scoring system is developed using microcontrollers to capture judges’ inputs and transmit them to a central application in real time. 
- A Python-based GUI processes the incoming data, applies scoring logic (including additions, deductions and averaging), and provides instant and transparent result visualization.

---

## System Architecture
<p align="justify">
The system is designed with multiple microcontroller-based input units assigned to each judge, which communicate with a central computer via serial (UART) connections. The central Python application acts as the processing hub, handling data synchronization, score computation, and real-time display through a user-friendly interface.
</p>

---

## Implementation
# Hardware
- Built hardware input system using push buttons and microcontrollers (Arduino Nano)
- Design PCB using EasyEDA and send for fabrication
<p align="center">
  <img src="../images/PSSSchematic1.png" width="300">
  <img src="../images/PSSSchematic2.png" width="300">
  <img src="../images/PSSPCB1.png" width="300">
  <img src="../images/PSSPCB2.png" width="300">
</p>

- Design hardware enclosure using Tinkercad
<p align="center">
  <img src="../images/PSS3DCover.png" width="300">
  <img src="../images/PSS3DBase.png" width="300">
</p>

# Software
- Established serial communication between devices and Python application
- Developed a multi-page GUI using Tkinter for data entry, scoring, and history tracking
- Implemented scoring logic including deductions, additions, and averaging across judges
<p align="center">
  <img src="../images/PSSSoftware1.png" width="300">
  <img src="../images/PSSSoftware2.png" width="300">
  <img src="../images/PSSSoftware3.png" width="300">
  <img src="../images/PSSSoftware4.png" width="300">
  <img src="../images/PSSSoftware5.png" width="300">
</p>
  
---

## Results
<p align="justify">
The system successfully automated score calculation, reduced human error, and provided real-time visualization of scoring and history tracking during competitions.
</p>

---

## Key Skills Demonstrated

- Embedded systems integration
- Serial communication (hardware–software interface)
- GUI development in Python
- Real-time data processing
- System design and debugging

## Technologies Used

- Python (Tkinter, PySerial)
- Arduino Nano
- Serial Communication (UART)
- Basic electronics (push buttons, GPIO)
