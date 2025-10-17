# Active-Directory-Ticketing-System-Lab
Simulated IT helpdesk project using Active Directory, Group Policy, and ServiceNow to document real world troubleshooting tickets such as password resets, account lockouts, setting changes, and folder access permissions in a Windows Server lab environment.
---
## Services used
- Active Directory
- ServiceNow Ticketing System
- Remote Desktop Protocol (RDP)
- DNS, DHCP
---
## Topology
### Windows Server 2022 (Domain Controller)
- Configured AD, DNS, DHCP, and Group Policies
- Hosts and manages all user accounts and permissions
### Windows 10 Client
- Used for simulating end user issues
- Connects via RDP and accesses shared resources through the host only network
---
## Process
### Windows Server
- Set up Active Directory Domain Services and promoted to Domain Controller
- Created an Organizational Unit for the IT users and users with intentional misconfigurations
- Applied Group Policies for password complexity, account lockout, and screen lock
- Simulated tickets such as password resets, access issues, and setting misconfigurations
- Documented steps and resolutions in ServiceNow
- Verified fixes before closing tickets
- PASSWORD POLICY AND ACCOUNT LOCKOUT PATH (group policy management> expand the forest> right click default domain policy and select edit> computer configuration> policies> windows settings> security settings> account policies> password policies)
- SCREEN LOCK POLICY PATH (create GPO in domain> edit> user configuration> administrative templates> control panel> personalization)
- ENFORCED POLICIES AFTER IN COMMAND PROMPT WITH (gpupdate /force)
  
### Windows Client
- Connected Windows Client to the Domain Controller (system settings> about> advanced system settings> computer name> change)
- Configured user accounts and misconfigurations, documenting issues and solutions

  
