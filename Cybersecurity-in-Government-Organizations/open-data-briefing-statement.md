
# Open Data Briefing Statement

**Author:** Leah  
**Course:** Cybersecurity in Government Organizations  
**Type:** Briefing Statement  
**Event:** Cyber Scholars Day  
**Date:** March 2025  

---

## Introduction

Good afternoon and thank you for attending Cyber Scholars Day.

Today’s briefing is intended to raise awareness about the security issues arising from open data initiatives at the federal and state levels. These initiatives promote transparency by making government data freely available for public access, use, and redistribution. While the benefits of such openness are significant, notable risks must be identified and addressed to ensure responsible and secure data sharing.

---

## What is Open Data?

Open data is publicly accessible and may be reused or shared by anyone, usually with minimal requirements such as attribution or similar licensing (Open Knowledge Foundation, n.d.).

The Open Definition emphasizes that data must be fully accessible, downloadable in modifiable formats, and freely reusable without restriction. This openness supports interoperability and the combination of datasets from different sources, key for building better tools, services, and data-driven decisions (Open Knowledge Foundation, n.d.).

---

## Open Data and Related Security Issues

Three categories of open data with associated security risks include:

### 1. Critical Infrastructure Data

CISA defines critical infrastructure as sectors like energy, water and wastewater, transportation, and emergency services, systems vital to national security and public health (CISA, n.d.-a).

Open datasets often include geospatial info (maps, coordinates) about physical assets like power plants and water treatment facilities. While useful for public planning, this data could be exploited by threat actors to plan cyberattacks or physical sabotage.

### 2. Cyber Incident Data

The Trojan Detection Software Challenge dataset on data.gov includes labeled malware samples for educational purposes (NIST, 2025-a). Though valuable for innovation, detailed threat data can be misused or reverse-engineered by attackers.

CISA warns that premature release of detailed incident data—before affected systems are secured—can create an exploit window for cybercriminals (CISA, n.d.-b).

### 3. Federal Financial Data

Datasets like those on USAspending.gov include award and subaward data, detailing recipients, locations, and project timelines (BFS, 2023). While this promotes accountability, such information may help attackers impersonate contractors, identify technologies in use, or exploit gaps in procurement processes.

---

## Recommended Safeguards

To promote transparency **without compromising security**, federal and state agencies should:

1. **Conduct Data Sensitivity Assessments**  
   - Use CIA triad (confidentiality, integrity, availability) criteria early in the system development life cycle (Howard, 2016).

2. **Apply NIST Risk Management Framework (RMF)**  
   - Assess threats, apply controls, and monitor risks before releasing public datasets (NIST, n.d.-b).

3. **Follow OMB Circular A-137 Guidance**  
   - Reduce disclosure risks using anonymization, aggregation, and suppression techniques (OMB, 2024).

These practices help balance public access with responsible data stewardship.

---

## Conclusion

While open data is vital for government transparency and civic engagement, it also introduces risks that must be proactively managed. Agencies should implement structured safeguards like data sensitivity assessments, risk-based decision-making, and protective techniques such as anonymization.

In today’s evolving cyber threat landscape, **transparency must not come at the cost of national or operational security**.

---

## References

- BFS. (2023). *USAspending.gov Award & Subaward Data*. https://catalog.data.gov/dataset/usaspending-gov-federal-award-subaward-and-account-data  
- CISA. (n.d.-a). *Critical Infrastructure Sectors*. https://www.cisa.gov/topics/critical-infrastructure-security-and-resilience/critical-infrastructure-sectors  
- CISA. (n.d.-b). *Cyber Threats and Advisories*. https://www.cisa.gov/topics/cyber-threats-and-advisories  
- Howard, P. D. (2016). *Official (ISC)² Guide to the CAP CBK® (2nd ed.)*. Sybex.  
- NIST. (2025-a). *Trojan Detection Software Challenge*. https://catalog.data.gov/dataset/trojan-detection-software-challenge-cyber-pdf-dec2022-train  
- NIST. (n.d.-b). *Risk Management Framework (RMF)*. https://csrc.nist.gov/projects/risk-management  
- OMB. (2024). *Circular A-137: Strategic Management of Acquisition Data*. https://www.whitehouse.gov/wp-content/uploads/2024/05/FACT-SHEET-OMB-Circular-A-137-Strategic-Management-of-Acquisition-Data-and-Information.pdf  
- Open Knowledge Foundation. (n.d.). *What is Open Data?* https://opendatahandbook.org/guide/en/what-is-open-data/
