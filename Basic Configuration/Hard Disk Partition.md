# Hard Disk Partition

## Partition during OS installation (Recommended)
The recommended way to partition an extra drive is when installing the OS. 
- Select New > Add the size of the partition. 

<img width="826" height="572" alt="image" src="https://github.com/user-attachments/assets/7a5ec9c5-b5cf-4ad8-9ee0-90b55350a31b" />

- Following images show how the drive is partitioned logically and how to make it visible once the OS is installed. 

<img width="762" height="560" alt="image" src="https://github.com/user-attachments/assets/83cda174-b120-4cc6-9815-3ff93325c82c" />

- Once the OS installation is complete. Go to This PC > Right-click and select Manage
- Select Computer Management > Disk Management
- Right-click on the Unallocated space and select New Simple Volume
<img width="1134" height="756" alt="image" src="https://github.com/user-attachments/assets/a25b607b-1975-47a9-b659-beb2df8d86f8" />

<img width="1268" height="754" alt="image" src="https://github.com/user-attachments/assets/20a5ff34-f810-4e61-a030-9c96998c0e05" />

<img width="1090" height="738" alt="image" src="https://github.com/user-attachments/assets/be52640d-5fdd-4253-8f63-5619bfa3899e" />


## Partition after the OS installation (Not recommended)

- Select the primary partition > Manage > Disk Manager

<img width="1096" height="756" alt="image" src="https://github.com/user-attachments/assets/585efda2-ee55-49f4-9bc0-352e8adfed51" />

<img width="1108" height="738" alt="image" src="https://github.com/user-attachments/assets/50713bb9-4f7a-4023-bbe3-6eec63c41837" />

## Real-World Scenario 
- C drive is damaged or crashed, therefore, you need to repair it by re-installing the OS. 
_For the demonstration purpose, C drive is deleted using VMs > Power on to firmware > Boot up using CDROM Drive_

<img width="1034" height="746" alt="image" src="https://github.com/user-attachments/assets/9115f738-bcf6-4402-97bc-a5060e1f374a" />

- Power off the VM > Choose to Boot up via CDROM Drive > Select the unallocated space previously assigned for C or the primary drive > Proceed

<img width="806" height="564" alt="image" src="https://github.com/user-attachments/assets/7fd0b8a1-cffd-4723-9240-efe16666a437" />



