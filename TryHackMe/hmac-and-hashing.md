# 🔐 HMAC and Hash Functions in Linux (TryHackMe Summary)

This guide covers how to calculate HMACs and SHA256 hashes using command-line tools, as well as a quick breakdown of how HMACs work internally. Based on practical examples from TryHackMe.

---

## 🧾 What is HMAC?

**HMAC** (Hash-based Message Authentication Code) is a type of message authentication code that combines:
- A **cryptographic hash function** (e.g., SHA-256)
- A **secret key**

HMAC is commonly used for:
- API request signing
- Message integrity
- Authentication

---

## 📐 How HMAC Works (RFC2104 Overview)

1. **Pad the key** with zeroes to the block size (B).
2. Create two padded keys:
   - `ipad`: inner pad (`0x36` repeated B times)
   - `opad`: outer pad (`0x5C` repeated B times)
3. `key ⊕ ipad` → Append the message → Hash it → call this `inner`
4. `key ⊕ opad` → Append `inner` → Hash again → final HMAC

---

## 💻 Linux HMAC Commands

### ✅ Using `hmac256`

```bash
hmac256 SECRETKEY filename
```

Example:
```bash
hmac256 1234 message.txt
```

### ✅ Using `sha256hmac`

```bash
sha256hmac filename --key SECRETKEY
```

Or:
```bash
sha256hmac filename --key 1234
```

---

## 🧪 File Integrity with SHA256

You can also use `sha256sum` to get the checksum of a file:

```bash
sha256sum file.txt
```

Example output:
```
f4616fd825a10ded9af58fbaee09f3e31751d15591f9323ea68b03a0e8ac3783  file.txt
```

---

## 🔍 Even Minor Differences Matter

Two files that look the same might have different checksums due to invisible differences (like uppercase vs lowercase):

```bash
hexdump text1.txt -C
hexdump text2.txt -C
sha256sum text1.txt
sha256sum text2.txt
```

---

## 📚 Tools You Can Use (as seen in TryHackMe)

- `hmac256`
- `sha256hmac`, `sha384hmac`, `sha512hmac`
- `sha256sum`
- `hexdump -C`

---

### ✅ Created by Leah as part of her hash functions learning notes.
