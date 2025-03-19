<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>

This is an easy to follow guide to installing osTicket, an open source ticketing system.<br />

[Required Files](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)



<h2>Environments and Technologies Used</h2>

- Windows 10 (22H2)
- Microsoft Azure (Virtual Machines)
- Remote Desktop (RDP)
- Internet Information Services (IIS)

<h2>List of Prerequisites</h2>

- Create a Virtual Machine in Azure
- Install osTicket
- Install HeidiSQL
- Install MySQL
- Install PHP
- Install Microsoft Visual C++ Redistributable

<h2>Installation Steps</h2>

First, create a resource group inside of Azure. Then, inside that resource group, create a Virtual Machine (VM). Choose a username and password, we'll be using them to connect to the VM using Remote Desktop (RDP). When creating the Virtual Machine (VM), allow Azure to create a new Virtual Network (Vnet).

![image](https://github.com/user-attachments/assets/aef8e8f1-3d8f-4c22-a7cf-81f78f553ce2)

Next, copy the public Ip Address of your VM, and connect via Remote Desktop, using the username and password you setup.

![image](https://github.com/user-attachments/assets/73ac104c-db04-4612-8ab6-20bc4bfa45c2)

Now inside the Windows 10 VM, we need to enable IIS with CGI.</p>
Control Panel -> Uninstall a Program -> Turn Windows Features on or off</p>
In the features window, enable Internet Information Services -> World Wide Web Services -> Application Development Features, enable CGI

![image](https://github.com/user-attachments/assets/06b5a116-a4f5-4b80-bbe2-c1b2e6c67b2c)

Now, unzip the zip file you downloaded. Open the folder and install PHP Manager</p>
(Located at the top of the page at the "required files" link)

![image](https://github.com/user-attachments/assets/d67fed57-b156-4996-bf3c-a6e0cf38752d)
















