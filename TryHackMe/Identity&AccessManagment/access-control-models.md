# 🔐 Access Control Models: DAC, RBAC, and MAC

Access control models are used to manage how users gain access to information, systems, and resources within an organization. These models define **who can access what**, and under which circumstances.

---

## 📘 1. Discretionary Access Control (DAC)

**Discretionary Access Control** allows the **resource owner** (user or application) to decide who gets access.

### Characteristics:
- Users can **grant or revoke access** to others.
- Control is **flexible** but **less secure**.
- Common in home or small team environments.

### Example:
You upload graduation photos to a cloud album and manually give viewing rights to specific family members.

### Pros:
- Easy to implement and understand
- Ideal for personal or small-scale environments

### Cons:
- Not scalable for large organizations
- Security risk if users misconfigure access

---

## 👥 2. Role-Based Access Control (RBAC)

**RBAC** assigns permissions based on the **user’s role** within the organization.

### Characteristics:
- Access is tied to **job function or department**
- Roles define what users **can and cannot do**
- Central to many enterprise IAM systems

### Example:
An accountant is assigned the “Finance” role and gains access to accounting systems, but not engineering files.

### Pros:
- Scalable and easy to manage
- Efficient for onboarding/offboarding
- Supports least privilege

### Cons:
- Rigid in dynamic environments
- Needs regular role review to avoid privilege creep

---

## 🔒 3. Mandatory Access Control (MAC)

**MAC** is the most restrictive model, used in high-security environments like the military.

### Characteristics:
- Access decisions are **centralized and enforced by system policies**
- Based on **classification labels** (e.g., Confidential, Secret)
- Users **cannot alter access rights**

### Example:
A government employee with a “Secret” clearance can only access documents labeled “Secret” or below.

### Implementations:
- **SELinux**: Enforces MAC on Red Hat, Fedora
- **AppArmor**: Used on Debian, Ubuntu

### Pros:
- Highest level of control and enforcement
- Prevents unauthorized information flow

### Cons:
- Complex to implement and manage
- Not suitable for flexible environments

---

## 🧠 Access Control Comparison Table

| Feature              | DAC                      | RBAC                         | MAC                                |
|----------------------|--------------------------|-------------------------------|-------------------------------------|
| Control By           | Owner (user)             | Role assigned by admin        | System (policy-based)               |
| Flexibility          | ✅ High                   | ⚖️ Moderate                   | ❌ Low                              |
| Security Level       | ⚠️ Lower                  | ✅ Strong                     | 🔒 Very High                        |
| Use Case             | Small teams, personal use| Enterprises, business systems | Military, government, classified   |
| User Configurable    | ✅ Yes                    | ⚠️ Limited                   | ❌ No                               |
| Scalability          | ❌ Poor                   | ✅ Excellent                  | ⚖️ Moderate                         |

---

## 🧩 How They Fit into IAM & GRC

- **GRC teams** assess whether access control aligns with **least privilege** and **segregation of duties**.
- **Auditors** look for policy enforcement and improper access assignments.
- **Security teams** choose access models based on sensitivity of data and environment.

> Example: MAC for federal contracts (compliance), RBAC for corporate apps (efficiency), DAC for personal/team sharing (flexibility).

---

> 🧠 Created by Leah to understand how access control models impact identity management, GRC, and secure system design.
