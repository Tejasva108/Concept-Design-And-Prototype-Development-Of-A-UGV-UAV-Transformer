# Concept-Design-And-Prototype-Development-Of-A-UGV-UAV-Transformer

# 🚘🛩️ Hybrid Transformable UGV–UAV Robot  
### A Ground-to-Air Transformable Robot using ESP Controllers, Servo Mechanism, and Custom Electronics  

---

## 📖 Overview  
This project demonstrates the design and implementation of a **hybrid ground–aerial vehicle** capable of operating in both **UGV (Unmanned Ground Vehicle)** and **UAV (Unmanned Aerial Vehicle)** modes.  

The robot can **move on the ground using its wheel-based mechanism** and **transform itself to take off as a quadrotor drone**, combining terrestrial mobility with aerial agility.  

The prototype was built using **3D-printed and laser-cut acrylic components**, **custom-designed electronics**, and **open-source control frameworks**.  

---

## 🧩 System Overview  

| Subsystem | Description |
|------------|-------------|
| **Mechanical Design** | The base structure was adapted from an existing open-source SolidWorks design. Modified for fabrication using **3D printing** and **acrylic sheets**. |
| **Transformation Mechanism** | The transformation between UGV and UAV modes is powered by **two servo motors**, which adjust the arm configuration and reorient the BLDC motor mounts for takeoff. |
| **Electronics & Control** | Custom circuit designed for voltage regulation, motor control, and communication. Integrated **flight controller**, **ESP boards**, **motor drivers**, and **servo motor control** for mode switching. |
| **Propulsion** | 6× **BLDC motors** (4 for flight, 2 for drive) controlled using a **4-in-1 ESC** and separate ESCs. |
| **Communication** | **RC receiver** and **transmitter** for manual control. ESP modules handle transformation logic and communication. |
| **Power System** | Li-Po battery setup with voltage regulators to power flight controller, servos, and drive systems. |
| **Software** | Control logic implemented on **ESP32/ESP8266** microcontrollers. Flight handled by onboard flight controller firmware. |

---

## ⚙️ Hardware Components  

| Component | Specification / Function |
|------------|---------------------------|
| **BLDC Motors (×6)** | 4 for flight + 2 for ground drive |
| **4-in-1 ESC** | Controls quadrotor motors |
| **Individual ESCs** | Controls ground drive motors |
| **Servo Motors (×2)** | Mechanically transform the robot from UGV to UAV mode |
| **Flight Controller** | Handles stabilization and flight dynamics |
| **ESP Boards (ESP32/ESP8266)** | Controls transformation sequence and logic |
| **Voltage Regulators** | Power management between modules |
| **RC Receiver + Transmitter** | Manual control interface |
| **3D Printed + Acrylic Frame** | Lightweight mechanical chassis and body |

---

## 🧠 Working Principle  

### 1. UGV Mode  
- The robot moves as a wheeled vehicle using two BLDC drive motors.  
- Controlled via RC transmitter or ESP-based wireless input.  
- Provides stable and power-efficient ground navigation.  

### 2. Transformation Phase  
- **Two servo motors** activate and reposition the arms and motor mounts.  
- The transformation sequence reorients the flight motors from horizontal (drive) to vertical (lift).  
- Power is gradually switched from ground ESCs to flight ESCs.  

### 3. UAV Mode  
- The robot takes off vertically and operates as a quadrotor drone.  
- Controlled via the flight controller and RC transmitter.  
- Enables agile movement and aerial surveillance capabilities.  

---

## 🧰 Fabrication Process  

- Modified **SolidWorks CAD** model from an open-source design.  
- Fabricated parts using **3D printing** and **laser-cut acrylic sheets**.  
- Mounted servo-based transformation joints on custom brackets.  
- Designed and soldered a **custom perfboard circuit** for regulators, ESC, and control logic.  
- Calibrated the **flight controller**, **ESCs**, and **servo positions** for seamless switching.  
- Conducted ground and flight tests for transformation reliability.  

---

## 🧪 Testing and Challenges  

| Stage | Key Challenges | Solutions |
|--------|----------------|-----------|
| **Mechanical Assembly** | Balancing structural rigidity with weight | Used acrylic supports and optimized motor placement |
| **Transformation Mechanism** | Servo synchronization and torque limitations | Tuned servo motion range and added delay for stability |
| **Power Management** | Voltage drops during high-current transitions | Added voltage regulators and capacitors |
| **Signal Interference** | Overlap between RC and ESP signals | Frequency separation and proper shielding |
| **Flight Stability** | Sudden center of mass shifts post-transformation | Adjusted PID parameters on flight controller |

---

## 📸 Demonstration  

