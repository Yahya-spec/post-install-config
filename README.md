<p align="center">
  <img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
In this home lab, I will perform Sysadmin tasks on osTicket. I will use both admin and user panels to create, configure, and assign roles and ticket settings.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)

<h2>Configuration Steps</h2>

<h3>Admin/Analyst Login Page:</h3>
<p><a href="http://localhost/osTicket/scp/login.php">http://localhost/osTicket/scp/login.php</a></p>

<h3>End Users osTicket URL:</h3>
<p><a href="http://localhost/osTicket">http://localhost/osTicket</a></p>

<h3>Acknowledge Agent Panel vs Admin Panel</h3>
<p><img src="https://github.com/user-attachments/assets/5173b4ca-7833-4f4c-acb0-5b01779e6b8a" alt="Configure Roles"></p>

<h3>Configure Roles (for grouping permissions)</h3>
<p>Admin Panel -> Agents -> Roles</p>
<p>Supreme Admin</p>
<p><img src="https://github.com/user-attachments/assets/00adf293-029f-437a-9a4d-de5f6280c3a6" alt="Role Configuration"></p>

<h3>Configure Departments (Ticket Visibility)</h3>
<p>Admin Panel -> Agents -> Departments</p>
<p>SysAdmins</p>
<p><img src="https://github.com/user-attachments/assets/fa91d680-07ec-41fc-b831-5a9fc7331ea9" alt="Department Configuration"></p>

<h3>Configure Teams</h3>
<p>Admin Panel -> Agents -> Teams (Pull Agents from different Departments)</p>
<p>Online Banking</p>
<p><img src="https://github.com/user-attachments/assets/fbe529b3-a295-4a60-a183-18542923e619" alt="Teams Configuration"></p>

<h3>Allow anyone to create tickets</h3>
<p>Admin Panel -> Settings -> User Settings (UNCHECK: unregistered users can create tickets)</p>
<p>Registration Required: Require registration and login to create tickets</p>

<h3>Configure Agents (workers)</h3>
<p>Admin Panel -> Agents -> Add New</p>
<p>Jane (Dept: SysAdmins)</p>
<p>John (Dept: Support)</p>
<p><img src="https://github.com/user-attachments/assets/04f0a3c3-3898-4db9-8ea9-44e196db2af6" alt="Agent Configuration"></p>

<h3>Configure Users (customers)</h3>
<p>Agent Panel -> Users -> Add New</p>
<p>Marty</p>
<p>Roman</p>
<p><img src="https://github.com/user-attachments/assets/cd174c87-cb49-49cd-bf65-29940388025e" alt="User Configuration"></p>

<h3>Configure SLA</h3>
<p>Admin Panel -> Manage -> SLA</p>
<ul>
  <li>Sev-A (Grace Period: 1 hour, Schedule: 24/7)</li>
  <li>Sev-B (Grace Period: 4 hours, Schedule: 24/7)</li>
  <li>Sev-C (Grace Period: 8 hours, Business Hours)</li>
</ul>
<p><img src="https://github.com/user-attachments/assets/05df48ac-8fe2-41b4-80af-86fa8b36d0aa" alt="SLA Configuration"></p>

<h3>Configure Help Topics (For when users create a ticket)</h3>
<p>Admin Panel -> Manage -> Help Topics</p>
<ul>
  <li>Business Critical Outage</li>
  <li>Personal Computer Issues</li>
  <li>Equipment Request</li>
  <li>Password Reset</li>
  <li>Other</li>
</ul>
<p><img src="https://github.com/user-attachments/assets/712ad11f-1e71-4e1e-b517-233fb56b850e" alt="Help Topics Configuration"></p>

<h2>Takeaways and Key Skills Developed</h2>
In this project, I configured osTicket by managing user roles, departments, and ticket settings. I set up roles to group permissions, defined departments for ticket visibility, and created teams by combining agents from different departments. I required user registration before ticket creation, added agents and users, and set up SLAs for different severity levels. Additionally, I created help topics to categorize tickets. This hands-on experience helped me learn to manage user roles, workflows, and settings in a ticketing system to improve help desk efficiency.
