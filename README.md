# Active-Directory-
I set up an Active Directory system on a VM to demonstrate setting up a domain, creating and managing users all in a simulated network.

# TECH USED
    - Microsoft azure  
    - Remote desktop
    - Active Directory Domain Services

# OPERATING SYSTEMS USED
    - Windows 10 
    - Windows server 2022


STEPS
  1.  The first thing I did was create a Virtual Machine running Windows server 2022<img width="1512" height="982" alt="Screenshot 2026-05-29 at 2 38 33 PM" src="https://github.com/user-attachments/assets/4938268e-4695-46cc-bd1b-66f9ebe0802b" />
  2. On the server manager,I installed the windows active directory domain services<img width="1512" height="982" alt="Screenshot 2026-05-29 at 2 57 16 PM" src="https://github.com/user-attachments/assets/3c47d7b2-973c-4d01-a8cf-9c82612daa38" />
<img width="1512" height="982" alt="Screenshot 2026-05-29 at 2 56 14 PM" src="https://github.com/user-attachments/assets/1908c701-2e4b-4f91-88df-95f3458c485f" />
  3. Next I turned the server into the Domain controller by creating a new forest with the Active Directory Domain Service and restarted my machine<img width="1512" height="982" alt="Screenshot 2026-05-29 at 3 03 47 PM" src="https://github.com/user-attachments/assets/7b989ff3-6c7c-406e-9c24-1444dc2265a9" />
  4. After restarting the machine I logged back in to start creating users for the domain. I opened the Active Directory Users and Computers and created an ADMIN folder for the admin user and a WORKERS folder for everyone else.I also gave Admin complete control while giving the users read only access. <img width="1512" height="982" alt="Screenshot 2026-05-29 at 3 14 02 PM" src="https://github.com/user-attachments/assets/b5a0cb07-4260-4958-b478-8ae124c3df70" />
<img width="1512" height="982" alt="Screenshot 2026-05-29 at 3 14 01 PM" src="https://github.com/user-attachments/assets/bf24a4ea-2d6a-4100-9ce5-92ad0c6eb69f" />
<img width="1512" height="982" alt="Screenshot 2026-05-29 at 3 09 30 PM" src="https://github.com/user-attachments/assets/f345df35-cd31-4901-ba44-474acddb1ba2" />
5. Now That I had the domain controller set up, I created a new VM running Windows 10. I also changed the DNS to be the same as the Controllers private IP. <img width="1512" height="982" alt="Screenshot 2026-05-29 at 3 20 03 PM" src="https://github.com/user-attachments/assets/34ce87c1-d1d3-41f8-ab58-422855bb67a9" />
<img width="1512" height="982" alt="Screenshot 2026-05-29 at 3 19 25 PM" src="https://github.com/user-attachments/assets/1f766c5c-575e-416f-837b-1f1a03bfc9da" />
6. I logged into the new VM and added it to the domain I created and gave domain users permission to remote connect to the client with the users and admins I created in step 4.<img width="1512" height="982" alt="Screenshot 2026-05-29 at 3 27 37 PM" src="https://github.com/user-attachments/assets/9c46175d-1bb9-4c82-82bf-9e03f997bcf9" />
<img width="1512" height="982" alt="Screenshot 2026-05-29 at 3 27 23 PM" src="https://github.com/user-attachments/assets/fcb01200-4600-482e-8585-8f1652fa1981" />
7. Once everything was created and set up, I went ahead and tested if it worked by logging in to the client VM with the domain user instead of the VM user and pass to make sure it was properly connected.  <img width="1512" height="982" alt="Screenshot 2026-05-29 at 3 36 32 PM" src="https://github.com/user-attachments/assets/8091db8b-bd51-4f4f-ba02-fe5029aad81d" />

