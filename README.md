# ITSupportHomelab
## Objective
A practical IT support lab built using virtualization to simulate real-world help desk and system administration tasks. Focused on Windows Server 2019 and Windows 10 environments with common Active Directory configurations, RSAT tools, and basic ticketing workflows.

## 🔧 Tools & Technologies Used
- Oracle VirtualBox
- Windows 10 ISO
- Windows Server 2019 ISO
- RSAT (Remote Server Administration Tools)
- Active Directory Users and Computers (ADUC)
- Group Policy Management
- Remote Registry / RSOP
- PDQ Deploy & PDQ Inventory
- File & Print Services
- Basic Ticketing & Task Documentation
  
## 🧠 Skills Practiced
- Active Directory Domain Services (AD DS)
- GPO Management & RSAT Tools
- Remote Administration (RDP, Registry, RSOP)
- Organizational Units & Security Group Structuring
- Print & File Sharing via GPO
- Software Deployment with PDQ Tools
- Ticketing Workflow & Issue Documentation

## 🧩 Steps & Activities

### 1. Virtual Environment Setup
- Installed and configured VirtualBox
- Created VMs for Windows Server 2019 and Windows 10
- Configured network adapters (NAT/Bridged)

### 2. Server Configuration & Domain Setup
- Renamed Server 2019 VM and assigned a static IP
- Installed Active Directory Domain Services (AD DS)
- Promoted server to Domain Controller with domain `homelab.local`

### 3. Client Configuration
- Installed Windows 10 on separate VM
- Joined client to `homelab.local` domain
- Verified domain login with domain users

### 4. RSAT & Group Policy Management
- Installed RSAT tools for remote management
- Created and linked Group Policies (GPOs) for:
  - Password policy
  - Mapped drives
  - Desktop restrictions
- Used Resultant Set of Policy (RSOP) and `gpresult` to verify GPOs

### 5. Active Directory Management
- Created and managed Organizational Units (OUs)
- Added users and computers to correct OUs
- Assigned users to security groups
- Delegated control to simulate tiered support access

### 6. Remote Tools & Administration
- Enabled Remote Desktop and Remote Registry on clients
- Used RSAT to manage clients remotely
- Troubleshot common AD login and permission issues

### 7. Software Deployment
- Installed and used PDQ Deploy and PDQ Inventory
- Pushed basic software installations to client VM
- Scanned machines to audit installed apps and status

### 8. File & Print Services
- Configured shared folders with proper NTFS permissions
- Set up shared printer on server and deployed via GPO

### 9. Basic Ticketing Practice
- Simulated user requests and created internal task logs
- Documented resolutions for issues like:
  - Password resets
  - Drive mapping failures
  - GPO not applying

