![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/a43e4997-9c1e-4b66-b8e9-5c0c953431c6)
# post-install-configuration
This tutorial continues the osTicket installation, which I've shared below if you still need to complete.

https://github.com/Timothyjdm44/osticket-prereqs

<h2>Environments and Technologies Used In Tutorial</h2>

- Microsoft Azure 
- Remote Desktop
- Internet Information Services (IIS)
- osTicket
- HeidSQL

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>STEPS USED</h2>

- Configure Roles
- Configure Departments
- Configure Teams
- Download and install the Rewrite Module
- Allow anyone to create tickets
- Configure Agents (employees)
- Configure Users (customers)
- Configure SLAs
- Configure Help Topics

<h2>Detailed Steps</h2>

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/ec8994a2-7f4c-4204-945b-ffff3b0e6ca4)

We'll first go to the login (http://localhost/osTicket/scp/login.php) to log in with the admin credentials from the previous tutorial.

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/db8fa13e-d6d1-414b-99e3-c7678eba81a5)

Next, click "Admin Panel" at the top right of the screen. The button will change to "Agent Panel" when navigating the admin panel.

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/263972dc-73a6-4218-ab44-0b8d58010838)

Then go to Agents > Roles > Add New Role

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/0199cc7f-d1ac-4fbd-ad75-4fc61606a59f)

Now, name the role to "Supreme Admin" and then allow all permissions in the next tab. Click "Add Role".

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/759702cc-2aef-48f7-bf98-8ee51450f54e)

Navigate to "Departments" and then click "Add New Department".

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/a2185c42-c153-4584-87e6-0bc835ed08d8)

Name the department to "SysAdmins" and then press "Create Dept".

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/7d1dc4be-760c-410b-9ca6-7923643dcfc1)

Head to the "Teams" panel and click "Create New Team". Name the new team "Level II Support" and press create.

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/6967e63b-0ad5-443a-9e12-3d515130b1e3)

Afterward, go to "Settings" > Users > Make sure the box for registration requirement is not checked > Make the method public > Save Changes.

Now go into the agent's panel and add a new agent.

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/5938425d-5f75-4f19-851a-cf4ebae9d981)

Create these accounts:

Name: Jane Doe
Email Address: jane.doe@osticket.com
Username: jane.doe
Set the password to "Password1"
Go to Access, set the department to SysAdmins, and select Supreme Admin for the role.
Go to the teams section and select Level II Support, then create.
After, create a second account for " John Doe"

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/2da446bf-b858-4faf-ae3d-a56467a3d502)

Then go to Agent panel > Users > Add User

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/1de3f300-566d-47b8-a8a7-8d9e0203ff7c)

Add the following users:

Email Address: ken@osticket.com

Full Name: Ken

Email Address: karen@osticket.com

Full Name: Karen

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/f9217137-2d72-45b6-8489-1a259b90c6b5)

Head to Admin Panel > Manage > SLA > Add New SLA Plan.

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/5ec4c756-d5d9-4238-abc0-a29697b21bed)

Next, add the following SLAs

SEV-A with a grace period of 1 hour, and a 24/7 schedule
SEV-B with a grace period of 4 hours, and a 24/7 schedule
SEV-C with a grace period of 8 hours, and a Mon-Fri business hours schedule

![image](https://github.com/Timothyjdm44/post-install-configuration/assets/142111972/5b3bdaa4-d902-4ac9-b772-d38af8996863)

Now, navigate to "Help Topics" and add the following help topics:

Business Critical Outage
Personal Computer Issues
Equipment Request
Password Reset







