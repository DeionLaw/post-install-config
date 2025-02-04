<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Pre-Reqs</h2>

- Completed install (https://github.com/DeionLaw/osticket-prereqs)
- Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
- End User osTicket URL: http://localhost/osTicket

<h2>Configuration Steps</h2>

![Screenshot 2025-02-03 164215](https://github.com/user-attachments/assets/46a562bc-22fa-4757-9cb5-64fbdcf7465a)
![Screenshot 2025-02-03 164354](https://github.com/user-attachments/assets/b66df54b-b02a-48cb-85ac-fffbffce048c)

<p>
Before getting started, I want to make you aware of the difference between the agent/admin panels. The first screenshot above is the Agent Panel where our workers would log in and begin work on tickets. The second screenshot is showing the Admin Panel, where higher ups would take care of backend settings and whatnot.
</p>
<br />

---

![Screenshot 2025-02-03 165039](https://github.com/user-attachments/assets/51bf7b90-029b-4198-a5bc-1ab747441336)
<p>
  Inside the Admin Panel, clicking 'Agents' and then 'Roles' will bring you to the current roles that are available in the default osTicket system. We will run through adding our own custom roles and departments now, go ahead navigate there as shown above.
</p>

---

![Screenshot 2025-02-03 175254](https://github.com/user-attachments/assets/2293fda1-a179-462b-b9ce-bc6be49b9cce)
<p>
  We are going to create a role called 'Super Admin', you can call it what you would like, this role is going to have every ability check marked, shown above is every permission checkmarked in the 'Tickets' section, go ahead and do the same for the 'Tasks' and 'Knowledgebase' sections
</p>

---

![Screenshot 2025-02-03 175455](https://github.com/user-attachments/assets/9f4b672d-ce2b-4c00-9cb5-32e059a3ee17)
![Screenshot 2025-02-03 175801](https://github.com/user-attachments/assets/7d3da04f-d547-4b19-9b30-8751341094be)

<p>
  Next we are going to add some departments. Click 'Agents', 'Departments', and then 'Add New Department'. We will create a 'SysAdmins' department, and add people to it later. Make sure this is a Top Level Department, as set in the parent section seen in the second screenshot above.
</p>

---

![Screenshot 2025-02-03 180044](https://github.com/user-attachments/assets/100f0351-4fec-41df-86f0-80d4cd47fd57)
![Screenshot 2025-02-03 180200](https://github.com/user-attachments/assets/a54b9fcf-dbad-46c4-ae24-383e290392d2)

<p>
  Next we will create a team, similar to the last step, click 'Agents', 'Teams', and 'Add New Team'. I will name my team 'Online Banking'. Click Create at the bottom.
</p>

---

![Screenshot 2025-02-03 180533](https://github.com/user-attachments/assets/8e713673-109d-477c-934d-c2fd560b66ed)
<p>
  We are also going to allow anyone to create tickets. You could choose to force users to be registered if you would like. To do this we will go to 'Settings', 'Users' and make sure "Require registration and login to create tickets" is unchecked.
</p>

---

![Screenshot 2025-02-03 180808](https://github.com/user-attachments/assets/d24a143b-d35c-4e59-95bc-98e86b2ec67a)
<p>
  Next we are going to add some Agents or the workers that would be working the tickets. Still being inside the Admin Panel, click 'Agents', and 'Add New Agent'
</p>

---

![Screenshot 2025-02-03 181223](https://github.com/user-attachments/assets/f7c5835f-e409-46cb-88cf-3f895d280f3a)
![Screenshot 2025-02-03 182308](https://github.com/user-attachments/assets/4c2e7661-ac22-47d4-a31a-744aba1113fe)
![Screenshot 2025-02-03 181249](https://github.com/user-attachments/assets/0eda4922-7905-43d7-a265-8097daf5aec4)
![Screenshot 2025-02-03 181314](https://github.com/user-attachments/assets/e13189f7-80b6-43f5-9919-c05677c2976e)

<p>
  We are going to make Jane Doe a 'Super Admin', under the 'Access' section and with her team being 'Online Banking' under the 'Teams' section. You can set her password by clicking 'Set Password' and unchecking the box that comes up. Make the password whatever you will remember. Make sure she is not set to 'Vacation Mode' also.
</p>

<p>Next we are going to do the same thing with a John Doe, set his department to 'Support' in the 'Access' section and 'Extended Access' in the dropdown to the right. </p>

---

![Screenshot 2025-02-03 182947](https://github.com/user-attachments/assets/29c9fde4-6eb0-4e99-a634-93c8df75aa63)
![Screenshot 2025-02-03 183040](https://github.com/user-attachments/assets/88c61785-0fb2-4c6a-ba0d-cbec9204658b)
![Screenshot 2025-02-03 183243](https://github.com/user-attachments/assets/009fa12a-1e93-4682-9ab2-cfb00469d2ea)


<p>Next we are going to add 2 users or customers in this case. They will be Karen and Ken. For this we will want to switch to the Agent Panel, then 'Users' and 'Add User'. Create 2 users, mine will be Ken and Karen. </p>

---

![Screenshot 2025-02-03 183505](https://github.com/user-attachments/assets/bda45790-f97b-41ef-8133-f8f66b0f98dd)

<p>
  Next we are going to add some SLAs, in the Admin Panel and select 'Manage' and 'SLA' then click 'Add SLA Plan'.
</p>

---

![Screenshot 2025-02-03 183805](https://github.com/user-attachments/assets/9d648b6b-20ca-4301-899a-e68590db88ca)
![Screenshot 2025-02-03 183944](https://github.com/user-attachments/assets/57555e1e-301c-4217-8abb-b7212d38ae9b)
![Screenshot 2025-02-03 184027](https://github.com/user-attachments/assets/bce0e0c2-86ab-438f-a95d-a16b8757c757)



<p>
  We are going to make Sev-A, Sev-B, and Sev-C. In Sev-A we will make the 'Grace Period' 1 hour, and the 'Schedule' to be 24/7.
</p>

<p>
  You can set your own custom SLAs but I will set Sev-B to be a 4 hour grace period, 24/7, and Sev-C to be business hours at 8 hour grace period.
</p>

---

![Screenshot 2025-02-03 185826](https://github.com/user-attachments/assets/73ee377f-6f09-4e7a-b79e-2be669e3cbdd)

<p>
  Lastly, we are going to create some Help Topics that will help orgainze the tickets. In the Admin Panel head to 'Manage' then 'Help Topics' and click 'Add New Help Topic'.
</p>

---

![Screenshot 2025-02-03 190332](https://github.com/user-attachments/assets/dfad1f6c-b2bb-4e81-88aa-74600886ff33)

<p>
  I am going to make mine 'Business Critical Outage', 'Personal Computer Issues', 'Password Reset', 'Equipment Request' and 'Other'. The first 3 will get the 'Parent Topic' of 'Report a Problem', 'Equipment Request' will get 
</p>

---

![Screenshot 2025-02-03 190543](https://github.com/user-attachments/assets/2f8a3348-5fa1-4039-be91-e9897304b27a)

<p>
  You should now have something similar to this. With that set up, everything is good to go to use in an at least practice environment!
</p>

