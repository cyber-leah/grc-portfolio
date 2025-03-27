
# Hardening Techniques  
**Domain 2: Threats, Attacks, and Vulnerabilities**

---

## Hardening Techniques

Hardening is the process of reducing system vulnerabilities and strengthening security.

### Common Hardening Methods
- **Encryption**: Converts plaintext into ciphertext to ensure data remains unreadable without the decryption key.
- **Endpoint Protection**: Includes solutions like antivirus, EDR, HIPS, and host-based firewalls.

---

## Endpoint Detection and Response (EDR)

EDR is a real-time cybersecurity solution using AI/ML for detecting and mitigating threats on endpoints.

### EDR Capabilities:
- **Continuous Monitoring**: Tracks activity, behavior, and processes
- **Behavioral Analysis**: Detects deviations from normal behavior
- **Threat Detection**: Uses threat intel, databases, and IOCs
- **Alert Generation**: Sends alerts for investigation
- **Response and Remediation**: Enables fast reaction to threats
- **Forensic Analysis**: Investigates breaches and attack vectors
- **Real-Time Threat Mitigation**: Stops threats before spreading
- **Improved Incident Response**: Streamlines containment
- **Endpoint Visibility**: Offers insight into posture and vulnerabilities

---

## Host-Based Protection

- **HIPS (Host-Based Intrusion Prevention System)**: Monitors individual hosts for unauthorized activity.
- **Host-Based Firewalls**: Control inbound/outbound traffic at the device level.  
  > Example: Helps protect laptops for remote workers.

---

## Disabling Unused Ports and Protocols

Minimizes attack surfaces by blocking commonly exploited paths:

| Protocol and Port             | Restriction                    |
|------------------------------|--------------------------------|
| Telnet port 23               | Remote access (insecure)       |
| Secure Shell (SSH) port 22   | Secure remote access           |
| NETBIOS ports 137–139        | Legacy file/print services     |
| Server message block port 445| Modern file/print services     |

> Administrators should avoid using Telnet and secure default settings.

---

## Additional Practices

- **Default Password Changes**: Prevent unauthorized access from well-known or reused credentials.
- **Removal of Unnecessary Software**: Reduces vulnerabilities by eliminating unneeded attack vectors.

These hardening practices strengthen system defenses, reduce risks, and enhance overall enterprise resilience.
