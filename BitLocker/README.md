# BitLocker Home Lab 
## Overview
Deploy, manage, recover, and troubleshoot BitLocker on Windows devices in an Active Directory environment. 

## What is BitLocker
A full disk encryption feature built into Microsoft Windows to protect data by encrypting entire drives. Prevent unauthorized access to sensitive information if a computer is lost, stolen, or accessed by someone without permission.  

BitLocker encrypts the entire operating system drive, ensuring that Windows files, applications, user data, and temporary files are all protected.  

In enterprise environments, BitLocker is commonly managed through Active Directory, Microsoft Entra ID, Microsoft Intune, or Microsoft Configuration Manager, allowing IT administrators to centrally enforce encryption policies and securely store recovery keys.

## When to Use BitLocker

### BitLocker is recommended when:

- Protecting company laptops from theft or loss.
- Encrypting operating system drives and fixed data drives.
- Meeting organizational security policies and compliance requirements.
- Managing encryption centrally through Active Directory or Microsoft Intune.

## BitLocker Deployment in an Active Directory Environment
### Lab Goal
Deploy BitLocker to a domain-joined Windows 10 client, configure Group Policy to back up recovery keys to Active Directory, and verify the recovery key can be retrieved by IT Support.

### Lab Environment
- Windows 19 Server
- Windows 10 client

### Step 1 - Check pre-requisites 
Verify that the Windows 10 client has a functional Trusted Platform Module before deploying BitLocker. TPM provides hardware-backed protection for cryptographic keys and help verify the integrity of the startup environment.

_The Windows 10 client was running in VirtualBox without a virtual TPM. BitLocker was therefore configured to operate without a compatible TPM for lab purposes._

### Step 2 - Create Group Policy & Allow Bit Locker without TPM

Create a new group policy under your computers > Computer Configurations > Administrative templates > Windows Components > Bit locker Drive Encryption> Require addition authentication at startup

<img width="1256" height="1172" alt="image" src="https://github.com/user-attachments/assets/b4c56509-c10c-449b-9c05-a526d445c6e1" />

### Step 3 - Configure recovery information

<img width="1180" height="1104" alt="image" src="https://github.com/user-attachments/assets/47ad9a50-79a7-44eb-884a-8d492a4ebf11" />

### Step 4 - Apply GPO and confirm GPO applied

<img width="998" height="254" alt="image" src="https://github.com/user-attachments/assets/138340f3-808d-4985-86ad-6c4eb1d99195" />

### Step 5 - Setup BitLocker in Client
- In Windows client turn on the Bit Locker
- Choose how to unlock Bit Locker
<img width="1020" height="768" alt="image" src="https://github.com/user-attachments/assets/309b9ab5-f5a7-482f-b13f-4e9d03b218e1" />






