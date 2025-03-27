# 📘 Study Guide: CISA's Defending Against Software Supply Chain Attacks

## 🧠 Key Concepts

- **Software Supply Chain Attack**: A cyberattack where the threat actor targets the software development or distribution process to compromise the final product.
- **Attack Surface**: Includes build systems, CI/CD pipelines, source code repositories, third-party components, and vendors.

---

## 🔍 Section Breakdown & Summary

### 📌 Introduction

- Modern software supply chains are increasingly targeted by advanced adversaries.
- Even trusted vendors and components can introduce risk.
- Notable examples: SolarWinds, NotPetya (via MeDoc), and CCleaner.

---

### 🧰 Recommended Practices (Across the Software Lifecycle)

#### 1. **Secure Development Practices**

- Use version control (e.g., Git) with access control
- Perform code reviews and dependency validation
- Avoid hard-coded secrets
- Scan for known vulnerabilities (e.g., using SCA tools)

#### 2. **Build Environment Security**

- Separate build and development environments
- Use ephemeral build environments
- Restrict build process internet access
- Implement signing for build artifacts

#### 3. **CI/CD Pipeline Security**

- Authenticate users and services
- Limit permissions and avoid long-lived credentials
- Secure the software signing process
- Monitor pipeline activity and logs

#### 4. **Use of Trusted Components**

- Prefer packages from trusted sources
- Validate integrity of third-party code
- Track open source licenses and risks

#### 5. **Deployment Best Practices**

- Use SBOMs (Software Bill of Materials)
- Enforce integrity checks and tamper detection
- Validate runtime behavior using monitoring or EDR tools

#### 6. **Operational Practices**

- Conduct regular audits and penetration testing
- Train developers and security teams
- Have an incident response plan for software supply chain attacks

---

## 🛠️ Security Tools and Techniques Highlighted

- Static/Dynamic Analysis (SAST/DAST)
- Software Composition Analysis (SCA)
- Container/image scanning
- Digital signing and verification
- Least privilege enforcement
- Audit trails and behavioral monitoring

---

## 🔗 Real-World Relevance to GRC

- **Vendor Risk Management**: Suppliers may unknowingly introduce malicious code.
- **Third-Party Risk**: Organizations must vet and monitor software providers and developers.
- **Compliance**: Many frameworks now reference secure SDLC, such as NIST 800-53, ISO 27001, and NIST CSF.

---

## 🧩 Framework Connections (Preview)

In `cisa-to-nist-crosswalk.md`, we'll map CISA recommendations to:

- 🔐 **NIST SP 800-53 Rev. 5** (e.g., SA-12, SR-3, CM-6)
- 🔄 **NIST CSF v1.1 or v2.0** (e.g., ID.SC-4, PR.DS-1, DE.CM-7)
- 🌐 **ISO/IEC 27001:2022** controls (Annex A)

---

## 📝 Next Steps

- Create crosswalks to NIST/ISO frameworks
- Build a checklist for vendor software risk evaluation
- Add diagrams to visualize supply chain threats

---
