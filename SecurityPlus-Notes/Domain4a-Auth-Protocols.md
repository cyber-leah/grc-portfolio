## 🔐 Authentication Protocols

Authentication protocols define how devices, users, or systems verify identity before allowing access to a network or resource. These protocols are essential for maintaining secure wireless and enterprise environments.

---

### 🔄 802.1X
- A **port-based access control protocol** used to ensure that only authenticated devices can connect to a network.
- Often used in enterprise environments with **managed switches** and **RADIUS servers**.
- Requires a certificate installed on the endpoint (client device).

---

### 🧩 PEAP (Protected Extensible Authentication Protocol)
- Encapsulates EAP within a secure **TLS tunnel**.
- Adds protection to the authentication process by encrypting the inner EAP messages.
- Commonly used in WPA2-Enterprise networks.

---

### 🔒 EAP-TLS (Extensible Authentication Protocol - Transport Layer Security)
- One of the **most secure EAP methods**.
- Requires **certificates** on both the client and server side.
- Provides strong mutual authentication and is widely used in government and financial sectors.

---

### 🛡️ EAP-TTLS (Tunneled Transport Layer Security)
- Uses two phases:
  1. Sets up a **secure tunnel** using server-side certificates
  2. Then authenticates the client using usernames, passwords, or tokens
- Does not require client-side certificates.

---

### ⚡ EAP-FAST (Flexible Authentication via Secure Tunneling)
- Developed by Cisco.
- Does **not use certificates**.
- Uses **Protected Access Credentials (PACs)** to create a secure tunnel.
- Designed for fast and lightweight authentication.

---

## 🧠 Summary

| Protocol | Certificate Needed? | Notes |
|----------|---------------------|-------|
| **802.1X** | Yes (client) | Often used with RADIUS for port-based access control |
| **PEAP** | Server only | Uses TLS tunnel; hides inner authentication |
| **EAP-TLS** | Yes (client + server) | Very secure; strong mutual authentication |
| **EAP-TTLS** | Server only | Tunnel + secondary credentials (user/pass) |
| **EAP-FAST** | No | Uses PACs; designed for fast, secure, cert-less auth |

---

## 📚 Bonus:
- These protocols often appear on Security+ exam scenarios.
- Focus on **who provides the certificate**, how the tunnel is created, and **whether client credentials are exposed**.

