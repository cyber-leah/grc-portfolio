
# Zero Trust  
**Security+ Domain 1: Threats, Attacks, and Vulnerabilities**

## What is Zero Trust?

Zero Trust is a cybersecurity model based on the principle of "never trust, always verify." It eliminates implicit trust by continuously validating users and devices trying to access resources, regardless of their location.

Zero Trust challenges two traditional assumptions:
- That data and control planes can be tightly coupled.
- That internal network zones are automatically trustworthy.

---

## Core Concepts

### Control Plane
The control plane dictates **who can access what** on a network. It uses:
- **Policy Engine**: Evaluates access requests using policies, threat intelligence, and user/device data.
- **Policy Administrator**: Issues tokens or credentials for access.
- **Policy Enforcement Point**: Enforces decisions made by the administrator and engine.

By centralizing control and separating duties, the control plane minimizes risk and improves threat response.

### Data Plane
The data plane handles **actual movement of data** (e.g., routing, switching, packet forwarding). It:
- Executes based on predefined rules from the control plane.
- Ensures secure, efficient data transmission between devices.
- Plays a critical role in performance and secure communications.

---

## Supporting Features

### Adaptive Identity
Dynamically adjusts user privileges based on contextual factors like behavior, location, and device attributes. Enhances user experience while maintaining security.

### Threat Scope Reduction
Reduces the attack surface by:
- Minimizing exposed services
- Limiting code base
- Applying rigorous patching

This proactive defense approach lowers the risk of exploitation.

### Policy-Driven Access Control
Turns security policies into enforceable access decisions. Automates consistency, reduces human error, and allows tailored access for roles and functions.

---

## Trust Zones

Trust zones categorize network areas by risk and trustworthiness:

- **Implicit Trust Zone**: Components are assumed secure without verification.
- **Internal Network Zone**: Trusted area behind the firewall (e.g., LAN, domain controller).
- **DMZ (Demilitarized Zone)**: Semi-trusted area allowing controlled access between external/internal systems.
- **External Network Zone**: Untrusted (e.g., Internet) and requires strict access controls.

---

## Visual Model (Described)
A flowchart shows:
- **Subjects** send access requests to the **Policy Engine**.
- The engine consults identity data and policies to make decisions.
- The **Policy Administrator** issues access tokens and informs the **Policy Enforcement Point**.
- If approved, access is granted to the **Data Plane** for secure transmission.

This model separates decision-making from data movement to reduce risk and enforce Zero Trust principles.

---

Zero Trust is a fundamental shift in cybersecurity—perfect for GRC professionals focused on access control, policy enforcement, and minimizing attack surfaces.
