# Active Directory Home Lab
## Overview

This project was created to develop hands-on experience with Active Directory administration and Windows Server technologies commonly used in IT Support, Help Desk, and Junior Systems Administration roles.

The lab simulates a small business environment where users, groups, computers, policies, and shared resources are managed through Active Directory.

## Lab Environment
### Hypervisor
- Oracle Virtualbox

### Servers
- Windows 19 Server

### Clients 
- Windows 10
- Windows 11

### Domain
- VS.local

### Services Implmented 
- Active Directory Domain Services (AD DS)
- DNS
- DHCP
- Group Policy
- File Sharing
- User and Group Management

## Active Directory Configuration
### Installing Active Directory Domain Services
### Objective

Install the AD DS role and promote the server to a Domain Controller.

### Tasks Completed
Configured static IP address
Installed AD DS role
Created a new forest
Configured domain - VS.local
Verified DNS installation

### Outcome

Successfully deployed a Domain Controller and established the Active Directory environment.

<img width="2406" height="1020" alt="image" src="https://github.com/user-attachments/assets/059e8930-d58a-4193-899d-3f1a919325df" />

### Organizational Unit (OU) Structure
### Objective

To simulate a real business environment, Organizational Units were created for users, computers, servers and different departments. Each OU is assigned with Groups to assign user rights and permissions.

OU - USER, COMPUTER (Main OU)  
OU - TELCO, FINTECh (Sub OU)  
GROUPS - Fintech_Users: Security group to assign user rights and permissions  
GROUPS - Fintech_DL_Managers : Distribution group to send emails to Fintech managers  




