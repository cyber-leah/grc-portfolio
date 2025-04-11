# 🔐 RSA Key Breakdown: Understanding `p` and `q` in a Private Key

This guide explains how to inspect an RSA private key and find values like `p` and `q` using OpenSSL. It's based on a TryHackMe challenge and will help you remember what these values mean and how to extract them.

---

## 📌 Why `p` and `q` Matter

In RSA encryption:

- `p` and `q` are **large prime numbers** randomly chosen when generating a key pair.
- They are used to calculate:
  - The **modulus (n)**: `n = p × q`
  - The **private exponent (d)`**, which is part of the private key
- If an attacker discovers `p` and `q`, they can factor `n` and **break the encryption**.

So, `p` and `q` are **super sensitive parts** of the RSA private key.

---

## 🧪 How to Inspect an RSA Private Key

### 🔧 Step 1: View the Full Key Breakdown

```bash
openssl rsa -in private-key.pem -text -noout
```

Replace `private-key.pem` with your file (e.g., `private-key-bob.pem`).

This will show a full breakdown of:
- Modulus
- Public Exponent (usually `65537`)
- Private Exponent
- **Prime1 (p)**
- **Prime2 (q)**
- Exponents and Coefficients used for CRT (Chinese Remainder Theorem)

---

### 🔍 Step 2: Find the Last Byte of `p` and `q`

Scroll to the `prime1:` and `prime2:` sections in the output.

Example:
```
prime1:
    00:d1:28:cb:6a:e7:1b:...:**3a**
prime2:
    00:cd:bb:6f:a9:e2:2f:...:**4c**
```

➡️ The **last byte** is the final hex pair:
- For `prime1`, last byte = `3a`
- For `prime2`, last byte = `4c`

Just strip the colons and grab the final pair. That’s your answer!

---

## 🧠 TL;DR: Commands

```bash
# View key structure and primes
openssl rsa -in private-key.pem -text -noout

# Look for these sections in the output:
# prime1: → value of p
# prime2: → value of q
```

---

## 🧩 Real-World Relevance

Understanding this helps with:

- Key audit & review
- Compliance reporting (PCI, SOC 2, etc.)
- Recognizing how private keys work under the hood
- Explaining cryptography concepts to non-technical stakeholders
- Becoming confident in OpenSSL usage for security tasks

---

> 💡 Tip: RSA private keys contain more than just a "secret key" — they contain a mini math world inside them.

---

### ✅ Created by Leah as part of her cybersecurity learning journey.
