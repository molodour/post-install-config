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
<p>- Supreme Admin -> Give all permissions</p><br />
![Capture1](https://github.com/user-attachments/assets/cc062ee1-7c1c-4082-bbf1-17c84866898b)


-----------------------------


<p>Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)</p>
<p>Admin Panel -> Agents -> Departments</p>
<p>- SysAdmins</p><br />

<p>Configure Teams</p>
<p>Admin Panel -> Agents -> Teams (Pull Agents from different Departments)</p>
<p>- Online Banking</p><br />
-----------------------------

<p>Allow anyone to create tickets</p>
<p>Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)</p>
<p>Registration Required: Require registration and login to create tickets </p><br />
-----------------------------

<p>Configure Agents (workers)</p>
<p>Admin Panel -> Agents -> Add New</p>
<p>- Jane (Dept: SysAdmins)</p>
<p>- John (Dept: Support)</p><br />
-----------------------------

<p>Configure Users (customers)</p>
<p>Agent Panel -> Users -> Add New</p>
<p>- Karen</p>
<p>- Ken</p><br />
-----------------------------

<p>Configure SLA</p>
<p>Admin Panel -> Manage -> SLA</p>
<p>- Sev-A (Grace Period: 1 hour, Schedule: 24/7)</p>
<p>- Sev-B (Grace Period: 4 hours, Schedule: 24/7)</p>
<p>- Sev-C (Grace Period: 8 hours, Business Hours)</p><br />
-----------------------------

<p>Configure Help Topics (For when users create a ticket)</p>
<p>Admin Panel -> Manage -> Help Topics</p>
<p>- Business Critical Outage</p>
<p>- Personal Computer Issues</p>
<p>- Equipment Request</p>
<p>- Password Reset</p>
<p>- Other</p>

