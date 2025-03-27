
# Domain 3: Security Architecture  
**Topic: Software-Defined Networking (SDN)**

## Overview

Software-Defined Networking (SDN) introduces a modern approach to managing network infrastructure, especially in cloud environments.  
Unlike traditional networking where control, management, and data planes are tightly integrated, SDN **separates** them for better flexibility and control.

---

## Planes in SDN

### Management Plane
- Oversees **network orchestration and traffic monitoring**
- Provides a high-level view of the network for administrators

### Control Plane
- Acts as the **network "brain"**
- A centralized system that:
  - Makes high-level decisions
  - Sets policies
  - Manages traffic routing and resource allocation
- Based on rules set by network administrators

### Data Plane
- Responsible for **forwarding packets**
- Executes instructions from the control plane
- Includes devices like switches, routers, and access points

---

## Benefits of SDN

- **Separation of control and data planes**:
  - Enables **dynamic control** over the network
  - Improves **resource allocation** based on real-time demands
- **Fine-grained control**:
  - Enables real-time **security policy enforcement**
  - Supports **automated responses** to threats
  - Allows **network segmentation** in response to attacks

SDN enhances **network flexibility**, **security**, and **scalability**, making it a vital concept in modern enterprise and cloud-based infrastructures.
