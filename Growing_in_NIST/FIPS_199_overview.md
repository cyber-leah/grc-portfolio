# 📘 FIPS 199 Study Guide  
**Standard:** Federal Information Processing Standards (FIPS) Publication 199  
**Full Title:** *Standards for Security Categorization of Federal Information and Information Systems*  
**Link:** [FIPS 199 PDF](https://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.199.pdf)

---

## 🔍 What is FIPS 199?

FIPS 199 is a **NIST-issued federal standard** that establishes **requirements for categorizing information and information systems** based on the impact of potential security breaches.

It is the **first mandatory standard** under the **Federal Information Security Modernization Act (FISMA)** and serves as the **starting point for the NIST Risk Management Framework (RMF).**

---

## 🎯 Purpose of FIPS 199

To provide a consistent standard for:

- Determining the **security category** of federal information and systems
- Laying the groundwork for selecting appropriate **security controls**
- Supporting organizational **risk assessments** and **system security planning**

---

## 🧱 Core Concepts

### 🔐 Security Objectives

FIPS 199 uses three key security objectives:

| Objective       | Description                                                  |
|----------------|--------------------------------------------------------------|
| **Confidentiality** | Protection from unauthorized disclosure of information       |
| **Integrity**       | Protection from unauthorized modification or destruction     |
| **Availability**    | Timely and reliable access to information and systems        |

---

### 📈 Impact Levels

Each objective is assigned an impact level:

| Level   | Meaning                                                                 |
|---------|-------------------------------------------------------------------------|
| **Low**      | Limited adverse effect                                              |
| **Moderate** | Serious adverse effect                                              |
| **High**     | Severe or catastrophic adverse effect                               |

---

> 📌 **Example: Categorizing System X**
> 
> ```
> System X:
> - Confidentiality: Moderate
> - Integrity: High
> - Availability: Moderate
> 
> => Overall Security Category = **High**
> ```
> 
> 🔺 *The highest impact level (Integrity = High) sets the overall security category for the system.*

### 📐 Security Categorization Formula

```plaintext
Security Category (SC) = {(confidentiality, impact), (integrity, impact), (availability, impact)}
