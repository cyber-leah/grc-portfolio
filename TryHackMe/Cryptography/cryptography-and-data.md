# 🔐 Cryptography and Data: SSL/TLS, Certificates, and Secure Login

This guide focuses on how cryptography protects data during login over HTTPS, especially the role of SSL/TLS certificates, handshakes, and how passwords are securely transmitted and stored.

---

## 🌐 HTTPS and SSL/TLS Certificate Exchange

When you log into a secure website (HTTPS), a cryptographic process begins to protect your data:

### 🛠 Step-by-step Breakdown:

1. **Client requests the server’s SSL/TLS certificate**
2. **Server sends its SSL/TLS certificate** to the client
3. **Client checks if the certificate is valid** (i.e., signed by a trusted Certificate Authority)

---

## 📜 Certificate Validation (Trust Chain)

- A certificate is **valid** if it is **digitally signed** by a **trusted CA** (Certificate Authority).
- Signing involves hashing the certificate and encrypting the hash with the CA’s **private key**.
- The client then:
  - Uses the **CA’s public key** to decrypt the signature
  - Compares the decrypted hash with its own hash of the certificate
- If these match → the cert is trusted.

> ❌ If the CA isn’t trusted or the cert is altered, the connection will be **blocked** or a warning is shown.

---

## 🤝 SSL/TLS Handshake (After Trust is Established)

Once the certificate is verified, the **SSL/TLS handshake** begins. This handshake:
- Negotiates cryptographic algorithms
- Uses **asymmetric encryption** to exchange a symmetric key
- Establishes a **shared session key** for the rest of the session

From here on, all communication is encrypted using **symmetric encryption** (faster for bulk data).

---

## 🔐 Secure Login with SSL/TLS

Once the secure channel is established:
- The client sends **login credentials (username + password)** through the encrypted SSL/TLS tunnel
- The server receives the data securely and checks credentials

> This protects login details from being intercepted over the internet (e.g., by attackers on public Wi-Fi).

---

## 🧂 Password Handling on the Server

Even though the password was encrypted during transmission, servers must still **securely store** it to protect it long-term.

### ✅ Best Practices:
- Never store plaintext passwords
- Always store a **hashed version** of the password
- Append a **random salt** before hashing

Example flow:
```plaintext
password → hash(password + salt) → stored in DB
```

If an attacker gets access to the database, they still have to:
- Crack the hash
- Guess the correct password
- Deal with salting and (potentially) peppering

---

## 📚 Bonus Knowledge

- HTTPS uses **TLS (Transport Layer Security)**, which is the successor to SSL.
- Public-key cryptography is only used for the initial handshake — after that, TLS uses **symmetric encryption** for performance.
- The most secure implementations use **TLS 1.2 or TLS 1.3**.
- Common algorithms used include **RSA**, **ECDSA**, **AES**, and **SHA-256**.

---

## ✅ TL;DR: How Cryptography Secures a Login

| Step                          | Purpose                                     |
|-------------------------------|---------------------------------------------|
| SSL/TLS certificate exchange | Ensures server identity is trusted          |
| TLS handshake                | Securely exchanges session key              |
| Symmetric encryption         | Protects data during the session            |
| Password hashing & salting   | Secures credentials after login             |

---

> 🧠 Created by Leah to understand how cryptography protects real-world user data during login and beyond.
