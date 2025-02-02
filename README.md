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

<p>Admin/Analyst Login Page:</p>
<p>http://localhost/osTicket/scp/login.php </p>

<p>End Users osTicket URL:</p>
<p>http://localhost/osTicket </p>

-----------------------------

<p>Acknowledge Agent Panel vs Admin Panel</p>

<p>Configure Roles (for grouping permissions)</p>
<p>Admin Panel -> Agents -> Roles</p>
<p>- Supreme Admin -> Give all permissions</p>

![Capture1](https://github.com/user-attachments/assets/cc062ee1-7c1c-4082-bbf1-17c84866898b)


-----------------------------


<p>Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)</p>
<p>Admin Panel -> Agents -> Departments</p>
<p>- SysAdmins</p><br />

![Capture2](https://github.com/user-attachments/assets/a5b3bea0-c5d9-4bd9-a790-b4c55a095e58)

-----------------------------

<p>Configure Teams</p>
<p>Admin Panel -> Agents -> Teams (Pull Agents from different Departments)</p>
<p>- Online Banking</p><br />

![Capture3](https://github.com/user-attachments/assets/66f1eb75-909e-40f9-b3cc-c7d66d189aa7)

-----------------------------

<p>Allow anyone to create tickets</p>
<p>Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)</p>
<p>Registration Required: Require registration and login to create tickets </p><br />

![Capture4](https://github.com/user-attachments/assets/b91c484c-4b3c-4318-8171-14c2aecd7c16)

-----------------------------

<p>Configure Agents (workers)</p>
<p>Admin Panel -> Agents -> Add New</p>
<p>- Jane (Dept: SysAdmins)</p>
<p>- John (Dept: Support)</p><br />

![Capture5](https://github.com/user-attachments/assets/2427ad1d-37ae-4114-ad11-34880dec9151)
![Capture6](https://github.com/user-attachments/assets/c62f6d85-5fc9-4795-9bdd-8a0bf088a745)
![Capture7](https://github.com/user-attachments/assets/29a19570-bfd7-4974-b239-481a87dd17b7)

-----------------------------

<p>Configure Users (customers)</p>
<p>Agent Panel -> Users -> Add New</p>
<p>- Karen</p>
<p>- Ken</p><br />

![Capture8](https://github.com/user-attachments/assets/6b97c058-59f3-43f2-be53-82f3f9c72119)

-----------------------------

<p>Configure SLA</p>
<p>Admin Panel -> Manage -> SLA</p>
<p>- Sev-A (Grace Period: 1 hour, Schedule: 24/7)</p>
<p>- Sev-B (Grace Period: 4 hours, Schedule: 24/7)</p>
<p>- Sev-C (Grace Period: 8 hours, Business Hours)</p><br />

![Capture9](https://github.com/user-attachments/assets/13ca217d-5cd0-44a7-9efc-91c60cd68aa4)

-----------------------------

<p>Configure Help Topics (For when users create a ticket)</p>
<p>Admin Panel -> Manage -> Help Topics</p>
<p>- Business Critical Outage</p>
<p>- Personal Computer Issues</p>
<p>- Equipment Request</p>
<p>- Password Reset</p>
<p>- Other</p>

![Capture0](https://github.com/user-attachments/assets/87e1f6fc-ab5e-4436-8a1c-7925ffeb1940)


