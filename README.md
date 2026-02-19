# 🛡️ IT Support Enterprise Lab Portfolio
**Administrator:** John Belita
**Location:** Calgary, AB | **Email:** johnalbertbelita@gmail.com

---

## 🚀 Project Overview
Welcome to my technical portfolio. This repository serves as documented proof of my hands-on proficiency in enterprise IT support, bridging the gap between my formal Cybersecurity and Networking education and real-world Service Desk operations. 

To demonstrate my readiness for IT Support roles, I engineered a comprehensive **Enterprise Home Lab**. This simulated hybrid environment allowed me to execute the daily responsibilities of a Service Desk Analyst, from resolving end-user incidents to managing identity lifecycles and enforcing endpoint security.

### 🛠️ Tech Stack & Tools Used
* **Infrastructure:** Windows Server 2022, Windows 11 Pro, Oracle VirtualBox
* **Identity & Security:** Active Directory (AD DS), Group Policy (GPO), NTFS/RBAC
* **ITSM & Ticketing:** Jira Service Management
* **Endpoint Management:** Action1 RMM

### 🎯 Core Competencies Demonstrated
* **Identity & Access Management (IAM):** Administering Active Directory user lifecycles, configuring account restrictions, and enforcing security policies.
* **IT Service Management (ITSM):** Managing the full ticket lifecycle, practicing First Call Resolution (FCR) methodologies, and enforcing SLAs.
* **Remote Fleet Management:** Deploying third-party software, monitoring endpoint health, and managing patch compliance.
* **Security & Compliance:** Architecting secure file shares, applying the Principle of Least Privilege, and enforcing Role-Based Access Control.

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
> *Provisioned new user accounts (e.g., Neil Nepu) with standard naming conventions and configured strict Logon Hours/Account Expiry to enhance security.*

![New User Neil
