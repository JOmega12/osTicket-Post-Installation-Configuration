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

- Configure Agent Roles
- Configure Departments
- Configure Teams
- Allow Anyone To Create Tickets
- Confiure Agent Workers
- Configure Users(customers)
- Configure SLA
- Configure Help Topics

<h2>Configuration Steps</h2>

- First, we are starting with this link while logging in to your information: <a href="http://localhost/osTicket/scp/login.php">Admin/Analyst Login Page</a>
- If you haven't set up osTicket yet, please go to the setup osTicket link <a href="https://github.com/JOmega12/osTicket-Prerequisites-and-Installation">here</a>

<h3>Configure Agent Roles</h3>

- In the Admin/Analyst Page, go to Admin Panel -> Agents -> Roles
- Create 'Super Admin' as a name and give yourself ALL permissions
- Click Add Role then you should get something like this:

<h3>Configure Departments (used for ticket visibility)</h3>

- In the Admin/Analyst Page, go to Admin Panel -> Agents -> Departments
- Click 'Create Dept'


<h3>Configure Teams </h3>

- In the Admin/Analyst Page, go to Admin Panel -> Agents -> Teams ( Pull Agents from different Departments)
- Create 'Online Banking' Team

<h3>Allow Anyone To Create Tickets</h3>

- In the Admin/Analyst Page, go to Admin Panel -> Settings -> Users
- Disable "Registration Required" for creating tickets then Save Changes

<h3>Configure Agent Workers</h3>

- Create Jane under SysAdmin Department
- Create John under Support Department
- make sure to set both agents' Password to `Password1`

<h3>Configure Users(customers)</h3>

- Create Karen
- Create Ken

<h3>Configure SLA</h3>

- Within Admin Panel -> Manage -> SLA

- Then click on "Add New SLA Plan" 

- We are going to create 3 SLA Plans

1) Sev-A
   - Grace Period: 1 hour
   - Schedule: 24/7
2) Sev-B
   - Grace Period: 4 hours
   - Schedule: 24/7
3) Sev-C
   - Grace Period: 8 hours
   - Schedule: Business Hours

<h3>Configure Help Topics</h3>

- Within Admin Panel -> Manage -> Help Topics
- Then click on "Add New Help Topic"
- We are going to create these help topics:
  - Help Topic 1:
    - Topic: Business Critical Outage
    - Parent Topic: Report a Problem
  - Help Topic 2:
    - Topic: Personal Computer Issues
    - Parent Topic: Report a Problem
  - Help Topic 3:
    - Topic: Equipment Request
    - Parent Topic: General Inquiry
  - Help Topic 4:
    - Topic: Password Reset
    - Parent Topic: Report a Problem
  - Help Topic 5:
    - Topic: Other
    - Parent Topic: General Inquiry

<br />
