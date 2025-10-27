# IoT-Based RFID Crowd Analyzer

## Overview
The **RFID Crowd Analyzer** is an IoT-driven system designed to monitor real-time occupancy and environmental conditions in shared spaces such as gyms or offices.  
This project integrates **RFID, Arduino, Raspberry Pi, and cloud analytics** to enable remote visibility of crowd density and facility conditions, helping users make informed decisions about when to visit.

Developed as part of an academic research project, the system demonstrates the practical convergence of **IoT sensing, edge computing, and cloud-based analytics**.

---

## Objectives
- Design and implement an IoT system to monitor room occupancy using RFID sensors.  
- Collect and visualize real-time environmental data (temperature, humidity, lighting).  
- Enable remote monitoring through ThingSpeak Cloud API integration.  
- Automate environmental controls (fans, lights) based on live conditions.  

---

## Tools and Technologies
- **Hardware:** Raspberry Pi 3, Arduino Uno, RFID Reader (MFRC522), RFID Tags, DHT-11 Sensor, Photoresistor, DC Motor  
- **Software & Libraries:**  
  - Arduino IDE  
  - Python (Raspberry Pi)  
  - PyFirmata for Arduino–Raspberry communication  
  - ThingSpeak Cloud API for real-time data visualization  
- **Connectivity:** Wi-Fi network (via Raspberry Pi)  
- **Programming Languages:** C++, Python  

---

## System Architecture
1. **Data Acquisition**  
   - Each gym member is identified via **RFID tag scans** at entry and exit points.  
   - Environmental sensors collect temperature, humidity, and light intensity data.  

2. **Processing Layer**  
   - Arduino handles sensor data collection and actuator control (LEDs, fans).  
   - Raspberry Pi serves as the intermediary node, running Python scripts to aggregate and transmit data to the cloud using **PyFirmata**.  

3. **Cloud Integration**  
   - ThingSpeak Cloud API used for remote monitoring and visualization of real-time data.  
   - Dashboards display metrics like gym occupancy, ambient temperature, and humidity levels.  

4. **Automation Logic**  
   - Automated fan and lighting controls based on sensor readings and occupancy count thresholds.  

---

## Results
- Successful real-time monitoring of occupancy and environmental conditions using cloud dashboards.  
- Enabled remote decision-making for users based on live crowd data.  
- Reduced manual environmental control by automating fan and light systems.  
- Demonstrated a scalable architecture for IoT-driven facility management.  

---

## Challenges and Limitations
- Connectivity issues encountered between Raspberry Pi and dorm Wi-Fi network.  
- Integration challenges due to Cisco PL-App incompatibility with macOS.  
- Delays in real-time data sync during early cloud integration phases.  

---

## Future Work
- Deploy dual RFID scanners for separate entry and exit tracking to improve accuracy.  
- Integrate SQL-based attendance database for member analytics.  
- Apply predictive analytics for **peak hour forecasting** and user behavior insights.  
- Develop a dedicated **mobile app** for user access to personalized analytics and alerts.  

---

## Author
**Aashika Chakravarty**  
Master of Engineering, Information and Electrical Engineering  
Hochschule Wismar, Germany  
Email: aashikachakravarty@gmail.com  
LinkedIn: [linkedin.com/in/aashikachakravarty](https://www.linkedin.com/in/aashikachakravarty)
