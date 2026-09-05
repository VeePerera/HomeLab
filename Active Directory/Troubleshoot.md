### Common Problems and Troubleshooting
- Cannot Ping Domain Controller - Client and Domain were in diiferent virtual Networks  
- Desktop Policy was not applied - Group Policy was not added to the relevant group

### Real-World common Scenario 

John Doe locked out from his account after forgetting his password. As the system Admin, you were asked to unlock his account and reset his password and allow him to add a new password when he log in to the computer  

- John Doe is locked from his account after 3 unsucessful attempts (Lockout policy is set to 3 attempts)
  
<img width="1028" height="758" alt="image" src="https://github.com/user-attachments/assets/a9756e47-1439-4dc9-97d6-c7113ddbd139" />

- System Admin unlock the account and setup a new password which user can change in his first attempt to login
- Go to users & computers > Go to the OU/Group user is added > Account > Tick unlock account and change password on next logon
  
  <img width="1026" height="736" alt="image" src="https://github.com/user-attachments/assets/c5f06972-fd65-4e2b-8d0e-929756d2800d" />
  
  <img width="1036" height="768" alt="image" src="https://github.com/user-attachments/assets/b810e4ea-86f3-4997-9820-3bbaad12e0d9" />
