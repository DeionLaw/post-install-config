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

<h2>Post-Install Configuration Objectives</h2>

- Everything listed in the pre-reqs (https://github.com/DeionLaw/osticket-prereqs)
- Admin/Analyst Login Page: http://localhost/osTicket/scp/login.php
- End User osTicket URL: http://localhost/osTicket

<h2>Configuration Steps</h2>

![Screenshot 2025-02-03 164215](https://github.com/user-attachments/assets/46a562bc-22fa-4757-9cb5-64fbdcf7465a)
![Screenshot 2025-02-03 164354](https://github.com/user-attachments/assets/b66df54b-b02a-48cb-85ac-fffbffce048c)

<p>
Before getting started, I want to make you aware of the difference between the agent/admin panels. The first screenshot above is the Agent Panel where our workers would log in and begin work on tickets. The second screenshot is showing the Admin Panel, where higher ups would take care of backend settings and whatnot.
</p>
<br />

![Screenshot 2025-02-03 165039](https://github.com/user-attachments/assets/51bf7b90-029b-4198-a5bc-1ab747441336)
<p>
  Clicking 'Agents' and then 'Roles' will bring you to the current roles that are available in the default osTicket system. We will run through adding our own custom roles and departments now, go ahead navigate there as shown above.
</p>
