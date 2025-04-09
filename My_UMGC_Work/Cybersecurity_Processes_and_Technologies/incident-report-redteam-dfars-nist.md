# 📄 Incident Report Summary: Security Breach Investigation & Compliance Implications

> ⚠️ _This content was developed for academic purposes and adapted for public learning use in a professional portfolio. It is not intended for direct reuse or submission. Please use it as a study reference only._

> _This incident report was written as part of a Red Team assessment and reflects how the business responded to a simulated cybersecurity breach. It incorporates key compliance considerations under DFARS 252.204-7012 and NIST SP 800-171._

---

## Contact Information

- **Name:** Leah Livingston  
- **Role:** IT Manager  
- **Organizational Unit:** IT Department  
- **Email:** corp.email@example.org  
- **Phone:** 859-618-1234  
- **Location:** 1555 Pine Knob Trail, Pine Knob, KY 42721 – Room #301  

---

## Incident Timeline

| Event                  | Timestamp (EDT)         |
|------------------------|-------------------------|
| Incident started       | 2024-06-10 14:00        |
| Incident discovered    | 2024-06-11 10:00        |
| Incident reported      | 2024-06-11 10:45        |
| Incident resolved      | 2024-06-14 15:00        |

---

## Incident Summary

The incident was **discovered by the Red Team** as part of a penetration test. The attackers:

- Exploited an **unprotected network connection**
- Used **USB drops** to capture keystrokes
- Conducted **social engineering** and phishing campaigns
- Installed malware on the **PROM burner**

They successfully exfiltrated:

- **100% of AX10 Drone System design documents and source code**
- Passwords for 20% of employees
- A test vehicle

---

## Affected Resources

| Resource               | Hostname               | IP Address       | Issue                  |
|------------------------|------------------------|------------------|------------------------|
| R&D Server             | R&D-Server-01          | 10.10.135.2      | Unprotected connection |
| SCADA Workstation      | SCADA-Workstation-01   | 10.10.135.4      | Stolen credentials     |
| Corporate Workstation  | Corp-Workstation-01    | 10.10.100.6      | USB drop attack        |

---

## Incident Classification

- **Category:** Data Breach, Malware, Social Engineering  
- **Attack Vectors:** Phishing, USB drops, physical access, unprotected network  
- **Indicators:** Unauthorized logins, keylogging software, missing vehicle, malware artifacts, spike in suspicious email traffic

---

## Impact Analysis

- **Functional Impact:** Low – limited to server shutdown  
- **Information Impact:** Loss of confidentiality & integrity of sensitive IP  
- **Recoverability:**
  - **Systems:** Recoverable  
  - **Data (IP):** Not recoverable due to exfiltration

---

## Mitigating Factors

There were **no existing mitigating controls** in place at the time of the incident.

---

## Response Actions

- Shutdown of compromised server  
- Incident is under internal review  
- Contact made with:
  - Department of Defense (DoD)
  - Department of Homeland Security (DHS)
  - Relevant software vendors

---

## Root Causes

- No **awareness training** on social engineering  
- No **automated monitoring or detection tools**  
- No **network segmentation** between R&D and corporate environments  
- Outdated or unimplemented **security policies**  
- No formal **incident response plan**

---

## Cost Estimate for Recovery

| Task                          | Hours | Rate/hr | Cost     |
|-------------------------------|-------|---------|----------|
| Identification & Containment  | 40    | $100    | $4,000   |
| Forensic Analysis             | 40    | $100    | $4,000   |
| Patching & Updates            | 35    | $100    | $3,500   |
| Data Recovery & Restoration   | 30    | $100    | $3,000   |
| Security Improvements         | 40    | $100    | $4,000   |
| Policy & Procedure Revisions  | 30    | $100    | $3,000   |
| Awareness Training            | 25    | $100    | $2,500   |
| **Total Estimated Cost**      | —     | —       | **$25,000** |

---

## Business Impact

- Reputational damage  
- Financial losses due to downtime  
- Loss of customer trust  
- Theft of intellectual property  
- Compliance risks with government contracts

---

## Compliance Discussion

This incident highlights the need for compliance with:
- **DFARS 252.204-7012**: Safeguarding Covered Defense Information (CDI) and incident reporting  
- **NIST SP 800-171**: Protecting Controlled Unclassified Information (CUI) in nonfederal systems

These frameworks provide essential controls such as access restrictions, audit logging, incident response plans, and employee training. Adhering to them not only improves security posture but demonstrates responsibility and accountability to government partners.

---

## 📚 References

- U.S. Department of Defense. (n.d.). *DFARS 252.204-7012 – Safeguarding Covered Defense Information and Cyber Incident Reporting*. Retrieved April 9, 2025, from [https://www.acquisition.gov/dfars/252.204-7012](https://www.acquisition.gov/dfars/252.204-7012)

- National Institute of Standards and Technology (NIST). (2021). *Special Publication 800-171 Rev. 2: Protecting Controlled Unclassified Information in Nonfederal Systems and Organizations*. Retrieved April 9, 2025, from [https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-171r2.pdf](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-171r2.pdf)

---

> _“Compliance with DFARS and NIST 800-171 isn’t just a checkbox — it’s a blueprint for defending what matters most.”_
