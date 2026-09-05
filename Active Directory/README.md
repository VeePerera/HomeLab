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
#### Objective

Install the AD DS role and promote the server to a Domain Controller.

#### Tasks Completed
Configured static IP address
Installed AD DS role
Created a new forest
Configured domain - VS.local
Verified DNS installation

#### Outcome

Successfully deployed a Domain Controller and established the Active Directory environment.

<img width="2406" height="1020" alt="image" src="https://github.com/user-attachments/assets/059e8930-d58a-4193-899d-3f1a919325df" />

### Organizational Unit (OU) Structure
#### Objective

To simulate a real business environment, Organizational Units were created for users, computers, servers and different departments. Each OU is assigned with Groups to assign user rights and permissions.

OU - USER, COMPUTER (Main OU)  
OU - TELCO, FINTECh (Sub OU)  
GROUPS - Fintech_Users: Security group to assign user rights and permissions  
GROUPS - Fintech_DL_Managers : Distribution group to send emails to Fintech managers  

### Group Policy Object 
Collection of policies in AD that can be applied to domains and users.

#### Objective
Configure basic GPO required for organizations. These policies can be applied to an OU or group of objects. Demonstrated below a

#### Password Policy
Enforce password policy for the computers, laptops getting assigned to the Domain. This is configured with Computer configuration > Policies. Policies enable rules that cannot be modified by individual users. 

<img width="1756" height="992" alt="image" src="https://github.com/user-attachments/assets/fd93c999-ee22-4949-b1bb-c957fa13a5fb" />

#### Driver Mapping Policy
Map Network Drivers for users when they sign-in to the account. This is configured with User configuration > Preferences. Preferences can be modified later by individual users. 

<img width="1814" height="994" alt="image" src="https://github.com/user-attachments/assets/cda49472-a98a-4708-b2aa-5475699a07df" />

#### Desktop Wallpaper Policy
Add a default wallpaper to all users. This is configured with User configuration > Policies. 

<img width="2442" height="1194" alt="image" src="https://github.com/user-attachments/assets/10373ba5-2fe6-41e6-a212-c21f77c2d1f3" />

#### USB Restriction Policy
Prevent users from usign USB Storage devices. This is configured with Computer configuration > Policies. 

<img width="2156" height="982" alt="image" src="https://github.com/user-attachments/assets/f76af537-acaf-4d64-a6a7-1b8f06b45bb0" />

#### Account Lockout Policy
Configure account lockout policy to prevent brute force attacks. This is configured with Computer configuration > Policies. 

<img width="1922" height="980" alt="image" src="https://github.com/user-attachments/assets/208f0efb-a1e1-4938-9d01-5af15f6c5413" />


### Domain-Join 
### Objective 
Join a client computer to the Domain. Test the implemented GPO to control users and computer settings. 

**Pre-requisites**
- Windows server installed
- Active Directory tools installed
- GPOs created
- Domain Controller IP needs to be set to static IP - To ensure consistent and reliable DNS resolution and connectivity
- Client VM installed

### Join Client to the Domain Controller

#### Configure Domain
- Through Change adpater settings > Internet Protocol Version 4 (TCP/IPv4) > Properties  
- Set the Preferred DNS setting to Domain Controller's IP

#### Change the computer Name/Domain
- Select This PC > Properties > Advanced Settings > Computer Name > Select Domain > Enter Domain Name  
- Provide Adminstrator credentials to confirm the action
- Restart 

<img width="872" height="626" alt="image" src="https://github.com/user-attachments/assets/cf6c65d6-ac0f-4232-8054-bf4d418b8f11" />

#### Verify computer in AD
- Go to the Server and under computers, verify the domainjoined client computer is visible    
- Move this to the correct OU

<img width="628" height="412" alt="image" src="https://github.com/user-attachments/assets/4cea7b2b-c11a-4272-bc8d-dc574c5564e4" />



































