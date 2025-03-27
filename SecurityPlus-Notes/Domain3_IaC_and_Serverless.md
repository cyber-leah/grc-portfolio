
# Domain 3: Security Architecture  
**Topic: Infrastructure as Code (IaC) & Serverless Computing**

## Infrastructure as Code (IaC)

**Definition**:  
Infrastructure as Code (IaC) is the practice of defining and managing IT infrastructure through **machine-readable code or scripts**, using languages like **YAML** and **JSON**.

Instead of manually configuring infrastructure, IaC allows components (servers, networks, storage, etc.) to be **defined in code**, enabling:
- **Automation**
- **Scalability**
- **Repeatability**

### Key Benefits of IaC:
- **Efficiency Redefined**: Infrastructure provisioning that once took weeks/days can now be done in seconds.
- **Consistency and Reproducibility**: Ensures infrastructure remains consistent across environments and reduces configuration errors.
- **Version Control and Collaboration**: IaC supports versioning and team collaboration—like application code.
- **Providers and Tools**: Cloud providers like AWS, Azure, and Google Cloud support IaC. Tools like Terraform, Ansible, Puppet, and Chef enable organizations to build repeatable, secure infrastructure setups.

---

## Serverless Computing

**Definition**:  
Serverless computing offloads operational overhead to the cloud service provider (CSP), allowing developers to focus only on **writing and deploying code**.

### Characteristics:
- No need to provision or manage servers
- Cloud provider automatically handles:
  - Scaling
  - Resource provisioning
  - Server management

### Security Considerations:
- The **CSP manages the infrastructure**, enhancing security.
- Serverless environments often use **Backend as a Service (BaaS)**, where backend functions like databases, authentication, and file storage are handled by the provider.

### Customer Responsibilities:
- Customers are still responsible for:
  - **Managing applications**
  - **Securing data stored in the cloud**

This model offers a **cost-effective and scalable** way to deploy services without the complexity of managing infrastructure.

