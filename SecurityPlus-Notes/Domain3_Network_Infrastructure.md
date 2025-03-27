
# Domain 3: Security Architecture  
**Topic: Network Infrastructure & OSI Model Layers**

## Overview

Network infrastructure consists of the devices, protocols, and routing components that support secure communication within an interconnected environment.

---

## OSI Model & Network Devices

| Layer                     | Devices                                             | Function                                           |
|--------------------------|-----------------------------------------------------|----------------------------------------------------|
| Layer 7: Application     | Web Application Firewall (WAF), NIPS                | Handles protocols like DNS, SMTP, HTTP, FTP        |
| Layer 4: Transport       | Load Balancer                                       | Manages TCP/UDP traffic                            |
| Layer 3: Network         | Routers, Subnets, Layer 3 Switch                    | IP addressing and packet routing                   |
| Layer 2: Data Link       | Switch, VLAN, Wireless Access Point (WAP)           | MAC addresses, VLANs, ARP                          |
| Layer 1: Physical        | Cabling                                             | Physical media for transmission                    |

---

## Key Terms & Components

### Address Resolution Protocol (ARP)
- Maps **IP addresses to MAC addresses**
- Allocates a unique MAC to each port on a switch

### Layer 3 Switch
- Also called a **multilayer switch**
- Works at both Layer 2 and Layer 3
- Used to segment traffic and route packets

### Load Balancer
- **Distributes traffic** across multiple servers
- Helps ensure efficient handling of **high traffic loads**

### Web Application Firewall (WAF)
- Protects **web servers and applications** from common exploits
- Monitors and filters **HTTP traffic**

### Network Intrusion Prevention System (NIPS)
- Continuously monitors traffic for malicious activity
- Uses:
  - **Signature-based detection**
  - **Anomaly detection**
  - **Behavioral analysis**
- Identifies and blocks:
  - Unauthorized access
  - Malware
  - Other network threats
- Supports:
  - Data integrity
  - Availability
  - **Incident response**
  - **Policy enforcement**

---

## Security Consideration

- **Switch Port Security**:  
  Network administrators must implement security measures (e.g., disabling unused ports, port security features) to **prevent unauthorized access** to the switch infrastructure.

These layers and devices form the backbone of secure, resilient network design and are essential knowledge for securing enterprise environments.
