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

- Configuring the following:
  - Roles
  - Departments
  - Teams
  - Allow anyone to create tickets
  - Agents 
  - Users (Customers)
  - SLA (Service Level Agreements)
  - Help Topics

<h2>Configuring Roles</h2>

- Log into osTicket with your created profile

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/f7664e9c-b69f-4349-bad5-e1665e76fed4)

<br />

-  As the Admin, your initial log in will be within the Admin Panel.  From here:
    - Click the Agents tab
    - Click Roles
    - Click Add New Roles 


![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/62a131a5-2315-4865-af19-3275a1838d74)

<br />

-  From here we will be adding the Supreme Admin Role
    -  Enter 'Supeme Admin' for the name of the role
    -  Click the Permissions tab
    -  Click all check boxes to grant full access to this role
    -  Click Add Role when complete
    

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/373cd15c-c0f8-4559-b981-acbf93af57f8)

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/e0aaf637-5b24-433d-9380-b9e67b4aeee4)

<br />

<h2>Configuring Departments</h2>

- Return to the Agents Tab
    - Click Departments
    - Click Add New Department
 
![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/043cbe96-2264-45ec-8aef-67a08a5a34d3)

<br />

- From here, we will be adding the System Administrators Department
    -  Enter 'System Adminstrators' for the name of the department
    -  Click Create Dept

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/5b77c144-4f74-41e7-8e89-79bfd2ecf8b3)

<br />

<h2>Configuring Teams</h2>

- Return to the Agents Tab
    -  Click Teams
    -  Click Add New Team
 
![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/be516c1b-2536-4b6e-b19e-9570dfa16fe2)

<br/>

- From here, we will be adding the Level II Support Team
    -  Enter 'Level II Support' for the name of the team
    -  Click Create Team

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/d1764ee3-7f67-4ce5-a4bd-7035e0278056)

 <br/>
 
<h2>Ticket Creation Settings</h2>

- Click the Settings Tab in the top left
- Click Users
- Ensure the box for '[ ] Require registration and login to create tickets' is left unchecked
    -  This will allow us to create tickets when logged in as our future users/customers without extra barriers
- Click Save Changes if necesssary

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/6fb76683-15fb-4b6a-a11d-54ad84eaa7c4)

<br/>

<h2>Configure Agents</h2>

