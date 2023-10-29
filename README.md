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

- Return to the Agents Tab
    -  Click Add New Agent

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/5f4413d1-5331-4004-bce6-b930daf48d50)

- From within the Agents Tab, enter the follwing basic account information
  -  Name: Jane Doe
  -  Email Address: jane@helpdesk.com


![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/ff93f651-361e-4def-a589-f43c96c7ce81)

- Click the Access sub tab
    -  Ensure 'System Administrators' and 'Supreme Admin' are selected from their respective dropdown menus.

- In order to grant more access to an agent, select another department from the drop down menu under Extended Access and click Add.
    -  The added department will need an assigned role i.e. Supreme Admin, so be sure to select one if extended access to other departments is granted.
  
![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/396e864d-7fe9-4eb4-883b-4dddff6c8da6)

- Note: the above steps can be repeated to add several more agents.  For example:
    - Name: John Doe
    - Email Address: john@helpdesk.com
    - Primary Department: Support, Limited Access
  
- Click Create once complete

<br/>

<h2>Configure Users/Customers</h2>

- Click the Agent Panel link in the top right corner
    -  Click the Users Tab
    -  Click Add User

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/bcab707d-c2ba-4f22-a421-15fbd1825c50)

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/d4c2632c-f92d-4287-8d29-3d8ca0bb199d)

- From within the new menu, enter the following basic information for your first user:
    -  Email Address: karen@customeremail.com (or whatever email you choose)
    -  Full Name: Karen Doe
- Select Add User

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/211b16f3-03d1-4f38-b3b0-bc37b1ce781b)

- Note: the above steps can be repeated to add several more users.  For example:
   
    - Email Address: Ken@customeremail.com
    - Name: Ken Doe
 
<br/>

  <h2>Configure SLA</h2>

- Click Admin Panel in the top right corner (will appear as 'Agent Panel' in the bottom image)
    -  Click the Manage tab
    -  Click the SLA sub tab
    -  Click Add New SLA Plan
 
![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/5f384229-1fe0-43bd-84c5-2d98ce81b261)

- From within the new menu, use the following information as the parameters for the new SLA Plans:

<br/>

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/3580a8eb-e045-4f5d-b8d7-681ea66cb19c)

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/4d7912f4-5040-450e-8957-b9edd8675e75)

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/f9313000-2f6c-4882-b077-60287c358459)

<b>Note:</b> The above SLA plans reflect different priortity levels of attention depending on hypothetical circumstances. <br>
Depening on the severity of a client's problem, it should be addressed with the time frame of the corresponding SLP plan. <br>


Examples of these are as follows:
- A critical error has occured, affecting the financial status of a company: <b>SEV-A</b>
- An employee has put in a request for a firmware udpate for a potentially slow operating system: <b>SEV-C</b>

<br/>

<h2>Configure Help Topics</h2>

  - Click the Manage tab
    -  Click <b>Help Topics</b>
    -  Click Add <b>New Help Topic</b> <br>
  
<b>Note:</b> Default Help topics can be seen listed below.  We will be adding four additional topics that can be further associated with the new SLA plans we previously added.

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/320d5098-a060-4f22-9926-fe108ef678ef)

<br/>

- From within the new menu, use the below images to add new topics to the already existing list of options.

    - Equipment Request: Sev-C
    - Password Reset: Sev-B
    - Personal Computer Issues: Sev-B
    - Report a Problem / Business Critical Outage: Sev-A
![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/0661a18d-514f-45dc-b3fc-7c8ecd253530)

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/92ee3321-7e1d-4b65-a2ba-bea734b20365)

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/e21ec622-d4a8-4c3f-9b4b-b1243f7e5671)




