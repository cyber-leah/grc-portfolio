
# Supply Chain Risk Analysis – Sifers-Grayson

**Author:** Leah  
**Date:** October 15, 2024  

---

## Introduction

Sifers-Grayson relies on a network of vendors for equipment, components, and software used in their drone and robot projects. While this supply chain is critical to operations, it introduces significant risks to product quality, intellectual property, and the security of sensitive client data—especially concerning their work with the Department of Defense (DoD) and Department of Homeland Security (DHS).

This report outlines Sifers-Grayson's exposure to cyber and IT supply chain risks, provides examples of hardware and software vulnerabilities, and recommends best practices to mitigate these risks.

---

## Cyber IT & Supply Chain Risks

A vulnerability in either hardware or software from vendors can severely impact Sifers-Grayson. A ReversingLabs survey found that nearly 90% of tech professionals encountered major software supply chain risks in the past year.

### Hardware Supply Chain Risks

1. **Backdoors in Hardware Components:**  
   Preinstalled backdoors (e.g., Huawei routers) can allow undetected access. These are often diagnostic tools that become exploitable vulnerabilities.

2. **Network Infrastructure Compromise:**  
   Attackers may target components like Private 5G infrastructure to access sensitive data, which is especially concerning for Sifers-Grayson’s R&D center.

3. **Malicious Hardware Components:**  
   Nation-state attackers may insert malware at the manufacturing level. Over one-third of businesses report concern over this risk (HP Wolf Security).

### Software Supply Chain Risks

1. **Open-Source Threats:**  
   With 90% of applications using open-source code, vulnerabilities can spread easily. Sonatype reported a 430% rise in supply chain attacks in 2020.

2. **Hijacked Updates:**  
   Compromised update mechanisms (e.g., NotPetya 2017) can distribute malware to multiple organizations simultaneously.

3. **Vendor Risks:**  
   Even trusted vendors can cause disruptions, as shown by a CrowdStrike EDR update that triggered system crashes beyond their direct customer base.

---

## Best Practices for Reducing Risks

To protect itself and its clients (DoD and DHS), Sifers-Grayson should adopt the following:

- **Evaluate vendor cybersecurity posture**  
- **Continually monitor third-party suppliers**  
- **Utilize Endpoint Detection & Response (EDR) tools**  
- **Ensure secure system builds and regular updates**  
- **Have a tested incident response plan**

These practices collectively minimize the likelihood and impact of supply chain breaches.

---

## Summary and Conclusion

Supply chain risks are a significant threat to Sifers-Grayson and its clients. Hardware tampering, software vulnerabilities, and vendor-related issues could all lead to compromised systems and national security concerns.

Sifers-Grayson must:
- Rigorously evaluate vendors
- Use real-time monitoring tools like EDR
- Secure builds and patch systems promptly
- Be ready to respond effectively to incidents

These steps will enhance resilience, protect operations, and maintain the trust of high-profile clients like the DoD and DHS.

---

## References

- [CISA, 2021](https://www.cisa.gov/sites/default/files/publications/defending_against_software_supply_chain_attacks_508_1.pdf)  
- [Fortinet, n.d.](https://www.fortinet.com/resources/cyberglossary/supply-chain-attacks)  
- [GuyCarpenter, 2024](https://www.guycarp.com/insights/2024/07/global-outage-with-widespread-impact.html)  
- [Ishihara, 2021](https://www.trendmicro.com/en_us/research/21/k/private-5g-security-risks-in-manufacturing-part-4.html)  
- [Korolov, 2021](https://www.datacenterknowledge.com/supply-chain/what-are-supply-chain-attacks-and-how-to-guard-against-them)  
- [McCann, 2024](https://cybermagazine.com/articles/hp-businesses-fear-physical-supply-chains-posing-cyber-risk)  
- [Neate, 2019](https://www.theguardian.com/technology/2019/apr/30/alleged-huawei-router-backdoor-is-standard-networking-tool-says-firm)  
- [ReversingLabs, 2023](https://www.globenewswire.com/news-release/2023/04/20/2651056/0/en/Nine-Out-of-10-Companies-Detected-Significant-Software-Supply-Chain-Security-Risks-in-the-Last-12-Months-According-to-New-ReversingLabs-Report.html)  
- [Wysopal, 2024](https://www.forbes.com/councils/forbestechcouncil/2024/02/06/rising-threat-understanding-software-supply-chain-cyberattacks-and-protecting-against-them/)
