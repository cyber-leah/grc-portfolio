# 🔐 IAAA Model in Identity and Access Management (IAM)

The **IAAA model** is a foundational concept in Identity and Access Management (IAM). It outlines the four key processes that govern how individuals interact with secure systems and how their access is managed and monitored:

---

## 🔹 IAAA Stands For:
1. **Identification**
2. **Authentication**
3. **Authorization**
4. **Accountability**

---

## 1️⃣ Identification

**Identification** is the process of claiming an identity.

- It begins when a user provides a unique identifier such as a username, email, or user ID.
- This does **not verify** who the user is — it only states *who they say they are*.
- Example: Entering your email address on a login page.

🧠 *Think of identification as "Who are you claiming to be?"*

---

## 2️⃣ Authentication

**Authentication** is the process of proving that the identity claimed is valid.

- This is done by requiring **credentials** or proof, such as a password or biometric scan.
- Common factors used in authentication:
  1. **Something you know** (e.g., password, PIN)
  2. **Something you have** (e.g., smart card, token, phone)
  3. **Something you are** (e.g., fingerprint, facial recognition)

🔐 Additional lesser-used factors:
- **Somewhere you are** (e.g., IP address, GPS)
- **Something you do** (e.g., typing patterns, behavior-based auth)

🧠 *Authentication is the system saying: “Prove it.”*

---

## 3️⃣ Authorization

**Authorization** defines what an authenticated user is allowed to do.

- It assigns **permissions and roles** to users based on:
  - Job function
  - Department
  - Level of clearance
- Restricts access to resources the user doesn’t need.

🔓 Example: A developer can access dev tools, but not HR payroll files.

🧠 *"What are you allowed to access?"*

---

## 4️⃣ Accountability

**Accountability** ensures users are held responsible for their actions.

- Achieved by **logging**, **auditing**, and **monitoring** user activity.
- Helps trace actions in the event of:
  - A security incident
  - Unauthorized access
  - Policy violation

🧠 *"Can we prove what you did?"*

---

## 🔁 Why the IAAA Model Matters

- Prevents **unauthorized access** and **data breaches**
- Helps enforce **least privilege** and **role-based access control (RBAC)**
- Supports compliance efforts (HIPAA, PCI DSS, ISO 27001, etc.)
- Provides audit trails for accountability and forensic analysis

---

## ✅ Summary Table

| Step           | Description                                      | Example                      |
|----------------|--------------------------------------------------|------------------------------|
| Identification | Claiming an identity                            | Typing username              |
| Authentication | Proving the identity is real                    | Entering password or OTP     |
| Authorization  | Granting rights/permissions                     | Access to a specific folder  |
| Accountability | Tracking and logging user actions               | Log review, audit report     |

---

> 🧠 Created by Leah to understand the IAAA model and how it fits into secure system access and user accountability.
