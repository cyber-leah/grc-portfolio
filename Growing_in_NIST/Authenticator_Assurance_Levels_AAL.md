# 🔐 Authenticator Assurance Levels (AAL) – NIST SP 800-63-3

This page summarizes the three Authenticator Assurance Levels (AALs) defined in [NIST SP 800-63-3](https://pages.nist.gov/800-63-3/sp800-63b.html). These levels help determine how strong authentication needs to be based on the **risk of the service or system being accessed**.

---

## 📊 What is AAL?

**AAL** stands for **Authenticator Assurance Level**.  
It refers to how strong or trustworthy an authentication process is, and how resistant it is to impersonation or attack.

---

## 🧱 The 3 AAL Levels

### ✅ AAL1 – Basic Assurance
- **Used for:** Low-risk activities (e.g., viewing public data or basic account functions)
- **Authentication Example:** 
  - Password
  - One-Time Password (OTP) via email or SMS
- **Goal:** Basic protection without adding too much burden to the user

---

### ✅ AAL2 – Moderate Assurance
- **Used for:** Medium-risk actions (e.g., accessing personal records, updating payment info)
- **Authentication Example:** 
  - Password **plus** a second factor like:
    - OTP app (e.g., Google Authenticator)
    - Biometrics (fingerprint, face scan)
- **Goal:** Stronger protection against stolen credentials

---

### ✅ AAL3 – High Assurance
- **Used for:** High-risk or sensitive systems (e.g., government databases, financial platforms)
- **Authentication Example:** 
  - Cryptographic hardware (e.g., smart card, hardware token)
  - Biometric or PIN (in combination with the device)
- **Goal:** Maximum protection with resistance to phishing and replay attacks

---

## 🔍 Summary Table

| Level | Risk Type       | Example Use                   | Authentication Example                  |
|-------|------------------|-------------------------------|------------------------------------------|
| AAL1  | Low              | Basic services                | Password or OTP (email/SMS)              |
| AAL2  | Moderate         | Personal/account settings     | Password + OTP app or biometrics         |
| AAL3  | High             | Sensitive or critical systems | Hardware token + biometric or PIN        |

---

## 🧠 Why AALs Matter

Using the right AAL helps protect data while keeping login methods manageable for users. Not every service needs the same level of security — **AALs help tailor authentication to the risk involved**.

---

## 📚 Source  
[NIST SP 800-63B: Digital Identity Guidelines – Authentication and Lifecycle Management](https://pages.nist.gov/800-63-3/sp800-63b.html)

