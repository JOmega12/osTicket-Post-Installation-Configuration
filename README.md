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
![cofnigureAgent](https://github.com/user-attachments/assets/920ac9e0-ba45-468b-9cc1-f9f3d04dd71c)

- Click Add Role then you should get something like this:
![SupremeAdminEndResult](https://github.com/user-attachments/assets/fcf3b8b7-34cb-466b-a147-b4c41f6f05e4)

<h3>Configure Departments (used for ticket visibility)</h3>

- In the Admin/Analyst Page, go to Admin Panel -> Agents -> Departments
- Click 'Create Dept'
  
![createDepartment](https://github.com/user-attachments/assets/8fa85262-ec3d-43b5-8877-4cdbd759f93c)

- This will be the result: 
![createBothSysadminAndSupport](https://github.com/user-attachments/assets/c28c823e-1da4-4fa1-963d-e01655ad5b12)

<h3>Configure Teams </h3>

- In the Admin/Analyst Page, go to Admin Panel -> Agents -> Teams ( Pull Agents from different Departments)
- Create 'Online Banking' Team

![createTeam](https://github.com/user-attachments/assets/a5bef8fd-94fe-48cd-a666-1fafe5d858d0)

<h3>Allow Anyone To Create Tickets</h3>

- In the Admin/Analyst Page, go to Admin Panel -> Settings -> Users
- Disable "Registration Required" for creating tickets then Save Changes
![createNoRegisterUserTicket](https://github.com/user-attachments/assets/5a56bd07-02e1-4f9a-8920-4acf5cd04fe5)

<h3>Configure Agent Workers</h3>

- Create Jane under SysAdmin Department
![createJaneAdmin_superAdmin](https://github.com/user-attachments/assets/f63d985c-f1f8-418f-b24d-a2cda83351df)
![selectSysadminDep_jane](https://github.com/user-attachments/assets/1911c4f1-615e-4d8a-bb2c-3bb5d486a52b)


- Create John under Support Department
![createJohn](https://github.com/user-attachments/assets/184611c0-6719-4c7a-8b1f-d1505b9c052a)


- make sure to set both agents' Password to `Password1`


<h3>Configure Users(customers)</h3>

- In Agent Panel -> Users -> Add New

![createNewUsers(customers)](https://github.com/user-attachments/assets/bd3fa43a-0c8c-49d1-9626-df88d92a94ad)
- Create Karen

![createKaren](https://github.com/user-attachments/assets/3396e564-b96d-4d3c-a4e9-f7de1de03b31)

- Create Ken

<h3>Configure SLA</h3>

- Within Admin Panel -> Manage -> SLA
![ManageSLA](https://github.com/user-attachments/assets/9757311c-7bb0-4176-9bf8-a210bfb031e8)

- Then click on "Add New SLA Plan" 
![AddNewSLAPlan_SevA](https://github.com/user-attachments/assets/5fe29d80-b5d0-4d29-930b-707065764d83)

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
![EndGameSLA_Plan](https://github.com/user-attachments/assets/dc8cbf59-1678-47f5-b11e-5299d94afceb)

<h3>Configure Help Topics</h3>

- Within Admin Panel -> Manage -> Help Topics
![directHelpTopics](https://github.com/user-attachments/assets/49d0a457-8ef7-448a-80f1-2e6ed520a20e)

- Then click on "Add New Help Topic"
![createHelpTopc](https://github.com/user-attachments/assets/8e5e608c-1175-44b3-8b1b-f137884de777)

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
![endGoalhelpTopics](https://github.com/user-attachments/assets/6b62ca94-fcd1-4599-9049-bb884f9a0d36)

<h2>Conclusion</h2>
<p>Congratulations! You've fully setup a working ticketing system that can be used as tickets to configure day to day operations in the IT department. If you want to see the ticketing lifecycle, click <a href="https://github.com/JOmega12/osTicket-Ticket-Lifecycle-Examples">here</a></p>
<br />
