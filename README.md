# Hydroelectric-Power-Plant-Project
Hydroelectric Power Plant with HMI written in LAD, FBD, SCL, STL

# Project Description 
### This project simulates the control and automation of a small-scale hydroelectric power plant using Siemens S7-1500 PLC and HMI. The system is designed to handle fluctuating river flow rates and dynamically adjust plant parameters to ensure safe and efficient power generation.

![Image](https://github.com/user-attachments/assets/00a3e1eb-8671-4c0c-8443-873c9a66fe08)

## Control System
**Developed a PLC-based control system using Siemens S7-1500 and HMI. A servo-controlled baffle (4–20 mA) adjusts river flow to control rotor speed and power output. A VFD-driven oil pump cools rotor bearings, with flow monitored to prevent overuse. Power is delivered to the grid once generation reaches threshold levels. Safety features include an HMI-based emergency stop and rotor brake when idle.**

![Image](https://github.com/user-attachments/assets/46f7fcc8-9063-4c09-b545-136e872f0238)

### Main Components
 - Baffle 
 - Alarm Horn
 - Generator
 - Oil Pump
 - Power Station

## Built With
- Software: TIA Portal V20
- PLC: Siemens S7-1500
- Simulation: PLC Sim Advance
- HMI: PC Station (WinCC Simatic)
- Programming Language: Ladder Logic (LAD) and FBD, SCL, STL

## Project Tree
  ![Image](https://github.com/user-attachments/assets/2ca0a34f-4273-454e-97c7-00ec5253fcc5)
  
**The program is structured using four programming languages and divided into layers: I/Os, HOA control, Alarm Management, Hour Meter, and Modes. Each layer is responsible for one main task, ensuring clarity, modularity, and efficient system operation.**

## Main
### How to switch Programming Languages
  - Using a Ladder in Main OB
  - Switching languages using a Equal Comparator with values

![Image](https://github.com/user-attachments/assets/f4d296c9-6f7f-4ed5-9bed-cef6ff991e25)
![Image](https://github.com/user-attachments/assets/46c7cc43-9dc2-4f9f-88bf-c2e69b1f7275)


## Features
### IO's
**Analog input values are read as REAL data types for accurate measurement. Functions like Scale X are used to convert raw signals (e.g., 4–20 mA) into usable engineering units, while Norm X normalizes the values. These are then converted to INT if needed for control logic or digital processing**

![Image](https://github.com/user-attachments/assets/b1592ee6-5fb8-455e-abc0-f5d3032a1ff3)

### **Our Digital&Analog IO**
  - Baffle
  - Rotor Speed
  - Oil Pump VFD
  - Oil Flow
  - Oil Temperature
  - Power Station Interlock
  - Alarm Horn
  - Generator Brake
  - E Stop
  - AC Current

  ## Alarm Condition
  **High Oil Temp Shown in SCL**

  ![Image](https://github.com/user-attachments/assets/61e884d7-5617-456d-836b-73cf4ab28b81)
  
  - Overcurrent
  - High Oil Temperature
  - Rotor Overspeed
  - Oil Low Flow
  - Oil High Flow
  - E Stop
  - Brake Failure
    
  ## Sequence of Modes
  ![Image](https://github.com/user-attachments/assets/bad80e28-b300-4bc8-ab4a-f961cd50e559)
  - Warmup Mode
  - Stabilize Mode
  - Generation Mode
  - Cooldown Mode
    
**Idle Mode and Fault Mode**
**Shown in STL**
    
  ![Image](https://github.com/user-attachments/assets/e0e6da03-1ade-40da-8900-193b1c777f52)
      
  ## HMI Details
 > **System Status show system mode, alarm indicators, important process values, high-level system 
controls** 

![Image](https://github.com/user-attachments/assets/660ca294-9d6e-4e5a-a95a-529179f12cd5)


 >**System Overview show a graphical representation of our system with relevant process values 
appearing at their points of collection.**   

![Image](https://github.com/user-attachments/assets/a03b066f-d966-48c5-8edc-b165aec8a734)


 >**Alarm Management show alarm history, alarm reset and silence buttons, and indicators which show 
the presence of actual alarm bits**

![Image](https://github.com/user-attachments/assets/fdeffd3c-ab8f-46b6-8538-5556c610b636)


>**Configurations give the Operator controls over all devices to include manual setpoints for analog devices. 
Also, display the status / values of inputs signals / hour meter used to know the generation days or hours.**

![Image](https://github.com/user-attachments/assets/8f7d4e2b-d655-4dbf-8114-c5299db8d39a)


## Learning Outcomes
- Mastered analog and digital signal integration in PLCs
- Understood hydroelectric plant operation and automation challenges
- Gained experience in real-time monitoring and interface design
- Improved fault handling and system safety implementation







      
