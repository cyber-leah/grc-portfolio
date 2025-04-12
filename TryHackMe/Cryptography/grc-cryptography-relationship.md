# 🔐 GRC & Cryptography: The Relationship Between Security Controls and Crypto Practices

This guide explores how cryptography intersects with **Governance, Risk, and Compliance (GRC)** and how technical crypto practices (like password hashing, SSL/TLS, and PKI) map to real-world **auditing**, **risk mitigation**, and **regulatory compliance** efforts.

---

## 📘 Why Cryptography Matters to GRC

Cryptographic controls form the foundation of many critical GRC requirements. They help:
- **Enforce data confidentiality and integrity**
- **Verify authenticity and non-repudiation**
- **Protect personally identifiable information (PII)**
- **Demonstrate due diligence in safeguarding sensitive data**

---

## ✅ Cryptography in Compliance Frameworks

| Framework       | Cryptography-Related Requirements |
|-----------------|------------------------------------|
| **NIST SP 800-53**  | SC-12 (Cryptographic Key Establishment), SC-28 (Data Protection) |
| **PCI DSS**         | Requirement 3: Protect stored cardholder data (encryption & hashing) |
| **ISO/IEC 27001**   | Annex A.10: Cryptographic Controls |
| **HIPAA**           | §164.312(a)(2)(iv) Encryption and Decryption |
| **FedRAMP**         | Requires FIPS 140-2 validated encryption for federal systems |

---

## 🕵️ GRC Use Cases for Cryptography

### 🔐 1. **Password Security Controls**
- **Audit Criteria:** Are passwords salted and hashed using approved algorithms like bcrypt, Argon2, or PBKDF2?
- **Risk Mitigation:** Prevents credential stuffing, brute force, and post-breach password reuse.
- **Policy Enforcement:** Password storage policy should mandate salted hashing and key derivation functions.

---

### 🌐 2. **SSL/TLS Usage**
- **Audit Criteria:** Are TLS certificates valid, trusted, and using modern algorithms (TLS 1.2+)? Are expired/self-signed certs flagged?
- **Compliance Mapping:** Required by PCI DSS, ISO 27001, and SOC 2 to protect data in transit.
- **Risk Management:** Protects against eavesdropping and man-in-the-middle (MITM) attacks.

---

### 🧾 3. **Certificate Management**
- **Audit Criteria:** Is there a certificate lifecycle process? Are private keys stored securely (e.g., in HSMs or vaults)?
- **Compliance Reference:** NIST, CIS Controls, and ISO require proper key and certificate management.
- **Risk:** Poor certificate hygiene can lead to expired certs, broken trust chains, and exposed services.

---

### 🔐 4. **Secrets and Pepper Storage**
- **Audit Consideration:** Are application secrets like peppers stored securely (not in source code or databases)?
- **Control Mapping:** Secrets should be stored in encrypted vaults (e.g., AWS Secrets Manager, HashiCorp Vault).
- **Risk Tie-In:** Exposed secrets can compromise authentication and system access.

---

## 🧠 How GRC Professionals Benefit from Crypto Knowledge

- **Auditors** can validate technical controls more confidently.
- **Risk Managers** can model threats like credential compromise or MITM and assess cryptographic control strength.
- **Compliance Analysts** understand how encryption supports data protection clauses in legal and regulatory standards.
- **Policy Writers** can define cryptographic standards clearly and align them with best practices.

---

## ✅ TL;DR: GRC Meets Crypto

| Crypto Practice      | GRC Relevance                               |
|----------------------|---------------------------------------------|
| Password Hashing     | Password security policies, breach response |
| SSL/TLS              | Data in transit protection, vendor assessments |
| Certificate Management | Risk of expired/compromised certs         |
| Key & Secret Storage | Risk of leaked credentials or tampering     |
| FIPS/Validated Crypto| Federal & regulatory compliance requirements |

---

> 🧩 Created by Leah to bridge technical learning with real-world auditing, risk, and compliance practices in cybersecurity.
