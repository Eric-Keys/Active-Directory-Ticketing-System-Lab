# Active-Directory-Ticketing-System-Lab
Simulated IT helpdesk project using Active Directory, Group Policy, and ServiceNow to document real world troubleshooting tickets such as password resets, account lockouts, setting changes, and folder access permissions in a Windows Server lab environment.

## Services used
- Active Directory
- ServiceNow Ticketing System
- Remote Desktop Protocol (RDP)
- DNS, DHCP

## Topology
- Windows Server 2022 (Domain Controller)
  -Configured AD, DNS, DHCP, and Group Policies
  -Hosts and manages all user accounts and permissions
- Windows 10 Client
  -Used for simulating end user issues
  -Connects via RDP and accesses shared resources through the host only network

## Process

  
