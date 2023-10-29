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

- Windows 10 22H2

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

-  As the Admin, your initial log in will be within the <b>Admin Panel.</b>  From here:
    - Click the <b>Agents</b> tab
    - Click <b>Roles</b>
    - Click <b>Add New Roles</b> 


![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/62a131a5-2315-4865-af19-3275a1838d74)

<br />

-  From here we will be adding the Supreme Admin Role
    -  Enter 'Supeme Admin' for the name of the role
    -  Click the <b>Permissions</b> tab
    -  Click all [ ]check boxes to grant full access to this role
    -  Click <b>Add Role</b> when complete
    

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/373cd15c-c0f8-4559-b981-acbf93af57f8)

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/e0aaf637-5b24-433d-9380-b9e67b4aeee4)

<br />

<h2>Configuring Departments</h2>

- Return to the <b>Agents Tab</b>
    - Click <b>Departments</b>
    - Click <b>Add New Department</b>
 
![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/043cbe96-2264-45ec-8aef-67a08a5a34d3)

<br />

- From here, we will be adding the System Administrators Department
    -  Enter 'System Adminstrators' for the name of the department
    -  Click <b>Create Dept</b>

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/5b77c144-4f74-41e7-8e89-79bfd2ecf8b3)

<br />

<h2>Configuring Teams</h2>

- Return to the <b>Agents</b> Tab
    -  Click <b>Teams</b>
    -  Click <b>Add New Team</b>
 
![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/be516c1b-2536-4b6e-b19e-9570dfa16fe2)

<br/>

- From here, we will be adding the Level II Support Team
    -  Enter 'Level II Support' for the name of the team
    -  Click <b>Create Team</b>

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/d1764ee3-7f67-4ce5-a4bd-7035e0278056)

 <br/>
 
<h2>Ticket Creation Settings</h2>

- Click the <b>Settings</b> tab in the top left
- Click <b>Users</b>
- Ensure the box for <b>[ ] Require registration and login to create tickets</b> is left unchecked
    -  This will allow us to create tickets when logged in as our future users/customers without extra barriers
- Click <b>Save Changes</b> if necesssary

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/6fb76683-15fb-4b6a-a11d-54ad84eaa7c4)

<br/>

<h2>Configure Agents</h2>

- Return to the Agents Tab
    -  Click Add New Agent

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/5f4413d1-5331-4004-bce6-b930daf48d50)

<br />

- From within the <b>Agents</b> Tab, enter the follwing basic account information
  -  Name: Jane Doe
  -  Email Address: jane@helpdesk.com

<b>Note:</b> The <b>Permissions</b> and <b>Teams</b> tabs can be further customized for agent categorization reasons, but is not currently necessary for this exercise. 


![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/ff93f651-361e-4def-a589-f43c96c7ce81)

<br />

- Click the <b>Access</b> sub tab
    -  Ensure 'System Administrators' and 'Supreme Admin' are selected from their respective dropdown menus.

- In order to grant more access to an agent, select another department from the drop down menu under <b>Extended Access</b> and click <b>Add</b>.
    -  The added department will need an assigned role i.e. Supreme Admin, so be sure to select one if extended access to other departments is granted.
  
![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/396e864d-7fe9-4eb4-883b-4dddff6c8da6)

<br />

- <b>Note:</b> the above steps can be repeated to add several more agents.  For example:
    - Name: John Doe
    - Email Address: john@helpdesk.com
    - Primary Department: Support, Limited Access
  
- Click <b>Create</b> once complete

<br/>

<h2>Configure Users/Customers</h2>

- Click the <b>Agent Panel</b> link in the top right corner
    -  Click the <b>Users</b> Tab
    -  Click <b>Add User</b>

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/bcab707d-c2ba-4f22-a421-15fbd1825c50)

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/d4c2632c-f92d-4287-8d29-3d8ca0bb199d)

<br />

- From within the new menu, enter the following basic information for your first user:
    -  Email Address: karen@customeremail.com (or whatever email you choose)
    -  Full Name: Karen Doe
- Select <b>Add User</b>

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/211b16f3-03d1-4f38-b3b0-bc37b1ce781b)

- <b>Note:</b> the above steps can be repeated to add several more users.  For example:
   
    - Email Address: Ken@customeremail.com
    - Name: Ken Doe
 
<br/>

  <h2>Configure SLA</h2>

- Click <b>Admin Panel</b> in the top right corner (will appear as 'Agent Panel' in the bottom image)
    -  Click the <b>Manage</b> tab
    -  Click the <b>SLA</b> sub tab
    -  Click <b>Add New SLA Plan</b>
 
![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/5f384229-1fe0-43bd-84c5-2d98ce81b261)

<br />

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

- From within the new menu, use the below information and images to add new topics to the already existing list of options.

    - Equipment Request
    - Password Reset
    - Personal Computer Issues
    - Business Critical Outage


![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/92ee3321-7e1d-4b65-a2ba-bea734b20365)

<br />


<b>Note:</b> In the <b>New ticket options</b> tab several options can be selected to further categorize your help topics for orgrizational purpurposes and convenience.  When we later address these tickets in the next tutorial, we will notice these details can also be completed when directly responding to the user who originally submitted them.

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/e21ec622-d4a8-4c3f-9b4b-b1243f7e5671)

![image](https://github.com/dgrofsick/osticket-post-install/assets/148154704/0661a18d-514f-45dc-b3fc-7c8ecd253530)


