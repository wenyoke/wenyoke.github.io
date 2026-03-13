### Final Year Project | iNOTEK Series I 2026 Silver Award
## Enhancing Privacy in Location-Based Services Using a Hybrid AOA-TDOA Positioning Technique 
<p align="justify">
This project develops a privacy-aware localization framework for Location-Based Services by combining Angle of Arrival and Time Difference of Arrival methods. The hybrid algorithm was implemented in MATLAB to improve positioning accuracy while reducing the exposure of precise user location data.
</p>

---

## Problem
<p align="justify">
Conventional Location-Based Services often require users to share precise location data with service providers, which may expose sensitive personal information. This project investigates how localization techniques can be designed to maintain accurate positioning while protecting user privacy.
</p>

---

## Proposed Solution
<p align="justify">
A hybrid localization algorithm combining Angle of Arrival (AOA) and Time Difference of Arrival (TDOA) was developed to estimate user location more accurately. A proximity-based access control mechanism was also designed to limit the disclosure of precise location information to unauthorized parties.
</p>

---

## System Architecture
<p align="justify">
The system architecture outlines the workflow for developing a hybrid AOA–TDOA localization framework. Standalone AOA and TDOA algorithms are first developed and validated before being integrated into a hybrid positioning algorithm implemented in MATLAB. The system then evaluates localization performance using simulated data and incorporates a proximity-based mechanism to enhance user privacy.
</p>

### Project Overall Flowchart
<p align="justify">
The flowchart illustrates the process of collecting AOA and TDOA measurements from multiple anchor nodes, followed by position estimation through the hybrid localization algorithm. The algorithm combines angular and time-difference information to improve localization accuracy compared to single-technique methods.
</p>
<p align="center">
  <img src="../images/Methodology1.png" width="471">
  <img src="../images/Methodology2.png" width="500">
</p>

### Proximity-Based Privacy Mechanism
<p align="justify">
To enhance user privacy, a proximity-based access control mechanism is introduced. Only users within a predefined proximity radius are allowed to obtain more precise location information, while others receive limited or obfuscated location data.
</p>
<p align="center">
  <img src="../images/PrivacyMechanism.png" width="500">
</p

---
---

## Implementation
<p align="justify">
The localization algorithm was implemented and simulated in MATLAB. Multiple anchor nodes were modeled to estimate target position using AOA and TDOA measurements. Performance was evaluated using statistical metrics including RMSE and CDF.
</p>
<p align="center">
  <img src="../images/AOAconcept.png" width="281">
  <img src="../images/TDOAconcept.png" width="310">
  <img src="../images/Hybridconcept.png" width="228">
</p>
<p align="center">
  Figure 1: Angle of Arrival (AOA) | Figure 2: Time Difference of Arrival (TDOA) | Figure 3: Hybrid Localization (AOA & TDOA)
</p>

---

## Results
<p align="justify">
Simulation results demonstrate that the hybrid AOA–TDOA framework improves localization accuracy compared to single-technique approaches. Performance evaluation using RMSE and cumulative distribution functions shows more reliable positioning while maintaining user privacy constraints.
</p>

### Angle of Arrival (AOA)
<p align="center">
  <img src="../images/AOANLOS.png" width="400">
  <img src="../images/AOANLOSMATLAB.png" width="400">
</p>
<p align="center">
  Figure 4: Angle of Arrival (AOA) with Non-Line-Of-Sight (NLOS) errors injected
</p>

### Time Difference of Arrival (TDOA)
<p align="center">
  <img src="../images/TDOANLOS.png" width="400">
  <img src="../images/TDOANLOSMATLAB.png" width="400">
</p>
<p align="center">
  Figure 5: Time Difference of Arrival (TDOA) with Non-Line-Of-Sight (NLOS) errors injected
</p>

### Hybrid Localization Approach (AOA + TDOA)
<p align="center">
  <img src="../images/HYBRIDNLOS.png" width="400">
  <img src="../images/HYBRIDNLOSMATLAB.png" width="400">
</p>
<p align="center">
  Figure 6: Hybrid Localization Method with Non-Line-Of-Sight (NLOS) errors injected
</p>

### Root Mean Square Error (RMSE) & Cumulative Distribution Function (CDF) Analysis

<p align="center">
  <img src="../images/AverageRMSEAOA.png" width="300">
  <img src="../images/AverageRMSETDOA.png" width="303">
  <img src="../images/AverageRMSEHYBRID.png" width="300">
</p>
<p align="center">
  Average RMSE VS Number of Base Stations for
</p>
<p align="center">
  Figure 7: AOA | Figure 8: TDOA | Figure 9: Hybrid
</p>

<p align="center">
  <img src="../images/AverageRMSEAOATable.png" width="300">
  <img src="../images/AverageRMSETDOATable.png" width="303">
  <img src="../images/AverageRMSEHYBRIDTable.png" width="300">
</p>
<p align="center">
  Average RMSE VS Number of Base Stations for
</p>
<p align="center">
  Figure 10: AOA | Figure 11: TDOA | Figure 12: Hybrid
</p>

---

## Key Skills Demonstrated

- Wireless localization algorithms
- MATLAB simulation and modeling
- Data analysis using RMSE and CDF metrics
- Privacy-aware system design

## Technologies Used

- MATLAB
- Localization Algorithms
- AOA and TDOA Positioning
- Wireless Network Simulation
