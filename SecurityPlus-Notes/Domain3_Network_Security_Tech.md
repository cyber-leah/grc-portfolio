
# Domain 3: Security Architecture  
**Topic: Network Appliances, Port Security, Firewalls, Tunneling, SD-WAN, and SASE**

---

## Network Appliances

### Jump Server
- Intermediary for remote admin of critical components.
- Connect via **SSH** or **RDP** to access/manage servers, switches, routers, and internal infrastructure.

### Proxy Server
- Acts as a go-between for clients and external resources.
- Maintains **logs of requests**, applies **URL filtering**, **content filtering**, **web caching**.

### Reverse Proxy Server
- Handles **incoming traffic** to internal resources.
- Sits in the **screened subnet (DMZ)**.
- Manages authentication and decryption before forwarding traffic.

### IPS (Intrusion Prevention System)
- **Active** device placed **inline** near firewalls.
- Detects and **blocks suspicious activity** using signature, anomaly, and behavioral analysis.

### IDS (Intrusion Detection System)
- **Passive** device.
- Detects but does not block threats.
- Sends alerts based on suspicious behavior.

---

## Load Balancer

- Distributes traffic to servers to ensure availability and performance.
- Types:
  - **Layer 4**: Uses packet headers (e.g., IP, port).
  - **Layer 7**: Uses content/context for routing decisions.
- Load balancing methods:
  - **Least Utilized Host**
  - **Affinity (Sticky Session)**
  - **DNS Round Robin**

---

## Port Security

### Overview
- Prevents unauthorized access through network ports.
- Controls who connects and what traffic is allowed.

### Techniques
- **Sticky MAC**: Binds port to device MAC address.
- **Disable unused ports**
- **802.1x Authentication**:
  - Authenticates users via certificates or RADIUS server.
  - **EAP (Extensible Authentication Protocol)** enhances 802.1x.

---

## Firewall Types

### Layer 4 Firewall
- Packet filtering.
- Stateless; makes decisions based on TCP/IP headers.

### Layer 7 Firewall
- Application layer inspection.
- Controls access based on app and user behavior.

### Web Application Firewall (WAF)
- Protects web servers from attacks like:
  - **SQL injection**
  - **XSS**
  - **DDoS**

### UTM (Unified Threat Management)
- Combines multiple security functions (malware, DLP, filtering).

### NGFW (Next-Gen Firewall)
- Uses **cloud-powered threat intelligence**.
- Deep packet inspection, user/app tracking.

---

## Tunneling Protocols

### TLS (Transport Layer Security)
- Uses certificates for secure connection establishment.

### IPSec
- Creates secure tunnels over IP networks.
- Key components:
  - **AH (Authentication Header)**: Integrity
  - **ESP (Encapsulated Security Payload)**: Encryption
  - **IKE (Internet Key Exchange)**: Sets up session using **DH over UDP port 500**

#### IPSec Modes
| Mode             | Description |
|------------------|-------------|
| **Tunnel Mode**  | Remote VPN, AH & ESP encrypted |
| **Always-on Mode** | Site-to-site VPN, constant connection |
| **Transport Mode** | Internal VPN, only ESP encrypted |

---

## Software-Defined WAN (SD-WAN)
- Protects traffic across dispersed branches, data centers, and cloud.
- Integrates firewalls and uses encryption for security.
- Supports centralized policy management.

---

## Secure Access Service Edge (SASE)
- Merges **WAN tech** and **cloud-based security**.
- Centralizes identity management and policies.
- Uses:
  - **IAM**
  - Intrusion prevention
  - Content filtering
  - Zero-trust model

---

These technologies form the backbone of enterprise network security and are critical for securing infrastructure against modern threats.
