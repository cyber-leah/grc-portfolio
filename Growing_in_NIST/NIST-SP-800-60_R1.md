# 🧠 NIST SP 800-60 Vol. 1 Rev. 1 Study Guide  
**Title:** *Guide for Mapping Types of Information and Information Systems to Security Categories*  
**Full PDF:** [NIST SP 800-60 Vol. 1 Rev. 1](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-60v1r1.pdf)

---

## 📚 What is SP 800-60?

NIST SP 800-60 is a **supporting guide** to **FIPS 199**, designed to help federal agencies:

- Categorize **information types** based on their **confidentiality, integrity, and availability** needs.
- Determine the **impact level (Low, Moderate, High)** for each security objective.
- Apply consistent, repeatable **security categorization** across all federal systems.

---

## 🧱 Key Concepts

### 🔐 Security Objectives (Same as FIPS 199)

| Objective       | Description                                                  |
|----------------|--------------------------------------------------------------|
| **Confidentiality** | Prevent unauthorized disclosure of information.              |
| **Integrity**       | Protect against unauthorized changes or destruction.         |
| **Availability**    | Ensure timely, reliable access to information and systems.    |

---

### 🔢 Information Type Categories

SP 800-60 provides **pre-defined information types**, such as:

- **Personal Identity and Authentication**
- **Law Enforcement**
- **Health Care Services Delivery**
- **Information System Development and Maintenance**
- **Financial Transactions and Reporting**

Each type includes guidance on **impact levels** for the three objectives.

---

### 🧩 The Mapping Process

1. **Identify Information Types** used by the system.
2. **Determine Impact Levels** for CIA for each type.
3. **Document Justifications** for selected levels.
4. **Derive Overall System Security Category** using highest impact value.

---

### 🔁 CIA Ratings for Information Types (Example)

> 👤 **Information Type: Personal Identity and Authentication**  
> - Confidentiality: **Moderate**  
> - Integrity: **Moderate**  
> - Availability: **Low**  
> ➡️ Security Category: **Moderate**

> 💸 **Information Type: Public Financial Reporting**  
> - Confidentiality: **Low**  
> - Integrity: **High**  
> - Availability: **Moderate**  
> ➡️ Security Category: **High**

---

## 📄 Volume 1 vs Volume 2

| Volume | Focus |
|--------|-------|
| **Vol. 1** | Overview and methodology for categorizing systems and information |
| **Vol. 2** | Reference tables with recommended impact levels for many info types |

You can find Volume 2 here: [SP 800-60 Vol. 2](https://csrc.nist.gov/publications/detail/sp/800-60/vol-2-rev-1/final)

---

## ✅ Why It Matters

- Enables **standardization** across agencies
- Supports the **Categorize** step of the **Risk Management Framework (RMF)**
- Helps ensure **appropriate security controls** are selected based on system sensitivity

---

## 🔗 Related Documents

- [FIPS 199](https://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.199.pdf): Defines the impact levels and security objectives
- [NIST SP 800-37](https://csrc.nist.gov/publications/detail/sp/800-37/rev-2/final): RMF process
- [NIST SP 800-53](https://csrc.nist.gov/publications/detail/sp/800-53/rev-5/final): Control catalog informed by impact levels

---

## 🏷 Tags  
`#NIST` `#FIPS199` `#SP80060` `#RMF` `#SecurityCategorization` `#GRC`

---

> _“Accurate impact categorization leads to meaningful risk mitigation.”_
