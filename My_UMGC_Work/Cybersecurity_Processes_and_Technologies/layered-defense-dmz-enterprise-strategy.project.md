# 🛡️ Final Project: Defensive Security Strategies for Strengthening Cybersecurity

> ⚠️ _This content was developed for academic purposes and adapted for public learning use in a professional portfolio. It is not intended for direct reuse or submission. Please use it as a study reference only._

> _This document outlines two proposed defensive security strategies to improve a company's cybersecurity posture: implementing a Demilitarized Zone (DMZ) and deploying enterprise-wide protective and detective measures._

---

## 📘 Introduction

As cyber threats evolve, organizations must implement strategic security measures to protect critical assets. This proposal introduces two comprehensive defensive strategies:

1. **Building a Demilitarized Zone (DMZ)** to secure remote R&D access  
2. **Implementing enterprise-wide protective and detective measures** to enhance visibility and resilience

These strategies, aligned with layered security and defense-in-depth frameworks, aim to protect the business from both internal and external threats.

---

## 🧱 Security Strategies Overview

### 🔐 Layered Security vs. Defense-in-Depth

- **Layered Security** protects multiple IT layers using a variety of tools. It minimizes risks by ensuring that if one control fails, others are in place to stop the attack (Apotheon, 2008).
- **Defense-in-Depth** incorporates technical, physical, and administrative safeguards. It uses AI, access controls, behavioral monitoring, and more to detect and prevent complex threats (Fortinet, n.d.).

Both concepts work together to enhance cybersecurity through redundancy and overlapping defenses.

---

## 🔧 Defensive Strategy #1: Building a DMZ

A **DMZ (Demilitarized Zone)** is a network segment that isolates externally accessible servers from the internal network (Newhouse et al., 2019). This strategy allows engineers to remotely access R&D resources securely without exposing the internal environment.

### ✨ Recommended Tools

| Tool                     | Purpose                                                                 |
|--------------------------|-------------------------------------------------------------------------|
| **Cisco RV340 Router**   | VPN support and automated updates                                       |
| **SonicWall TZ370W NGFW**| Deep packet inspection, real-time threat prevention                     |
| **Cisco Firepower 1120** | Intrusion detection & prevention with threat intelligence integration   |

This DMZ will shield critical assets from external threats and enforce strict access controls.

---

## 🛡️ Defensive Strategy #2: Enterprise-Wide Protective & Detective Measures

This strategy improves real-time monitoring, identity access, lifecycle management, and forensic readiness.

### ✨ Recommended Tools

| Tool                        | Purpose                                                                 |
|-----------------------------|-------------------------------------------------------------------------|
| **Inflectra SpiraTeam (ALM)** | Manages risk, software quality, and project lifecycles                 |
| **Auth0 by Okta (IAM)**     | Role-based access, fine-grained authorization, SSO integration          |
| **Splunk Enterprise Security (SIEM)** | AI-powered analytics and threat detection                    |
| **FTK Imager**              | Captures digital forensic images, preserves volatile data               |

Together, these tools establish a strong detection and response foundation to counter modern threats.

---

## ✅ Justification and Strategic Alignment

Both strategies address vulnerabilities discovered in penetration tests, particularly:

- Poor firewall placement leaving data centers exposed
- Lack of centralized visibility and control
- Use of legacy systems (e.g., Windows 10 and Windows Server 2012)

By deploying these solutions, the company mitigates risks associated with unauthorized access, internal threats, and cyberattacks — while ensuring regulatory compliance and long-term operational continuity.

---

## 🧩 Implementation Summary

### DMZ Benefits

- **Cisco RV340 Router:** Secure VPN access, automated firmware updates  
- **SonicWall TZ370W NGFW:** Deep packet inspection, threat detection, firewall rule control  
- **Cisco Firepower 1120:** Behavioral threat detection and malware containment

### Enterprise-Wide Tool Benefits

- **SpiraTeam:** Integrated project and risk management  
- **Auth0:** Identity governance with RBAC and multi-factor authentication  
- **Splunk Enterprise Security:** Real-time alerting and analytics  
- **FTK Imager:** Evidence capture for post-incident investigations

---

## 🔚 Conclusion

Together, the DMZ and enterprise-wide protective tools offer a layered, defense-in-depth solution. They will:

- Secure remote access for engineers  
- Segment and protect the network infrastructure  
- Detect and respond to threats in real time  
- Ensure forensic readiness and policy enforcement

This strategy future-proofs the organization against escalating cybersecurity risks.

---

## 📚 References

- Apotheon. (2008). *Defense in Depth and Layered Security*. Retrieved from [https://apotheon.net](https://apotheon.net)
- Auth0. (n.d.). *Secure Access for Everyone*. Retrieved from [https://auth0.com](https://auth0.com)
- Cisco. (2020). *Cisco RV340 Router Datasheet*. Retrieved from [https://www.cisco.com](https://www.cisco.com)
- Cisco. (2023). *Cisco Firepower 1120 Overview*. Retrieved from [https://www.cisco.com](https://www.cisco.com)
- Exterro. (n.d.). *FTK Imager Product Overview*. Retrieved from [https://www.exterro.com](https://www.exterro.com)
- Fortinet. (n.d.). *Defense in Depth Explained*. Retrieved from [https://www.fortinet.com](https://www.fortinet.com)
- Inflectra. (n.d.). *SpiraTeam Application Lifecycle Management*. Retrieved from [https://www.inflectra.com](https://www.inflectra.com)
- Newhouse, W., Keith, S., Scribner, B., & Witte, G. (2019). *NIST SP 800-181: NICE Cybersecurity Workforce Framework*. National Institute of Standards and Technology.
- SonicWall. (n.d.). *TZ370W Product Features*. Retrieved from [https://www.sonicwall.com](https://www.sonicwall.com)
- Splunk. (n.d.). *Splunk Enterprise Security Product Overview*. Retrieved from [https://www.splunk.com](https://www.splunk.com)

---

> _“When layered security meets smart planning, cyber resilience becomes not just a goal — but a standard.”_
