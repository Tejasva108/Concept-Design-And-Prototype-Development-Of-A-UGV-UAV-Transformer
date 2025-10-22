# Concept-Design-And-Prototype-Development-Of-A-UGV-UAV-Transformer
# 🚘🛩️ Hybrid Transformable UGV–UAV Robot  
### A Ground-to-Air Transformable Robot using ESP Controllers and Custom Electronics  

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
| **Transformation Mechanism** | The robot’s arms and wheels serve dual purposes — **driving in UGV mode** and **propelling in UAV mode** using **BLDC motors**. |
| **Electronics & Control** | Custom circuit designed for voltage regulation, motor control, and communication. Integrated **flight controller**, **ESP boards**, and **motor drivers** for mode switching. |
| **Propulsion** | 6× **BLDC motors** (4 for flight, 2 for drive) controlled using **4-in-1 ESC** and standalone ESCs. |
| **Communication** | **RC receiver** and **transmitter** used for manual control. ESP modules enabled control logic and data exchange. |
| **Power System** | Li-Po battery setup with voltage regulators for motor and control circuits. |
| **Software** | Control logic implemented via microcontrollers (ESP32/ESP8266) and flight controller firmware. |

---

## ⚙️ Hardware Components  

| Component | Specification / Function |
|------------|---------------------------|
| **BLDC Motors (×6)** | Drive and lift propulsion |
| **4-in-1 ESC** | Controls flight motors |
| **Individual ESCs** | Controls ground drive motors |
| **Flight Controller** | Stabilization and flight control |
| **ESP Boards** | Mode control and wireless communication |
| **Voltage Regulators** | Power supply stabilization |
| **RC Receiver + Transmitter** | Manual control interface |
| **3D Printed Parts + Acrylic Sheets** | Mechanical chassis and body |

---

## 🧠 Working Principle  

### 1. UGV Mode  
- Operates as a wheeled vehicle using ground motors.  
- Controlled via RC transmitter or ESP logic.  
- Stable and energy-efficient for ground navigation.  

### 2. Transformation Phase  
- On command, the robot switches power and control logic to flight mode.  
- Ground wheels disengage while flight motors spin up.  

### 3. UAV Mode  
- The robot takes off vertically and functions as a quadrotor drone.  
- Controlled via flight controller and RC inputs.  

---

## 🧰 Fabrication Process  

- Extracted and modified **SolidWorks CAD** from an open-source source.  
- Fabricated the body using **3D printing** and **laser-cut acrylic sheets**.  
- Assembled electronics on a custom **perfboard circuit**.  
- Calibrated flight controller and ESCs.  
- Conducted ground and short flight tests for stability and transformation control.  

---

## 🧪 Testing and Challenges  

| Stage | Key Challenges | Solutions |
|--------|----------------|-----------|
| **Mechanical Assembly** | Balancing weight between ground and flight components | Optimized component placement |
| **Power Management** | Voltage drops during mode switching | Added dedicated regulators and capacitors |
| **Transformation Stability** | Sudden torque shifts during takeoff | Gradual throttle mapping during transition |
| **Signal Interference** | Overlap between RC and ESP control | Used frequency separation and shielding |

---

## 📸 Demonstration  

> *(Add images or video links here once available)*  

Example:  
```markdown
![UGV Mode](images/ugv_mode.jpg)
![UAV Mode](images/uav_mode.jpg)
![Transformation](images/transformation.jpg)
