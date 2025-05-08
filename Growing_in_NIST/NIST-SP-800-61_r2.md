# 🚨 NIST SP 800-61 Revision 2 Study Guide  
**Title:** *Computer Security Incident Handling Guide*  
**Publisher:** National Institute of Standards and Technology (NIST)  
**PDF:** [NIST SP 800-61r2](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-61r2.pdf)

---

## 🎯 Purpose

SP 800-61 provides practical guidance on establishing and maintaining **effective incident response (IR) capabilities**. It outlines best practices for identifying, handling, and learning from security incidents across diverse organizational environments.

---

## 🧩 Where It Fits in the NIST Ecosystem

| Related Document       | Connection |
|------------------------|------------|
| **SP 800-53 (IR family)** | This guide supports implementation of IR controls like IR-1 to IR-9 |
| **SP 800-37 (RMF)**     | Ties into the “Monitor” and “Respond” phases |
| **FIPS 199**            | Helps identify system impact when a security incident occurs |
| **SP 800-122 / PII docs** | Relevant when handling breaches of personal or sensitive data |

---

## 🧱 Incident Response Lifecycle (4 Phases)

| Phase                  | Description |
|------------------------|-------------|
| **1. Preparation**     | Develop IR policies, train teams, acquire tools, and create communication plans |
| **2. Detection & Analysis** | Monitor systems, detect events, determine if they qualify as incidents, and analyze scope |
| **3. Containment, Eradication, and Recovery** | Stop the attack, remove the threat, and restore systems to normal operations |
| **4. Post-Incident Activity** | Conduct lessons learned meetings, update playbooks, and improve defenses |

---

## 🧰 Key Practices and Takeaways

- **Preparation is critical.** Build an incident response team (IRT) with clear roles and responsibilities.
- **Triage quickly.** Use criteria to evaluate incident severity, scope, and urgency.
- **Document everything.** Logs, timelines, and decisions should be recorded for analysis and reporting.
- **Coordinate with legal & PR.** Especially in breaches involving customer or sensitive data.
- **Improve over time.** Learn from incidents and adapt policies, training, and tooling.

---

## 🔧 Tools & Techniques for IR

| Tool/Technique       | Purpose |
|----------------------|---------|
| IDS/IPS              | Detect suspicious traffic |
| SIEM                 | Correlate logs and alert on patterns |
| Ticketing systems    | Track and manage incident cases |
| Forensic tools       | Analyze infected systems and determine cause |

---

## 💡 Incident Categories (Examples)

- Malware infections  
- Unauthorized access  
- Data exfiltration or theft  
- Denial of Service (DoS) attacks  
- Insider misuse

---

## 🧠 Tips to Remember

- Not all security events are incidents — **analyze before escalating**  
- Clear communication channels are crucial — **internally and externally**  
- Your IR plan is only as strong as your **team’s training and readiness**
- Document the **who, what, when, where, and how** of every incident

---

## 🔗 Related Resources

- [SP 800-53 Rev. 5](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-53r5.pdf) – See IR family of controls  
- [SP 800-37 Rev. 2](https://nvlpubs.nist.gov/nistpubs/SpecialPublications/NIST.SP.800-37r2.pdf) – Incident handling in the RMF  
- [SP 800-122](https://nvlpubs.nist.gov/nistpubs/Legacy/SP/nistspecialpublication800-122.pdf) – Guidance for breaches involving PII

---

## 🏷 Tags  
`#IncidentResponse` `#NIST80061` `#RMF` `#SecurityIncidents` `#IRLifecycle` `#Cybersecurity`

> _“The effectiveness of incident response depends more on preparation than reaction.”_
