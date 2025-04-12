# 🔐 Cryptography Folder - Study Notes by Leah

Welcome to my personal study notes on **cryptography**, created as part of my journey into cybersecurity and GRC (Governance, Risk, and Compliance). These markdown files cover foundational cryptographic tools, best practices for secure data handling, and real-world applications in auditing and compliance.

Each file in this folder is focused on a specific concept or tool, with examples, command usage, and plain-language explanations.

---

## 📁 File Overview

| File | Description |
|------|-------------|
| `RSA-key-breakdown.md` | Walkthrough of RSA private key components (`p`, `q`, modulus, etc.), including how to inspect them using OpenSSL. |
| `diffie-hellman-openssl.md` | How to generate and inspect Diffie-Hellman parameters (`P` and `G`) using OpenSSL. Explains the key exchange process. |
| `hmac-and-hashing.md` | Covers file integrity, HMAC vs hash functions, and how to use Linux tools like `sha256sum` and `hmac256`. |
| `password-authentication-guide.md` | Deep dive into secure password storage, including hashing, salting, peppering, and PBKDF2. Based on OWASP recommendations. |
| `pki-ssl-openssl.md` | Explains the use of PKI, SSL/TLS, certificate requests (CSR), self-signed certs, and how to inspect certs with OpenSSL. |
| `cryptography-and-data.md` | Describes what happens during HTTPS login, including certificate validation, TLS handshakes, and secure credential transmission. |
| `grc-cryptography-relationship.md` | Connects cryptographic concepts to GRC roles like auditing, compliance, and risk management. Explains how crypto practices map to frameworks like NIST, PCI DSS, and ISO 27001. |

---

## 🧠 Why This Folder Matters

These notes are designed to:
- Help me **retain and revisit** complex technical topics
- Serve as a **reference for future work** in GRC and security auditing
- Demonstrate my **technical depth and documentation skills** to employers

---

## 🧩 What’s Special About the `grc-cryptography-relationship.md` File?

This file brings it all together — it maps each cryptographic control (e.g., TLS, password hashing, cert validation) to its real-world relevance in:
- Internal audits
- Compliance assessments
- Risk mitigation strategies

This is especially useful for roles like:
- GRC Analyst
- Cybersecurity Auditor
- Compliance Specialist
- Risk Manager

---

> ✅ All content created and organized by Leah as part of her cybersecurity and GRC learning journey.
