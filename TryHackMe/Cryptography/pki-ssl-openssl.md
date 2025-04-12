# 🔐 PKI, SSL/TLS, and Certificate Signing with OpenSSL

This guide covers the basics of **Public Key Infrastructure (PKI)**, **SSL/TLS certificates**, and how to generate and inspect them using OpenSSL. These skills are essential for roles in cybersecurity, compliance, and DevSecOps.

---

## 📘 What is PKI?

**Public Key Infrastructure (PKI)** is a framework that enables secure communication and authentication across networks using asymmetric encryption (public/private key pairs). It supports:

- **Confidentiality**: Encrypting communication
- **Authentication**: Verifying identities with digital certificates
- **Integrity**: Ensuring data hasn't been altered
- **Non-repudiation**: Proving a sender’s identity and action

PKI is the backbone of **SSL/TLS**, email encryption, secure software updates, and more.

---

## 🔐 What Is an SSL/TLS Certificate?

An **SSL/TLS certificate** is a digital certificate that:
- Confirms the identity of a website or service
- Enables encrypted HTTPS connections between clients and servers

It contains:
- A **public key**
- The **subject** (organization/domain)
- The **issuer** (usually a Certificate Authority)
- Validity dates
- Signature and fingerprint

---

## 🧾 Certificate Signing Request (CSR)

To get a certificate signed by a trusted CA, you must first generate a CSR.

### 🔧 Generate a CSR and RSA Key (4096-bit)

```bash
openssl req -new -nodes -newkey rsa:4096 -keyout key.pem -out cert.csr
```

#### Options:
- `-req`: generate a certificate request
- `-nodes`: skip password protection for private key (not secure in production!)
- `-newkey rsa:4096`: generate a new RSA key (4096-bit)
- `-keyout`: where to save the private key
- `-out`: output the CSR

You'll be prompted for info such as:
- Country, State, Organization
- Common Name (typically the domain)
- Email (optional)

---

## 📄 Self-Signed Certificate (For Testing)

For internal or test environments, you can create a self-signed certificate:

```bash
openssl req -x509 -newkey rsa:4096 -nodes -keyout key.pem -out cert.pem -sha256 -days 365
```

- `-x509`: create a self-signed cert instead of a CSR
- `-sha256`: use SHA-256 digest
- `-days 365`: valid for 1 year

---

## 🕵️‍♀️ Inspect a Certificate

To view details of a certificate (like the issuer, subject, validity, etc.):

```bash
openssl x509 -in cert.pem -text
```

You’ll see:
- Serial number
- Validity period
- Subject/Issuer fields
- Public key details
- Signature algorithm

---

## 🏛️ Certificate Authority (CA)

In production, self-signed certs aren’t trusted. Instead, you:
1. Generate a CSR (certificate signing request)
2. Send it to a **trusted Certificate Authority (CA)** (e.g., DigiCert, Let's Encrypt)
3. The CA signs your cert and returns it
4. Clients (like web browsers) check their list of trusted CAs — if the CA is known, the connection is trusted

---

## ✅ Real-World Relevance (GRC & Security Roles)

Knowing this process helps with:
- **Auditing certificate expiration and usage**
- **Validating secure HTTPS implementations**
- **Supporting SOC 2, PCI DSS, FedRAMP, and ISO 27001 compliance**
- **Detecting weak keys or self-signed certs in scans**
- Writing or reviewing security policies for key and cert management

---

## 🧪 Key Terms Recap

| Term        | Meaning                                                      |
|-------------|---------------------------------------------------------------|
| PKI         | Public Key Infrastructure                                     |
| CSR         | Certificate Signing Request                                   |
| CA          | Certificate Authority                                         |
| x509        | Standard for public key certificates                          |
| SHA256      | Cryptographic hash used in signatures                         |
| `key.pem`   | Your private key                                              |
| `cert.pem`  | Your certificate (signed or self-signed)                      |

---

> 💡 Tip: Always keep private keys secure, and monitor certificate expiration in production environments.

---

### ✅ Created by Leah for her cybersecurity portfolio. Learning and applying OpenSSL, PKI, and SSL/TLS one command at a time.
