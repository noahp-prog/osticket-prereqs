<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>

This is an easy to follow guide to installing osTicket, an open source ticketing system.<br />

# [Required Files](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6)



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

Now, unzip the zip file you downloaded. Open the folder and install PHP Manager.</p>
[Files Located Here](https://drive.google.com/drive/u/0/folders/1APMfNyfNzcxZC6EzdaNfdZsUwxWYChf6) as well.

![image](https://github.com/user-attachments/assets/d67fed57-b156-4996-bf3c-a6e0cf38752d)

From the same folder, accept the terms and install Rewrite Module.

![image](https://github.com/user-attachments/assets/27792d1d-aacb-4245-9160-721e7f6ba814)

Once installed, navigate to the (C:) Drive, and create a folder there called **PHP**.

![image](https://github.com/user-attachments/assets/dbe02db4-ab46-451a-ad65-27b872c3db70)

After the PHP folder is created, extract PHP 7.3.8 to the PHP folder you created on the (C:) Drive.

![image](https://github.com/user-attachments/assets/0ff6d663-c00c-458e-92b6-26db4cc5804f)

Next, we are going to install Microsoft Visual C++ Redistributable.</p>
Agree to the terms and install.

![image](https://github.com/user-attachments/assets/27d167f2-7849-42b8-ae7d-e58c53e2869c)

We are now going to install MySQL. Choose "typical setup", once installed, launch the MySQL Configuration Wizard.

![image](https://github.com/user-attachments/assets/01d3c2f8-e7b6-40d2-a46a-9ad88f8907f2)

Now, inside the configuration wizard, choose "standard configuration" then setup a username and password that will be used to access your osTicket database.

![image](https://github.com/user-attachments/assets/7566db98-732c-436a-bf6d-e2cc74b66eb0)
























