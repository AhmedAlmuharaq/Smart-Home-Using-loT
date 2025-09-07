

### Project Title: Smart Home Using IoT

#### Project Project
This is a comprehensive **Internet of Things (IoT) based Smart Home Automation System** designed and implemented as a graduation project. The core objective is to create a connected home environment where various household appliances and security systems can be **automatically controlled based on sensor data** or **remotely managed via a dedicated Android application**.

The system intelligently monitors environmental conditions (like temperature, humidity, gas leaks, rain, and motion) and responds by activating appropriate devices (such as fans, lights, servo motors for doors/windows, and water pumps) to enhance comfort, safety, and energy efficiency.

---

#### **Key Features & Functionality**

1.  **Automated Environmental Control:**
    *   Uses a **DHT11 sensor** to monitor room temperature and humidity.
    *   Automatically turns on a **fan** if the temperature exceeds a predefined threshold (e.g., 25°C) to cool the room.

2.  **Smart Security System:**
    *   Employs a **PIR (Passive Infrared) sensor** to detect human motion.
    *   Triggers an alert or turns on **LED lights** automatically when movement is detected, enhancing home security.
    *   Uses an **MQ-2 sensor** to detect hazardous gas leaks (e.g., LPG, smoke) and sends immediate alerts to the user.

3.  **Weather-Responsive Automation:**
    *   Integrates a **Rain Sensor** to detect rainfall.
    *   The system can notify the user or trigger actions (like closing windows via a servo motor) when rain is detected.

4.  **Remote Control via Mobile App:**
    *   Developed an **Android application** using MIT App Inventor.
    *   Allows users to remotely control all connected devices (lights, fan, door lock via servo, water pump) from anywhere with an internet connection.
    *   Provides a real-time dashboard to view sensor readings (temperature, humidity, gas levels, weight).

5.  **Advanced Monitoring:**
    *   Includes a **Load Cell sensor** to measure weight, which can be used for applications like smart refrigerators to monitor contents.

---

#### **Core Technologies Used**

*   **Microcontroller:** ESP32 NodeMCU (chosen for its integrated Wi-Fi and Bluetooth capabilities).
*   **Sensors:**
    *   DHT11 (Temperature & Humidity)
    *   PIR (Motion Detection)
    *   MQ-2 (Gas/Smoke Detection)
    *   Rain Sensor
    *   Load Cell (Weight Measurement)
*   **Actuators:**
    *   Servo Motor (for simulating door/window control)
    *   DC Fan
    *   LED Bulbs
    *   Water Pump
*   **Software & Platforms:**
    *   Arduino IDE (for programming the ESP32)
    *   MIT App Inventor (for developing the Android control app)
    *   Cisco Packet Tracer (for network simulation and design)

---

#### **How It Works**
The ESP32 microcontroller acts as the brain of the system. It continuously reads data from the sensors. Based on pre-programmed logic, it can:
*   **React Automatically:** For example, if the temperature is too high, it turns on the fan without user intervention.
*   **Send Alerts:** If a gas leak or motion is detected, it sends a notification to the Android app.
*   **Execute Remote Commands:** When the user sends a command from the app
*    (e.g., "Turn on Light"),
*  the ESP32 receives the command via Wi-Fi (using HTTP requests) and activates the corresponding device.

This project successfully solve real-world problems, creating a safer, more comfortable, and efficient living environment.
