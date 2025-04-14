# Domain 4: Security Operations – Study Guide
*Compiled on April 14, 2025*

This guide covers key Security+ Domain 4 topics with real-world examples and simplified breakdowns to help reinforce your learning.

---

## 🔍 Vulnerability Scans

### What is a Vulnerability Scan?
A vulnerability scan systematically probes systems for security weaknesses in software, configurations, or hardware. These scans help identify potential entry points for attackers.

---

### 🔓 Non-Credentialed Scan

- **Access Level**: Limited or external access (no login credentials).
- **Perspective**: Mimics what an external hacker sees.
- **Pros**:
  - Fast and low-impact.
  - Reveals exposed services and open ports.
- **Cons**:
  - Doesn’t catch internal misconfigurations or unpatched software.
  - Less accurate.
- **Use Case**: Perimeter security check of public-facing systems.

---

### 🔐 Credentialed Scan

- **Access Level**: Uses valid system credentials.
- **Perspective**: Trusted insider or admin.
- **Pros**:
  - In-depth inspection of configs, updates, and settings.
  - Detects outdated software, weak passwords, misconfigured permissions.
- **Cons**:
  - Takes longer, more setup required.
- **Use Case**: Internal systems security audit.

---

### 🚨 Benefits of Regular Vulnerability Scanning

- **Identifies Weak Points**: Detects outdated patches and misconfigurations.
- **Prioritizes Remediation**: Helps allocate resources using CVSS scores.
- **Supports Continuous Monitoring**: Keeps security posture strong.

---

### 🔧 Common Tools

- **Nessus**: Network-based scanner for both scan types.
- Demo: [https://www.tenable.com/products/nessus/demo](https://www.tenable.com/products/nessus/demo)

---

## 📦 SCAP: Security Content Automation Protocol

A framework that automates vulnerability checking and policy compliance.

### Components:

- **OVAL**: Open Vulnerability and Assessment Language
  - Evaluates system posture using XML schema.
  - [https://oval.mitre.org/](https://oval.mitre.org/)
- **XCCDF**: Extensible Configuration Checklist Description Format
  - Machine-readable best practice checklists.
  - [NIST SCAP Docs](https://csrc.nist.gov/projects/security-content-automation-protocol/specifications/xccdf)

---

## 🔥 Firewalls

Firewalls are the first line of defense, filtering network traffic based on rules.

### Types of Firewalls:

| Firewall Type             | Mission                                                        | Use Case                                                                 |
|--------------------------|----------------------------------------------------------------|--------------------------------------------------------------------------|
| **Host-Based**           | Protects individual devices                                    | Personal computers or endpoints                                          |
| **Network-Based**        | Protects entire networks                                       | Securing entry points and internal segments                             |
| **Stateful**             | Analyzes traffic in context (TCP sessions)                     | Preventing DDoS, inspecting traffic patterns                             |
| **Stateless**            | Basic packet filtering (source, destination, port)             | Quick decisions, low overhead                                            |
| **WAF**                  | Protects web applications from web-based attacks               | Blocking SQL injection, XSS, etc.                                        |
| **UTM**                  | All-in-one tool (malware, content filtering, URL blocking)     | Small-to-mid business all-purpose firewall                              |
| **NGFW**                 | Cloud-integrated, app-aware, deep inspection                   | Enterprise protection, cloud + on-premises hybrid environments          |

---

## 🧱 Firewall Rules

### Common Rule Types:

- **Inbound Rules**: What comes in (e.g., web server port 80 open to public).
- **Outbound Rules**: What leaves (e.g., users can access the internet).
- **Explicit Allow/Deny**: Specific entries that allow or block traffic.
- **Implicit Deny**: Default rule at the bottom — if no match, deny traffic.

> 🔁 *Example*: If no rule permits TCP port 21 (FTP), firewall blocks it by default = implicit deny.

---

### Rule Criteria:

- **Port Numbers**: E.g., port 443 for HTTPS.
- **Protocol Types**: E.g., TCP vs UDP.
- **IP Addresses**: Source or destination address.

---

## 📊 Port Numbers & Protocols

| Port Type            | Range          | Purpose/Example                          |
|----------------------|----------------|-------------------------------------------|
| **Well-Known Ports** | 0–1023         | HTTP (80), HTTPS (443), SMTP (25)        |
| **Registered Ports** | 1024–49151     | MySQL (3306), RDP (3389)                 |
| **Dynamic Ports**    | 49152–65535    | Temporary, client-side ports             |

---

### TCP vs. UDP

| Protocol | Reliable? | Method                     | Example Use Cases               |
|----------|-----------|----------------------------|----------------------------------|
| **TCP**  | Yes       | 3-way handshake (SYN, ACK) | Web browsing, file transfers     |
| **UDP**  | No        | Fire-and-forget            | Streaming, video conferencing    |

---

## 🌐 Zones

Networks are segmented into zones to separate trust levels.

| Zone           | Description                                                                 |
|----------------|-----------------------------------------------------------------------------|
| **WAN**        | Untrusted, public internet                                                  |
| **Screened Subnet (DMZ)** | Buffer zone between WAN and LAN. Hosts semi-public services like mail or web servers |
| **LAN**        | Trusted internal network with sensitive data                                |

Diagram:
- LAN ← Firewall → Screened Subnet ← Firewall → WAN

---

## 📋 ACL (Access Control List)

- **Purpose**: Defines who/what can access which resources.
- **Applies to**: Routers and firewalls.
- **Implicit Deny**: Blocks everything unless explicitly permitted.

---

## ✅ Final Tips

- Use **credentialed scans** for deep internal insight.
- **Implicit deny** always applies unless rules say otherwise.
- Know your **firewall types**, and what each does best.
- Understand how **ports and protocols** relate to services.
- Keep network zones and segmentation in mind for defense-in-depth.

---

*You're doing great — keep studying and come back to this guide when you need a refresh!*
