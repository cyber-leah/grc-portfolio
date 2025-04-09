# 🔄 NIST SP 800-37 Revision 2 Study Guide  
**Title:** *Guide for Applying the Risk Management Framework to Federal Information Systems*  
**Full PDF:** [SP 800-37 Rev. 2](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-37r2.pdf)

---

## 🎯 What is SP 800-37?

SP 800-37 provides guidance for implementing the **Risk Management Framework (RMF)** — a structured, repeatable process for integrating **security**, **privacy**, and **cyber supply chain risk management** into the **system development life cycle (SDLC)**.

It supports compliance with **FISMA** and aligns with the **NIST Cybersecurity Framework (CSF)**.

---

## 🧱 Core Goals of RMF

- **Incorporate security and privacy from the start** (i.e., early in system design)
- Enable **continuous monitoring and risk-based decision-making**
- Promote **organizational accountability** for system and data protection

---

## 📈 The 7 Steps of the Risk Management Framework

| Step # | Name                    | Description |
|--------|-------------------------|-------------|
| 1️⃣     | **Prepare**               | Establish context and priorities before system development or control selection. Includes roles, risk tolerance, and resource allocation. |
| 2️⃣     | **Categorize**            | Define system impact levels for confidentiality, integrity, and availability (uses FIPS 199 and SP 800-60). |
| 3️⃣     | **Select**                | Choose baseline controls based on categorization (from SP 800-53), and tailor them as needed. |
| 4️⃣     | **Implement**             | Put selected controls into action and document how they were deployed. |
| 5️⃣     | **Assess**                | Determine if controls are implemented correctly and producing intended outcomes (security assessment). |
| 6️⃣     | **Authorize**             | Senior officials decide if system risk is acceptable and formally grant Authorization to Operate (ATO). |
| 7️⃣     | **Monitor**               | Continuously monitor control effectiveness, environment changes, and system operations. Update documents as needed. |

---

## 🔄 Continuous Monitoring Loop

After authorization, steps 4–7 are repeated continuously to maintain security over the system's life cycle.

---

## 🔧 Key Roles in RMF

| Role                    | Responsibility |
|-------------------------|----------------|
| **Authorizing Official (AO)** | Accepts risk and grants ATO |
| **System Owner**              | Accountable for system security posture |
| **Control Assessor (SCA)**    | Conducts control assessments |
| **Information System Security Officer (ISSO)** | Helps implement and monitor controls |

---

## 🔐 Integration with Privacy

SP 800-37 Rev. 2 explicitly includes **privacy risk management** alongside security, ensuring protections for:

- **Personally Identifiable Information (PII)**
- **Individual rights**
- **Transparency and data minimization**

---

## 🔁 Alignment with Other Frameworks

| Framework          | Purpose |
|--------------------|---------|
| **FIPS 199**       | Determines impact levels |
| **SP 800-60**      | Maps info types to impact levels |
| **SP 800-53**      | Provides the control catalog |
| **SP 800-53B**     | Offers control baselines for selection |
| **SP 800-39**      | Organization-wide risk management strategy |
| **Cybersecurity Framework (CSF)** | Strategic risk management using functions: Identify, Protect, Detect, Respond, Recover |

---

## 📋 Required Documentation

| Document                     | Purpose |
|------------------------------|---------|
| **System Security Plan (SSP)**     | Describes the system and selected controls |
| **Security Assessment Report (SAR)** | Results from control testing |
| **Plan of Action and Milestones (POA&M)** | Plans to correct deficiencies |
| **Authorization Package**          | Bundle of SSP + SAR + POA&M used for ATO decision |

---

## 🧠 Tips to Remember

- RMF is **cyclical**, not linear — always monitor and update
- **Prepare** step is new in Rev. 2 and focuses on org-level readiness
- **Authorization** is about **risk acceptance**, not risk elimination
- RMF helps enforce **accountability and transparency**

---

## 🔗 Related NIST Documents

- [FIPS 199](https://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.199.pdf)
- [SP 800-60](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-60v1r1.pdf)
- [SP 800-53 Rev. 5](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r5.pdf)
- [SP 800-53B](https://csrc.nist.gov/publications/detail/sp/800-53b/final)
- [SP 800-39](https://csrc.nist.gov/publications/detail/sp/800-39/final): Enterprise risk strategy

---

## 🏷 Tags  
`#NIST80037` `#RMF` `#RiskManagement` `#SystemAuthorization` `#ATO` `#GRC` `#FISMA` `#CybersecurityLifecycle`

---

> _“Security is not a one-time authorization — it’s a living process.”_

