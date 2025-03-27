
# Access Control  
**Security+ Domain 1: Threats, Attacks, and Vulnerabilities**

## What is Access Control?

Access control refers to the process of allowing or restricting access to an organization’s data, applications, network, or cloud resources based on established policies.  
Two key components used in access control are:

- **Access Control Lists (ACLs)**
- **Permissions**

---

## Access Control Lists (ACLs)

ACLs are lists used by routers and firewalls to grant or deny access based on rules.  
There are two main types:
- **ACLs for files and folders**
- **ACLs for incoming network traffic**

### File/Data Access ACLs
These control what type of data a user can access and what level (read, write, etc.).  
Example:  
- A sales manager may get **read-only access** to a spreadsheet.  
- A sales administrator may get **read/write access** to update data.

### Network ACLs
- Implemented on routers or firewalls.
- Typically start with a default **“deny all”** rule.
- Admins must create **“allow” rules** to permit specific types of access.

---

## Principle of Least Privilege

Users are granted only the permissions necessary to do their job—no more, no less.  
This minimizes the risk of accidental or intentional misuse of sensitive data.

---

## Permissions

Permissions determine **what actions a user can perform**, such as:
- Read
- Write
- Execute
- Delete

Permissions are **role-based** and tied to job functions, helping protect data integrity and prevent unauthorized access or data tampering.

---

# Application Allow List

An **Application Allow List** (also known as a whitelist) is a mitigation strategy that only permits approved applications to run on a system.  

### Purpose:
- Prevent unauthorized or malicious applications (e.g., malware) from executing.
- Protect against ransomware and user error.

### Example:
If a user frequently installs unsafe apps, an allow list will block any software **not explicitly approved**, reducing risk and exposure.

---

Access control, ACLs, and allow lists are foundational concepts for protecting data and systems in any enterprise environment.
