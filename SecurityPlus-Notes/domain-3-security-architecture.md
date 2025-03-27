
# Domain 3: Security Architecture

## Access Control

Access control refers to the process of allowing or restricting access of different parties to the organization’s data, applications, network, or the cloud based on the organization’s policies. There are two factors that are used to complete this task: the Access Control List (ACL) and permissions.

ACLs are lists used by routers and firewall devices to grant or deny network traffic based on a set of rules. There are two different kinds of ACLs, one for files and folders and another for incoming network traffic.

- **Data Access ACL**: Implemented in file and data access environments to control who gets access to the different types of data and restrict what level of access they get. Access is allotted according to the principle of least privilege.
- **Network ACL**: Implemented in a network environment and placed on the firewall or router. It generally starts with a "deny all" rule, with exceptions explicitly added as allow rules.

## Mitigation Techniques

Access control includes permissions (read, write, execute, delete) based on job roles. Permissions help protect against unauthorized data tampering and ensure the security of sensitive information.

### Application Allow List

This allows only pre-approved applications to run, blocking unauthorized software. Whitelisting can prevent users from accidentally executing malware.

## Data Decommissioning and Sanitization

- **Paper sanitization**: Prefer cross-cut shredders or burning.
- **Media sanitization**: Overwrite, format, or wipe; least secure is degaussing.
- **Effective decommissioning**: Reduces attack surface and operational costs.

## Hardening Techniques

- **Encryption**: Converts data to ciphertext to protect confidentiality and integrity.
- **Endpoint Detection and Response (EDR)**: Uses AI/ML for detection, continuous monitoring, behavioral analysis, threat detection, forensic analysis, and alert generation.
- **Host-Based Intrusion Prevention System (HIPS)**: Monitors at host level.
- **Host-based firewall**: Filters traffic per device.
- **Disabling ports/protocols**: Minimizes attack surface.
- **Removing unnecessary software**: Reduces vulnerabilities.
- **Changing default passwords**: Prevents unauthorized access.

## Cloud Service Models

- **IaaS**: Network infrastructure (e.g., storage, servers).
- **SaaS**: Web-accessed apps (e.g., Salesforce).
- **PaaS**: App dev tools and environment (e.g., Azure App Services).
- **SECaaS**: Identity and Access Management (IAM).
- **XaaS**: Covers additional services like NaaS, DaaS, BaaS.

## Responsibility Matrix

| Domains                     | Customer | Cloud Service Provider |
|----------------------------|----------|-------------------------|
| Physical Security          |          | Yes                     |
| IAM                        | Yes      | Yes                     |
| Security Monitoring        |          | Yes                     |
| Application Security       | Yes      |                         |
| Configuration Management   | Yes      | Yes                     |
| Incident Response          |          |                         |
| Awareness Training         | Yes      |                         |
| Maintenance                |          | Yes                     |

## Infrastructure Concepts

- **Infrastructure as Code (IaC)**: Uses code for automation, consistency, and scalability.
- **Serverless**: CSP manages infrastructure. Backend-as-a-Service reduces management burden.
- **SDN (Software-Defined Networking)**: Separates planes (management, control, data) for dynamic routing and traffic control.

## SCADA Systems

Levels:
- **Level 0**: Plant level (sensors, actuators).
- **Level 1**: Controller level (PLCs).
- **Level 2**: Coordinating level (HMI, supervisory control).
- **Level 3**: Program Logic Controller (advanced control and analytics).

Targeted sectors: Energy, Facilities, Manufacturing, Logistics, Industrial.

## Device Placement & Zones

- **LAN**: Trusted zone.
- **DMZ**: Screened subnet.
- **WAN**: Untrusted zone.

### Security Zones
- Segmentation, data protection (FDE, DLP), access control.

## Device Attributes

- **Active**: Firewalls, IPS.
- **Passive**: IDS.
- **Inline**: Load balancer, firewall appliances.
- **Tap/Monitor**: Packet analyzers.

## Network Appliances

- **Jump Server**: Manages internal resources via RDP/SSH.
- **Proxy Server**: Intermediary for web access, URL filtering.
- **Reverse Proxy**: Handles incoming internet traffic.
- **IPS/IDS**: Intrusion prevention/detection.
- **Load Balancer**: Layer 4 and Layer 7 distribution.
- **Sensors**: Detect anomalies.

## Port Security

- Sticky MAC, disabling ports, 802.1x authentication, EAP types (EAP-TLS, EAP-PEAP, EAP-MD5).

## Firewalls

- **WAF**: Protects web applications.
- **UTM**: Unified Threat Management.
- **NGFW**: Next-gen firewalls with threat intelligence.
- **Layer 4 Firewall**: Stateless, filters by port/IP.
- **Layer 7 Firewall**: Application layer, deep packet inspection.

## Tunneling & VPNs

- **TLS**: Uses certs for encrypted tunnels.
- **IPSec**: AH, ESP, optional trailer.
- **IKE**: Uses DH over UDP port 500.
- Modes:
  - Tunnel Mode: Remote user VPN.
  - Always-on Mode: Site-to-site VPN.
  - Transport Mode: Internal communication.

## SD-WAN & SASE

- **SD-WAN**: Encrypts data over WANs, manages network policies.
- **SASE**: Combines WAN + IAM + zero-trust + threat prevention.

## Data Protection Types

- PII, PHI, Financial, Legal, IP, Consumer, Government, Trade secrets, Customer, Proprietary, Biometric.

## Clustering

- **Active-passive node config**, **quorum disk**, **witness server**, **heartbeat**, **VIP**.

## Cloud Data Replication

- **LRS**: Local.
- **ZRS**: Zone.
- **GRS**: Geo.
- **GZRS**: Geo + Zone.

## Platform Diversity & Multi-Cloud

- Diversity improves redundancy, adaptability, compliance.
- Multi-cloud improves uptime, flexibility, avoids vendor lock-in.
