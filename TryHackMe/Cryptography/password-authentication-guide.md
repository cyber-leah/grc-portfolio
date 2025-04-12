# 🔐 Password Authentication & Secure Storage Study Guide

This study guide summarizes core concepts from the OWASP Password Storage Cheat Sheet and expands on important practices like **salting**, **peppering**, **hashing**, and **why encryption isn't a substitute for hashing** when handling user passwords.

---

## 📌 Password Hashing vs Encryption

| Method     | Description                                       | Reversible? |
|------------|---------------------------------------------------|-------------|
| Hashing    | One-way function used to store passwords securely | ❌ No        |
| Encryption | Two-way function used to protect data             | ✅ Yes       |

### 🧠 Key Points:
- **Passwords should be hashed, NOT encrypted.**
- Hashing ensures passwords can't be "decrypted" by an attacker.
- Encryption should only be used when the original plaintext password **must be retrieved** (e.g., for legacy systems or federation protocols like OpenID Connect).
- Hashing is safer for user authentication, even if the hash is stolen.

---

## 🧂 What is Salting?

**A salt** is a unique, randomly generated value added to each password **before hashing**.

### 🎯 Benefits of Salting:
- Prevents attackers from using precomputed hash tables (rainbow tables).
- Makes each stored password hash **unique**, even if two users have the same password.
- Slows down mass cracking attempts — attackers must brute-force each password individually.

### 🔒 Best Practices:
- Use a **unique salt per user**.
- Don't reuse salts.
- Let modern algorithms like Argon2id, bcrypt, or PBKDF2 handle salting automatically.

---

## 🌶️ What is Peppering?

**Peppering** is a technique used in addition to salting that involves applying a secret value (the pepper) to the password or its hash.

### 🔐 Key Differences:
- A **salt** is unique per user and stored in the database.
- A **pepper** is **shared across users** and **NOT stored** in the database.
- Pepper is treated like a secret key and stored securely (e.g., HSM or secrets manager).

### 🧰 Example Strategy:
```plaintext
password → hash(password + salt) → HMAC(hashed_pw, pepper)
```

### 🔁 Rotate the Pepper:
Like any secret key, **pepper rotation** should be part of your key management strategy.

---

## 🧪 Improved Hashing Strategy

Use **Key Derivation Functions (KDFs)** like:

- **PBKDF2**
- **bcrypt**
- **scrypt**
- **Argon2id** (recommended modern choice)

### Example Workflow:
```plaintext
hash(hash(password) + salt)
→ run through PBKDF2 or Argon2id
→ store the final hash and salt
```

Modern KDFs:
- Apply thousands (or millions) of iterations
- Automatically include salts
- Are designed to resist GPU and ASIC cracking

---

## 📘 References & Further Reading

- 🔗 [OWASP Password Storage Cheat Sheet](https://cheatsheetseries.owasp.org/cheatsheets/Password_Storage_Cheat_Sheet.html)
- 🔐 [Secrets Management Cheat Sheet (OWASP)](https://cheatsheetseries.owasp.org/cheatsheets/Secrets_Management_Cheat_Sheet.html)

---

## ✅ TL;DR: What to Do for Secure Password Handling

| Technique        | Use it for...                             | Where it goes           |
|------------------|-------------------------------------------|--------------------------|
| Hashing          | Validating passwords                      | Stored in DB             |
| Salting          | Making hashes unique per user             | Stored in DB (per user)  |
| Peppering        | Adding an extra layer of protection       | Stored securely (e.g., HSM) |
| KDF (PBKDF2 etc.)| Stretching passwords & increasing cost    | Combined with hashing    |

---

> 🧠 Created by Leah as part of her password security learning series.
