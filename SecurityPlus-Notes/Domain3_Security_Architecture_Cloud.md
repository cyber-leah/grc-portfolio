
# Domain 3: Security Architecture  
**Topic: Cloud Service Models & Responsibility Matrix**

## Cloud Service Models

### Infrastructure as a Service (IaaS)
- The cloud service provider (CSP) offers **network infrastructure** such as:
  - Desktops
  - Servers
  - Storage
  - Firewalls
  - Routers
  - Switches
- The customer is responsible for installing the operating system, patching, and configuration.

### Software as a Service (SaaS)
- The CSP hosts a **predefined software application** accessed via a web browser.
- Example: Microsoft 365, Salesforce, Goldmine.
- SaaS applications **cannot be modified**.

### Platform as a Service (PaaS)
- PaaS provides a development environment for building and deploying applications.
- Offers **tools and services** for:
  - App development
  - Deployment across platforms (iOS, Android, Windows)
- Example: Microsoft Azure App Services, MySQL.

### Security as a Service (SECaaS)
- SECaaS provides **Identity and Access Management (IAM)**.
- Users can access applications securely from anywhere.

### Anything as a Service (XaaS)
- Includes models like:
  - Network as a Service (NaaS)
  - Desktop as a Service (DaaS)
  - Backup as a Service (BaaS)
  - And many more

---

## Responsibility Matrix

In cloud environments, security responsibilities are **shared** between the customer and the service provider.

- The **cloud provider** is typically responsible for **physical security** and **infrastructure**.
- The **customer** handles **application security** and **user-level responsibilities**.

### Example: Cloud Responsibility Matrix

| Domain                         | Customer | Cloud Service Provider |
|-------------------------------|----------|-------------------------|
| Physical Security             |          | Yes                     |
| Identification & Access Mgmt  | Yes      | Yes                     |
| Security Monitoring           |          | Yes                     |
| Application Security          | Yes      |                         |
| Configuration Management      | Yes      |                         |
| Incident Response             |          |                         |
| Awareness Training            | Yes      |                         |
| Maintenance                   |          | Yes                     |

This matrix helps identify **who is responsible** for what, depending on the service model and agreement. Understanding this is key to managing cloud security effectively.

