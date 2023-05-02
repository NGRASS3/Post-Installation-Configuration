
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Installation-Configuration</h1>
This tutorial demonstrates the post configuration setup of the osTicket system.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Configure Roles / Departments / Teams / Agents / Users
- Configure multiple Service Level Agreements
- Configure Help Topics

<h2>Configuration Steps</h2>

Now that we have osTicket installed and running we will begin to configure various settings within the application as an Admin. For more information please refer to the original documentation located at: https://docs.osticket.com/en/latest/ 

To start create a new role entitled "Supreme Admin". Click Admin Panel -> Agents -> Roles -> Add New Role. When creating a  new role you can modify any specific roles permissions. In this case since we are creating a Supreme Admin they will be given all permissions. Keep in mind roles are used to determine an agents permissions so not all agents will have unlimited access. If you followed the steps correctly your screen should like something like this. As you can see we have successfully created the "Supreme Admin" role.

![image](https://user-images.githubusercontent.com/111653930/235697675-9476a9ca-2d33-4c3e-b8ec-a4dae7af0d03.png)


Next we will create a new Department. Select the Departments tab within the Agents tab, Admin Panel -> Agents -> Departments. Click "Add New Department" and name it System Administrators. Each Agent is assigned to a specific department depending on their assigned role within the helpdesk. In this case we will be creating the "System Administrators" department, this is where the Supreme Admins will be designated. Other specific settings such as SLAs, managers and other email settings can be set up in the departments tab.

![image](https://user-images.githubusercontent.com/111653930/235701515-b1bffc57-d445-4b89-8881-a3ae1641a43f.png)


Next we will configure some Teams. Teams allow you to pull Agents from different Departments and organize them to handle a specific issue or user via a Help Topic or Ticket Filter. To setup a team click Admin Panel -> Agents -> Teams -> Add New Team. Title this team Level II Support.

![image](https://user-images.githubusercontent.com/111653930/235702794-34024aaa-c3ca-452e-ac1b-f0fa6ef04344.png)


Now that we have created some roles and groups we will allow anyone to create a new ticket into the system. Click Admin Panel -> Settings -> User Settings. From here make sure "Require registration and login to create tickets" is **unchecked.** 

![image](https://user-images.githubusercontent.com/111653930/235704683-ed7b5fb9-7eab-49d7-9300-4fca4019a6a0.png)



