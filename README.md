<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial provides a step-by-step guide to configure the open-source help desk ticketing system osTicket after installation.

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used</h2>

- Windows 10 (21H2)

<h2>Post-Install Configuration Objectives</h2>

1. Log into the osTicket Admin panel
2. Configure Roles, Departments, & Teams
3. Allow anyone to create tickets
4. Configure Agents, Users, & SLA
5. Design Help Topics

<h2>Configuration Steps</h2>

1. **Log into the Admin Panel**  
   After logging into your helpdesk login page (`http://localhost/osTicket/scp/login.php`), you will be directed to the **agent** panel, where tickets created by end users are displayed for the helpdesk/admin.

   <img src="https://i.imgur.com/VlPO53m.png" height="80%" width="80%" alt="Agent Panel"/>

2. **Configure: Roles**  
   Roles define the permissions granted to agents based on their assigned department. Each role consists of a set of permissions that can be customized for agents within the department. There is no limit to the number of roles that can be created.

   - In the Admin panel, navigate to `Agents`, then click on `Roles`.
   - Create a new role and name it `Supreme Admin`.

   <img src="https://i.imgur.com/mzjHJiA.png" height="80%" width="80%" alt="Role Creation"/>
   <img src="https://i.imgur.com/Ef0Jpt0.png" height="80%" width="80%" alt="Role Permissions"/>

   Now, enable all available permissions for the "Supreme Admin" role.

   <img src="https://i.imgur.com/4p1Nff6.png" height="80%" width="80%" alt="Permission Settings"/>

3. **Configure: Departments**  
   Departments are used to direct tickets to specific areas of the helpdesk. You can configure various settings for each department.

   - In the Admin panel, go to `Agents`, then click on `Departments`.
   - Add a new department and name it **System Administrators**. Leave the remaining fields at their default settings and review the available options.

   <img src="https://i.imgur.com/5GkaoH3.png" height="80%" width="80%" alt="Department Settings"/>
   <img src="https://i.imgur.com/DHcMqqj.png" height="80%" width="80%" alt="Department Configuration"/>

4. **Configure: Teams**  
   Teams allow agents from various departments to collaborate on issues based on help topics or ticket filters.

   - In the Admin panel, navigate to `Agents`, then click on `Teams`.
   - Create two teams, naming them **Level I Support** and **Level II Support**.

   <img src="https://i.imgur.com/l6hdZrJ.png" height="80%" width="80%" alt="Team Creation"/>
   <img src="https://i.imgur.com/FdsELWj.png" height="80%" width="80%" alt="Team Setup"/>
   <img src="https://i.imgur.com/lvFxMQ4.png" height="80%" width="80%" alt="Team Configuration"/>

5. **Allow Anyone to Create Tickets**  
   By default, user registration is required to create tickets. To allow anyone to create tickets without registration:

   - In the Admin panel, go to `Settings`, then click on `User Settings`.
   - Uncheck `Registration Required` to allow unrestricted ticket creation.

   <img src="https://i.imgur.com/3iqKvL6.png" height="80%" width="80%" alt="User Settings"/>

6. **Configure: Agents**  
   Agents are assigned roles and departments to manage tickets. You can assign agents to specific departments and grant them additional access to other areas as needed.

   - In the Admin panel, go to `Agents`, then click on `Add New`.
   - Create two agents, naming them **Jane** and **John**.

   <img src="https://i.imgur.com/qv7K4Op.png" height="80%" width="80%" alt="Agent Creation"/>
   <img src="https://i.imgur.com/o0B7D42.png" height="80%" width="80%" alt="Agent Profile Setup"/>

7. **Configure: Users**  
   Users are able to create accounts and submit tickets. They can also track the status of existing tickets.

   - In the Admin panel, go to `Users`, then click on `Add New`.
   - Create two users and name them **Karen** and **Ken**.

   <img src="https://i.imgur.com/JvxHBib.png" height="80%" width="80%" alt="User Creation"/>
   <img src="https://i.imgur.com/efujVfj.png" height="80%" width="80%" alt="User Profile"/>

8. **Configure: SLA**  
   SLAs (Service Level Agreements) define the expected timeframes for resolving tickets.

   - In the Admin panel, go to `Manage`, then click on `SLA`.
   - Create three SLA plans, naming them **Sev-A**, **Sev-B**, and **Sev-C**. Set their grace periods and schedules as follows:
     - **Sev-A**: 1 hour, 24/7
     - **Sev-B**: 4 hours, 24/7
     - **Sev-C**: 8 hours, business hours

   <img src="https://i.imgur.com/pxblmkA.png" height="80%" width="80%" alt="SLA Setup"/>
   <img src="https://i.imgur.com/8wmF9e4.png" height="80%" width="80%" alt="SLA Configuration"/>
   <img src="https://i.imgur.com/aFHULuq.png" height="80%" width="80%" alt="SLA Details"/>

9. **Configure: Help Topics**  
   Help Topics help categorize and organize tickets for efficient assignment and resolution.

   - In the Admin panel, go to `Manage`, then click on `Help Topics`.
   - Create four Help Topics: **Business Critical Outage**, **Personal Computer Issues**, **Equipment Request**, and **Password Reset**.

   <img src="https://i.imgur.com/cqaaoI4.png" height="80%" width="80%" alt="Help Topics"/>
   <img src="https://i.imgur.com/v1JzYj4.png" height="80%" width="80%" alt="Help Topic Setup"/>

10. **View Created Tickets**  
   The selected tickets will be listed, along with the default tickets created during setup.

   <img src="https://i.imgur.com/Fs9fhuw.png" height="80%" width="80%" alt="Ticket Overview"/>

<p align="right"> Next up, *INSERT* </p>
