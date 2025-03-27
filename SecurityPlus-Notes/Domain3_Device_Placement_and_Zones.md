
# Domain 3: Security Architecture  
**Topic: Device Placement, Security Zones, and Device Attributes**

## Device Placement

Network devices should be strategically placed across three zones based on security requirements:

| Zone                      | Description            | Example Devices                                                                 |
|---------------------------|------------------------|----------------------------------------------------------------------------------|
| **Local Area Network (LAN)** – Trusted Zone | Internal, secure network | IPS, IDS, Load Balancer, Switches, Sensors                                      |
| **Screened Subnet (DMZ)** – Boundary Layer | Sits between LAN and WAN | IPS, IDS, Jump Server, Proxy, Reverse Proxy, Load Balancer, Sensors             |
| **Wide Area Network (WAN)** – Untrusted Zone | External network (e.g., Internet) | Router, ACL (Access Control List)                                               |

- **Firewalls** are placed between each zone to filter and inspect traffic.

---

## Security Zones

Security zones are network segments that enforce their own:
- **Security policies**
- **Access controls**
- **Trust levels**

### Key Features:

- **Segmentation**: Divides the network logically or physically based on criteria like roles, device types, or data sensitivity.
- **Data Protection**: Store sensitive data in secure, encrypted zones. Use **Full Disk Encryption (FDE)** and **Data Loss Prevention (DLP)** tools.  
  - Centralize data storage to avoid data leakage.
  - Use **VPNs** and maintain audit trails.
- **Access Control**: Zones have unique access rules.  
  - Example: DMZ may allow external web access, but LAN is only accessible by internal employees.

---

## Device Attributes

Devices in a network serve different security functions and can be categorized as:

### 1. **Active Devices**
- Intervene in real time to block threats
- Examples:
  - **Firewalls**: Block unauthorized access
  - **IPS**: Detect and block known attack patterns

### 2. **Passive Devices**
- Monitor and analyze traffic without interfering
- Focused on **visibility and analysis**
- Example:
  - **IDS**: Analyzes traffic for suspicious patterns

### 3. **Inline Devices**
- Placed directly in the path of network traffic
- Can allow/block packets in real time
- Examples:
  - **Firewall appliances**
  - **Load balancers**

### 4. **Tap/Monitor Devices**
- Duplicate traffic for analysis without affecting flow
- Example:
  - **Packet Sniffer** (network packet analyzer)

> **Note**: Failing to secure devices or zones properly can lead to vulnerabilities. Always evaluate placement and attributes for optimal defense.
