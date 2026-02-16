# 🛡️ IT Support Enterprise Lab Portfolio
**Administrator:** John Belita
**Location:** Calgary, AB
**Environment:** Windows Server 2022, Windows 11, Action1 RMM, Jira Service Management

---

## 🏗️ Section 0: Infrastructure Implementation
*Building the foundational server environment and promoting the Domain Controller.*

### 0.1 Virtual Machine Configuration
> *Provisioned a Windows Server 2022 VM with optimized resource allocation (2 vCPU, 8GB RAM) to host Domain Services.*

![VM Resource Config](screenshots/vm-config-resources.png)

### 0.2 Network Configuration (Static IP)
> *Configured a static IP address (10.0.0.10) to ensure reliable DNS resolution and network stability for the Domain Controller.*

![Static IP Setup](screenshots/server-static-ip.png)

### 0.3 Server Configuration (Naming)
> *Renamed the server to 'YYC-DC-01' to align with enterprise naming conventions.*

![Server Rename](screenshots/server-rename.png)

### 0.4 Domain Controller Promotion
> *Promoted the server to a Domain Controller by installing AD DS roles and creating a new forest root domain (belita.com).*

![AD DS Promotion](screenshots/server-promotion-ad.png)

### 0.5 Verification
> *Verified successful deployment of Active Directory Users and Computers (ADUC).*

![AD Verification](screenshots/ad-deployment-verified.png)

---

## 📂 Section 1: Identity & Access Management (Active Directory)
*Demonstrating core competency in user lifecycle management, security groups, and organizational structure.*

### 1.1 Organizational Unit (OU) Design
> *Designed a hierarchical OU structure to separate 'Admin' accounts from 'Standard Users' and 'Service Accounts,' ensuring granular policy application and reduced attack surface.*

![Active Directory OU Structure](screenshots/ad-ou-structure.png)

### 1.2 New User Provisioning
> *Created standard user accounts (e.g., Bob Jones) with specific attribute details (Job Title, Department) to support dynamic groups and automated drive mapping.*

![User Properties](screenshots/ad-user-properties.png)

### 1.3 Security Group Implementation
> *Implemented Role-Based Access Control (RBAC) using Departmental Security Groups (e.g., 'HR_Drive_Access') to streamline file permission management.*

![Security Groups](screenshots/ad-security-groups.png)

---

## ⚙️ Section 2: Endpoint Management & Automation (Group Policy)
*Showcasing the ability to automate configuration and security settings across the fleet.*

### 2.1 Drive Mapping Automation
> *Configured Group Policy Preferences (GPP) to automatically map network drives (Z:) based on user Security Group membership, reducing manual mapping tickets.*

![GPO Drive Mapping](screenshots/gpo-drive-map.png)

### 2.2 Security Hardening (Account Lockout)
> *Enforced a strict Account Lockout Policy (3 attempts) to mitigate brute-force attacks on network credentials.*

![Account Lockout Policy](screenshots/gpo-lockout.png)

### 2.3 Client-Side Validation
> *Verified GPO application on a Windows 11 client using command-line tools (`gpresult /r`) to ensure compliance and troubleshoot policy conflicts.*

![GPResult Command](screenshots/cmd-gpresult.png)

---

## ☁️ Section 3: Cloud RMM & Patch Management (Action1)
*Demonstrating modern, cloud-based fleet management and vulnerability remediation.*

### 3.1 Active Directory Integration
> *Connected on-premise Active Directory to Action1 Cloud RMM, enabling real-time discovery of unmanaged endpoints and automated agent deployment.*

![Action1 Connectors](screenshots/action1-connectors.png)

### 3.2 Third-Party Software Deployment
> *Deployed critical business software (7-Zip) to remote endpoints using the 'Run Now' scheduler to meet urgent user requirements.*

![Software Deployment](screenshots/action1-deployment.png)

### 3.3 Vulnerability Assessment
> *Identified and remediated high-severity CVEs (Common Vulnerabilities and Exposures) across the test environment to maintain security compliance.*

![Vulnerability Dashboard](screenshots/action1-dashboard.png)

---

## 🎫 Section 4: IT Service Management (Jira Service Management)
*Proving the ability to manage the ticket lifecycle, SLAs, and user communication.*

### 4.1 Service Request Fulfillment
> *Triaged and resolved a software installation request, deploying the application via RMM and verifying success with the user.*

![Resolved Request Ticket](screenshots/jira-ticket-7zip.png)

### 4.2 Incident Management (Break/Fix)
> *Resolved a high-priority 'User Locked Out' incident for user Kyrie within the SLA window using Active Directory tools to restore access.*

![Resolved Incident Ticket](screenshots/jira-ticket-incident.png)

---

## 📫 Contact
**John Belita** | Calgary, AB
