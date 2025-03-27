
# Domain 3: Security Architecture  
**Topic: SCADA Architecture & Security Implications**

## SCADA System Overview

SCADA (Supervisory Control and Data Acquisition) systems manage industrial control systems (ICS) and are commonly used in critical infrastructure environments.

### SCADA Hierarchical Levels

#### **Plant Level (Level 0)**
- Lowest level in the SCADA hierarchy
- Includes **physical equipment and processes** (e.g., sensors, actuators, motors, pumps)
- Devices collect data and perform actions directed by higher-level controllers

#### **Controller Level (Level 1)**
- Handles **real-time control** of physical processes
- Uses **Programmable Logic Controllers (PLCs)** to:
  - Receive sensor input
  - Process data
  - Send commands to actuators and devices
- Ensures plant operations run **efficiently and safely**

#### **Coordinating Computer Level (Level 2)**
- Includes **supervisory computers and HMIs (Human-Machine Interfaces)**
- Provides a **centralized view** of plant operations
- Collects and displays data from Level 1 controllers
- Allows operators to monitor status, respond to alarms, and adjust processes

#### **Program Logic Controller Level (Level 3)**
- Manages and controls **overall production**
- Often includes advanced systems for:
  - **Recipe management**
  - **Production scheduling**
  - **Data logging and reporting**

---

## Common SCADA Use Cases

SCADA systems are used in industries where automation and real-time control are essential:

- **Energy**: Power generation, oil & gas refineries
- **Facilities**: HVAC and building management systems
- **Manufacturing**: Assembly and production control
- **Logistics**: Device/component tracking and assembly (e.g., computers)
- **Industrial**: Processing raw materials (e.g., steel, water treatment)

---

## Real-World Example

- **Stuxnet Virus**:  
  A famous cyberattack on an Iranian uranium enrichment facility targeting SCADA-controlled centrifuges.
  - Discovered in 2007 (possibly active since 2005)
  - Highlighted vulnerabilities in SCADA environments

---

## Security Implications

SCADA systems are **high-value targets** due to their role in controlling critical infrastructure.  
Securing these systems involves:
- Strong access controls
- Network segmentation
- Real-time monitoring and response capabilities
