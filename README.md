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

- Configure Roles (for grouping permissions)
- Configure Departments (Ticket Visibility, Help Desk vs SysAdmins, vs Networking)
- Configure Teams
- Configure Agents (workers)
- Configure Users (customers)
- Configure SLA
- Configure Help Topics (For when users create a ticket)

<h2>Configuration Steps</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Summary: Configuring Roles in osTicket

Log in as Admin

Open your web browser and log in to the osTicket admin panel. (http://localhost/osTicket/scp/login.php)

Navigate to Roles

Go to Admin Panel → Agents → Roles.

Click Add New Role.

Create and Configure the Role

Name the role Supreme Admin.

Go to Permissions and check all the boxes to grant full access.

Move to the Tasks section and check all boxes.

Go to Knowledgebase and check the necessary permissions.

Click Add Role to save the changes.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Summary: Configuring Departments in osTicket

Access the Admin Panel

Navigate to Departments

Go to Agents → Departments.

Click Add New Department.

Create a New Department

Parent Department: Select Support.

Department Name: Enter SysAdmins.

Scroll down and click Create Department.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Summary: Configuring Teams and User Ticket Settings in osTicket

To create a team

Go to the Admin Panel.

Go to Agents → Teams.

Click Create New Team.

Team Name: Enter Online Banking (or any preferred name).

Click Create Team to save.

Allow Unregistered Users to Create Tickets

In the Admin Panel, go to Settings → User Settings.

Locate the option "Require registration and login to create tickets".

Ensure the box is unchecked so that unregistered users can submit tickets.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Summary: Configuring Agents in osTicket

Access the Admin Panel

Navigate to Agents → Add New Agent.

Create Agent: Jane Doe

Full Name: Jane Doe

Email: (Make up an email, e.g., jane.doe@example.com)

Username: jane

Password: Password1

Uncheck the box for "Send the agent a password reset email".

Uncheck the box for "Require password change at next login".

Assign Jane’s Permissions

Access Tab:

Department: Support / SysAdmins

Role: Supreme Admin

Teams Tab:

Assign Jane to Online Banking team.

Click Create Agent.

Create Agent: John Doe

Full Name: John Doe

Email: (Make up an email, e.g., john.doe@example.com)

Username: john

Password: Password1

Uncheck the box for "Send the agent a password reset email".

Uncheck the box for "Require password change at next login".

Assign John’s Permissions

Access Tab:

Department: Support

Role: View Only

Teams Tab:

Assign John to Online Banking team.

Click Create Agent.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Summary: Configuring Users in osTicket

Access the Agent Panel

Navigate to Users → Add New User.

Create a New User

Full Name: Karen

Email Address: (Make up an email, e.g., karen@example.com)

Click Add User to save.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Summary: Configuring SLAs in osTicket

Access the Admin Panel

Navigate to Manage → SLA Plans.

Create SLA Plans

Sev-A:

Grace Period: 1 hour

Schedule: 24/7

Click Add Plan

Sev-B:

Grace Period: 4 hours

Schedule: 24/7

Click Add Plan

Sev-C:

Grace Period: 8 hours

Schedule: Monday-Friday, 8 AM - 5 PM

Click Add Plan
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Summary: Configuring Help Topics in osTicket

Access the Admin Panel

Navigate to Manage → Help Topics.

Click Add New Help Topic to create a new topic.

Create Help Topics

Business Critical Outage

Parent Topic: Report a Problem

Click Add

Personal Computer Issues

Parent Topic: Report a Problem

Click Add

Equipment Request

Parent Topic: General Inquiry

Click Add

Password Reset

Parent Topic: Report a Problem

Click Add

Other

Parent Topic: General Inquiry

Click Add
</p>
<br />
