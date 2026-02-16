# 🛡️ IT Support Enterprise Lab Portfolio
**Administrator:** John Belita
**Location:** Calgary, AB
**Environment:** Windows Server 2022, Windows 11, Action1 RMM, Jira Service Management

---

## 🏗️ Section 0: Infrastructure Implementation
*Building the foundational server environment and promoting the Domain Controller.*

### 0.1 Virtual Machine Configuration
> *Provisioned a Windows Server 2022 VM with optimized resource allocation (2 vCPU, 8GB RAM) and installed Guest Additions for improved host-to-guest integration.*

![VM Resource Config](screenshots/vm-config-resources.png)
![Guest Additions](screenshots/vm-guest-additions.png)

### 0.2 Network Configuration & Shared Storage
> *Configured a static IP (10.0.0.10) for the server and established a secure Shared Folder path to simulate a mapped network drive for file transfer.*

![Static IP Setup](screenshots/server-static-ip.png)
![Shared Folder](screenshots/vm-shared-folder.png)

### 0.3 Domain Controller Promotion
> *Promoted the server to a Domain Controller (YYC-DC-01) by installing AD DS roles and creating a new forest root domain (belita.com).*

![Server Rename](screenshots/server-rename.png)
![AD DS Promotion](screenshots/server-promotion-ad.png)

### 0.4 Verification
> *Verified successful deployment of Active Directory Users and Computers (ADUC).*

![AD Verification](screenshots/ad-deployment-verified.png)

---

## 💻 Section 1: Client Workstation Deployment
*Configuring and joining a Windows 11 endpoint to the corporate domain.*

### 1.1 OS Installation & Selection
> *Selected Windows 11 Pro to ensure domain-joining capabilities, as Windows 11 Home does not support Active Directory integration.*

![Win 11 Pro Install](screenshots/client-win11-install.png)

### 1.2 DNS Configuration
> *Configured the Windows 11 Client DNS settings to point directly to the Domain Controller (10.0.0.10), ensuring successful name resolution for the belita.com domain.*

![Client DNS](screenshots/client-dns-config.png)

### 1.3 Domain Join
> *Successfully joined the Windows 11 client to the 'belita.com' Active Directory domain using administrative credentials.*

![Domain Join](screenshots/client-domain-join.png)

---

## 📂 Section 2: Identity & Access Management (Active Directory)
*Demonstrating core competency in user lifecycle management, security groups, and organizational structure.*

### 2.1 Organizational Unit (OU) Design
> *Designed a hierarchical OU structure to separate 'Admin' accounts from 'Standard Users' and 'Service Accounts,' ensuring granular policy application.*

![Active Directory OU Structure](screenshots/ad-ou-structure.png)

### 2.2 Advanced User Provisioning
> *Provisioned new user accounts (e.g., Neil Nepu) with standard naming conventions and configured strict Logon Hours to restrict access to business hours only.*

![New User Neil](screenshots/ad-user-neil.png)
![Logon Hours](screenshots/ad-logon-hours.png)

### 2.3 End-to-End Verification
> *Verified end-to-end connectivity by logging into the client workstation using the provisioned Active Directory user account.*

![Client Login Success](screenshots/client-login-success.png)

---

## ⚙️ Section 3: Endpoint Management & Automation (Group Policy)
*Showcasing the ability to automate configuration and security settings across the fleet.*

### 3.1 Drive Mapping Automation
> *Configured Group Policy Preferences (GPP) to automatically map network drives (Z:) based on user Security Group membership.*

![GPO Drive Mapping](screenshots/gpo-drive-map.png)

### 3.2 Security Hardening (Account Lockout)
> *Enforced a strict Account Lockout Policy (3 attempts) to mitigate brute-force attacks on network credentials.*

![Account Lockout Policy](screenshots/gpo-lockout.png)

### 3.3 Client-Side Validation
> *Verified GPO application on a Windows 11 client using command-line tools (`gpresult /r`) to ensure compliance.*

![GPResult Command](screenshots/cmd-gpresult.png)

---

## ☁️ Section 4: Cloud RMM & Patch Management (Action1)
*Demonstrating modern, cloud-based fleet management and vulnerability remediation.*

### 4.1 Active Directory Integration
> *Connected on-premise Active Directory to Action1 Cloud RMM, enabling real-time discovery of unmanaged endpoints.*

![Action1 Connectors](screenshots/action1-connectors.png)

### 4.2 Third-Party Software Deployment
> *Deployed critical business software (7-Zip) to remote endpoints using the 'Run Now' scheduler.*

![Software Deployment](screenshots/action1-deployment.png)

### 4.3 Vulnerability Assessment
> *Identified and remediated high-severity CVEs (Common Vulnerabilities and Exposures) across the test environment.*

![Vulnerability Dashboard](screenshots/action1-dashboard.png)

---

## 🎫 Section 5: IT Service Management (Jira Service Management)
*Proving the ability to manage the ticket lifecycle, SLAs, and user communication.*

### 5.1 Service Request Fulfillment
> *Triaged and resolved a software installation request, deploying the application via RMM.*

![Resolved Request Ticket](screenshots/jira-ticket-7zip.png)

### 5.2 Incident Management (Break/Fix)
> *Resolved a high-priority 'User Locked Out' incident for user Kyrie within the SLA window using Active Directory tools.*

![Resolved Incident Ticket](screenshots/jira-ticket-incident.png)

---

## 📫 Contact
**John Belita** | Calgary, AB
