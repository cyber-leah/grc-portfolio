# 🔐 FIDO2 and WebAuthn Overview

This page summarizes **FIDO2** and **WebAuthn**, modern authentication standards designed to replace passwords and make logins more secure and user-friendly.

---

## 🧩 What is FIDO2?

**FIDO2** is a set of authentication standards developed by the **FIDO Alliance** and the **World Wide Web Consortium (W3C)**.  
It allows users to log in to websites and services using a device they **have** (like a phone or security key) and/or something they **are** (like a fingerprint), without relying on traditional passwords.

FIDO2 has two main parts:
- **WebAuthn (Web Authentication API):**  
  - A standard for browsers and servers that lets users log in with biometrics, security keys, or PINs.
- **CTAP (Client to Authenticator Protocol):**  
  - Allows devices like security keys (e.g., YubiKeys) to interact with a computer or phone.

---

## 📚 How FIDO2/WebAuthn Work

Instead of sending a password over the internet, FIDO2 uses **public key cryptography**:
- Your device generates a key pair: a public key (shared with the server) and a private key (kept secure on your device).
- When you log in, your device proves ownership of the private key without sending it.

This method is **phishing-resistant** and **much harder to hack**.

---

## ✅ Real-Life Examples

- Using **Face ID** or **fingerprint** to sign into a website
- Logging into a service by **tapping a USB security key**
- Approving a login from your phone without typing anything

---

## 🧠 Why FIDO2 Matters

| Advantage              | Explanation |
|-------------------------|-------------|
| No passwords to steal   | Reduces risk of data breaches and credential theft |
| Phishing-resistant      | Protects against fake websites and login scams |
| Faster and easier       | Improves user experience without sacrificing security |

---

## 📘 Related Standards
- [NIST SP 800-63-3: Digital Identity Guidelines](https://pages.nist.gov/800-63-3/)
- [FIDO Alliance Official Site](https://fidoalliance.org/)
- [WebAuthn Overview (W3C)](https://www.w3.org/TR/webauthn/)

---

## 📚 Sources
- FIDO Alliance. (n.d.). [FIDO2: Moving the World Beyond Passwords](https://fidoalliance.org/fido2/)
- W3C. (n.d.). [Web Authentication: An API for accessing Public Key Credentials](https://www.w3.org/TR/webauthn/)
