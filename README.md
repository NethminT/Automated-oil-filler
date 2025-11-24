# 🛢️ Development of an Automated Oil Dispensing System

<p align="center">
  <img src="images/Nurse_calling_1.PNG" alt="AgriBot CAD Model" width="500"/>
</p>

## 🛢️ Overview

This project presents an **Automated Oil Filling System** designed to eliminate measurement errors, fraud, and operational inefficiencies in large-scale lubricant dispensing environments.  
The system automates the selection, measurement, and filling of lubricants from warehouse storage tanks through a **PLC-controlled**, **HMI-guided**, and **load-cell-based** dispensing platform.

It ensures that the exact volume selected by the user is dispensed—no more, no less—while continuously monitoring safety and operational integrity.

---

## 🏭 Application Domain

The system is implemented in a **lubricant warehouse environment**, where manual filling often results in:

- Discrepancies between recorded and actual stock levels  
- Inaccurate volume measurements  
- High chances of operator error or misuse  
- Lack of standardized dispensing workflow  

This automated setup provides:

- **Accurate inventory tracking**  
- **Standardized filling processes**  
- **Fraud detection and prevention**    
- **Efficient operation for workshops and service centers**

---

## 🧠 Key Modules & System Architecture

### ⚙️ Automated Dispensing Mechanism

- A **solenoid-valve system** controls oil flow from each storage tank.  
- A **movable trolley** equipped with a **load cell** measures the exact mass of dispensed oil.  
- Wireless data exchange ensures synchronised valve actuation and weight monitoring.  
- A **PLC–HMI network** manages oil type selection and volume entry.

<p align="center">
  <img src="images/oil_filling_trolley.png" alt="Oil Filling Trolley" width="500"/>
</p>

---

## 📲 User Interaction & Operation Workflow

1. Position the trolley under the selected storage tank using built-in guide rails.  
2. Ensure correct alignment via **proximity sensor LED indication**.  
3. Lock wheels and place the oil container on the trolley.  
4. Zero the weight using the load-cell indicator (`Tare/Zero`).  
5. Select:
   - **Oil type**  
   - **Required volume**  
6. Confirm inputs and press **Start**.  
7. The system automatically fills the exact volume and stops the flow.  
8. Remove trolley and power off the panel.

<p align="center">
  <img src="images/oil_filling_hmi.png" alt="HMI Process" width="600"/>
</p>

---
## 📐 System Design Highlights

### 🔧 Hardware & Controls

- PLC: **Xinje XC3-RT48-E**  
- HMI: **Flexem FE2070**  
- Max measurable load: **60 kg**  
- Supports up to **9 storage tanks**  
- Minimum volume resolution: **1 L**  
- Error margin: **± 50 ml per count**  


---

## 📦 Tools & Technologies

- `Xinje PLC` for automation control  
- `Flexem HMI` for interactive UI  
- `Load Cell + Weight Indicator` for precise measurements  
- `Solenoid Valves` for controlled oil flow  
- `Proximity Sensors` for tank selection validation  
- `Wireless modules` for trolley–panel communication  

---
