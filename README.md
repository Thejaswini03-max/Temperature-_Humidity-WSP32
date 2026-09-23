1. Project Title:
ESP32 Based Temperature and Humidity Monitoring System using DHT22 and ThingSpeak
2. Problem Statement:
Monitoring temperature and humidity manually can be difficult and time-consuming. This project provides an IoT-based solution to measure temperature and humidity using a DHT22 sensor connected to an ESP32. The collected data is sent through Wi-Fi to the ThingSpeak cloud platform for monitoring and visualization.
3. Objectives:
To measure temperature and humidity using the DHT22 sensor.
To interface the DHT22 sensor with ESP32.
To collect sensor readings using MicroPython.
To send the collected data to ThingSpeak through Wi-Fi.
To visualize temperature and humidity readings using graphs.
To understand the basic working of an IoT cloud-based monitoring system.
4. Components and Software Used:
Hardware
ESP32
DHT22 Temperature and Humidity Sensor
Software/Platforms
Wokwi Simulator
MicroPython
ThingSpeak Cloud Platform
GitHub
5. Circuit Diagram:
Connections
DHT22
ESP32
VCC
3V3
DATA
GPIO 15
GND
GND
Circuit diagram: Insert your circuit diagram screenshot here.
6.Block Diagram:
The block diagram of the proposed IoT-based temperature and humidity monitoring system is shown below.
7. Working Principle:
The DHT22 sensor measures the surrounding temperature and humidity. The sensor is connected to GPIO 15 of the ESP32.
The ESP32 reads the sensor values using a MicroPython program. It then connects to the Internet through Wi-Fi and sends the temperature and humidity data to the ThingSpeak cloud platform.
ThingSpeak receives the data and displays it in the form of graphs. This allows the sensor readings to be monitored and visualized easily.
8. Program Explanation:
The program uses MicroPython to control the ESP32 and DHT22 sensor.
Important parts of the program include:
import dht – imports the DHT sensor library.
from machine import Pin – allows the ESP32 GPIO pin to be used.
dht.DHT22(Pin(15)) – connects the DHT22 data pin to GPIO 15.
sensor.measure() – takes a new measurement.
sensor.temperature() – obtains the temperature value.
sensor.humidity() – obtains the humidity value.
Wi-Fi and HTTP requests are used to send the readings to ThingSpeak.
9. Output:
The ESP32 successfully reads temperature and humidity values from the DHT22 sensor.
The readings are displayed in the Wokwi serial monitor and are also sent to ThingSpeak. ThingSpeak displays the received temperature and humidity values using graphs.
Insert here:
Wokwi output screenshot
ThingSpeak graph screenshot
10. Applications:
Smart home environmental monitoring
Agriculture and greenhouse monitoring
Weather monitoring
Indoor temperature and humidity monitoring
IoT-based environmental monitoring
Educational IoT projects
11. Limitations:
The system requires Wi-Fi connectivity for cloud communication.
DHT22 has limitations in measurement range and accuracy.
ThingSpeak requires Internet connectivity to receive and display data.
Sensor readings may vary depending on environmental conditions.
12. Future Scope:
The project can be improved by:
Adding more sensors.
Adding mobile notifications and alerts.
Using a mobile application for monitoring.
Adding automatic control based on temperature or humidity.
Storing and analyzing larger amounts of sensor data.
Developing a complete smart-home monitoring system.
13. Team Members' Details:
Name:
Register Number:
Thejaswini C
U03ZW24S0084,
Bsc. 5th Semester MEC
14. Wokwi Project Link
Wokwi Project:
Paste your final saved Wokwi project link here.
Make sure it is your actual project link, not wokwi.com/projects/new/....
15. ThingSpeak Channel Link:
ThingSpeak Channel ID: 3500612
Paste your final ThingSpeak channel link here.
16. Learning Reflection:
Through this project, I learned how an IoT system can collect real-time environmental data using sensors and send the data to a cloud platform. I learned how to connect a DHT22 sensor with an ESP32, write a MicroPython program, simulate the circuit using Wokwi, connect the system to Wi-Fi, and send sensor readings to ThingSpeak. I also gained experience in using GitHub to store and present the project files. This project helped me understand the practical working of sensors, microcontrollers, cloud platforms, and IoT communication.
Conclusion:
This project successfully demonstrates an IoT-based temperature and humidity monitoring system using ESP32 and DHT22. The sensor data is collected, sent through Wi-Fi to ThingSpeak, and displayed as graphs. Through this project, we gained practical knowledge of IoT, sensors, ESP32, MicroPython, cloud platforms, and Wokwi simulation.
