# 📘 CAP CBK Notes — Official (ISC)² Guide to the CAP CBK, 2nd Edition
**Author:** Patrick D. Howard  
**Course:** Cybersecurity in Government Organizations  
**Purpose:** Study notes and summaries from the CAP CBK

---

## 📖 Chapter 1: Security Authorization of Information Systems

- **Purpose of RMF:** Structured process for integrating security and risk management into the system development life cycle (SDLC).
- **Steps of RMF:**
  1. Categorize Information System
  2. Select Security Controls
  3. Implement Security Controls
  4. Assess Security Controls
  5. Authorize Information System
  6. Monitor Security Controls
- **Key Concepts:**
  - Information System Boundaries
  - Risk-based decision making
  - Continuous monitoring

---

## 📖 Chapter 2: Categorize the Information System

- **FIPS 199:** Determines the impact levels (Low, Moderate, High) for confidentiality, integrity, and availability.
- **Documentation:**
  - System Security Plan (SSP)
  - Information Types and Impact Levels
- **Tools:** Categorization Worksheet, Data Flow Diagrams (DFDs)

---

## 📖 Chapter 3: Select Security Controls

### **Minimum Security Baselines and Best Practices**

- **Definition:** A **minimum security baseline (MSB)** is a set of standardized, essential controls that must be implemented across all systems to ensure a consistent level of compliance and protection.
- **Purpose:**
  - Establishes a reference point for assessing the organization's security posture.
  - Ensures every system meets at least a basic level of security.
  - Serves as a starting point for risk assessments and tailoring security controls.
- **Benefits:**
  - Enhances control requirements.
  - Eliminates non-applicable controls.
  - Supports compliance by enforcing consistent configurations across IT platforms and devices.
- **Key Takeaway:** "All of our systems will implement this basic set of security controls."

---

### **Security Controls**

- **FIPS 199 Definition:** Security controls are the management, operational, and technical safeguards or countermeasures used to protect the confidentiality, integrity, and availability of information systems.
- **Challenges:**
  - Implementing controls may be costly or technically infeasible for some systems.
  - Organizations can manage this by examining systems and applying MSBs aligned to risk needs.
- **Decomposition Strategy:**
  - Large systems can be broken down into manageable components for easier authorization and cost-effective control application.

### **Levels of Controls**

- Controls must be adjusted based on:
  - System type (e.g., general support vs. major application)
  - System sensitivity (e.g., low, moderate, high)
- **Technology-specific control sets** should supplement the MSB to meet baseline requirements for:
  - OS, databases, web servers, routers, etc.

#### Sensitivity Levels:
- **Low Sensitivity:** Implements automatic updates for malicious code protection.
- **Moderate Sensitivity:** Adds centralized management of protection mechanisms.
- **High Sensitivity:** Includes all prior plus full automation of virus protection updates.

### **Risk Assessment in System Authorization**

- **Purpose:** Tailors controls to system-specific risks. Ties asset identification to environment definition and maps vulnerabilities to MSBs.
- **Integration:** Must align with the overall system authorization process.

---

### **Risk Assessment Process — 9 Steps**

1. **System Characterization:** Define system type, boundaries, purpose, assets, users, and environment.
2. **Threat Identification:** Document potential threats (environmental, human, internal, external, intentional, unintentional).
3. **Vulnerability Identification:** Identify weaknesses that may be exploited; compare against MSBs and known vulnerabilities.
4. **Control Analysis:** Analyze existing and planned controls (technical, management, and operational) to determine what mitigates threats.
5. **Likelihood Determination:** Assess the probability of threat/vulnerability pairs using qualitative or quantitative ratings.
6. **Impact Analysis:** Determine the impact of exploitation based on system sensitivity and mission criticality.
7. **Risk Determination:** Combine likelihood and impact to assign risk ratings; identify most significant risks.
8. **Control Recommendations:** Suggest additional or alternative controls based on cost-effectiveness and risk reduction.
9. **Results Documentation:** Report threats, vulnerabilities, risk levels, and recommendations. Append findings to SSP.

- **Conducting the Risk Assessment** The minimum information for the risk assessment relates to:
1. **Assets** 
2. **Threats** 
3. **Vulnerability Identification:** 
---

> ✏️ *More chapters and details will be added.*

