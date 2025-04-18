# 🛡️ GDPR & PCI DSS Study Guide

This study guide covers the fundamentals of the **General Data Protection Regulation (GDPR)** and the **Payment Card Industry Data Security Standard (PCI DSS)**, two of the most widely implemented data protection and privacy frameworks in the world.

---

## 🇪🇺 General Data Protection Regulation (GDPR)

**GDPR** is a data protection law enforced by the European Union (EU) since May 2018. It governs how organizations collect, store, process, and transfer personal data of individuals residing in the EU.

### 📌 Key Principles of GDPR

- **Prior approval** must be obtained before collecting personal data.
- Data collection must be **minimal** and **necessary** for a specific purpose.
- Organizations must implement **adequate protection measures** for stored personal data.

### 🔐 Core Rights and Obligations

| GDPR Focus Area | Description |
|------------------|-------------|
| **Data subject rights** | Individuals have rights to access, correct, or delete their personal data. |
| **Lawful processing** | Personal data must be collected and used lawfully and transparently. |
| **Personal data breaches** | Organizations must report data breaches promptly. |
| **Limitation of purpose, data, and storage** | Data must only be collected for specific, clear purposes. |
| **Data protection impact assessment** | Required for high-risk data processing activities. |
| **Consent** | Must be freely given, specific, informed, and unambiguous. |
| **Data protection officer (DPO)** | Some organizations must designate a DPO. |
| **Privacy by design** | Data protection must be built into systems and processes. |
| **Awareness and training** | Staff must be trained to handle data securely. |
| **Data transfer** | Rules govern transfers of personal data outside the EU. |

### 💸 GDPR Penalties

GDPR violations are enforced under a **two-tiered penalty system**:
- **Tier 1**: Up to 4% of global revenue or €20 million (whichever is higher) for serious violations (e.g., unlawful processing, consent failure).
- **Tier 2**: Up to 2% of global revenue or €10 million for lesser violations (e.g., inadequate breach notification).

🔗 Learn more: [GDPR Info](https://gdpr-info.eu/)

---

## 💳 Payment Card Industry Data Security Standard (PCI DSS)

**PCI DSS** is a global standard for protecting cardholder data, developed by major credit card companies (Visa, Mastercard, AmEx, etc.).

### 🛠 PCI DSS Overview

- Applies to any business **that stores, processes, or transmits credit card data**.
- Ensures card data is protected from theft, fraud, and unauthorized access.

### 📋 Key Requirements

| Control Area | Example Measures |
|--------------|------------------|
| **Access Control** | Restrict access to cardholder data by business need-to-know. |
| **Encryption** | Encrypt transmission of cardholder data across open networks. |
| **Monitoring and Logging** | Track and monitor all access to network resources and cardholder data. |
| **Vulnerability Management** | Regularly update systems and apply security patches. |
| **Security Testing** | Conduct vulnerability scans and penetration testing. |
| **Authentication** | Require strong passwords and multifactor authentication. |

### 🔐 Tools Often Used to Meet PCI DSS
- Web application firewalls (WAF)
- Encryption protocols (e.g., TLS)
- Security Information and Event Management (SIEM)
- Antivirus and patch management solutions

🔗 PCI DSS Quick Guide: [PCI DSS v4.0 QRG](https://docs-prv.pcisecuritystandards.org/PCI%20DSS/Supporting%20Document/PCI-DSS-v4_x-QRG.pdf)

---

## 🧠 Summary

| Framework | Focus | Applies To |
|----------|-------|------------|
| **GDPR** | Personal data privacy and protection | Any organization handling EU residents’ data |
| **PCI DSS** | Credit card data security | Any organization processing card payments |

---

*Tip: For compliance roles, understand which controls (e.g., encryption, breach response) overlap between GDPR and PCI DSS, and tailor your documentation and training accordingly.*
