# osticket-prereqs
<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Enable Internet Information Services/IIS
- Install Web Platform Installer
- Install MySQL
- Install C++
- Configure Permissions and Install osTicket


<h2>Installation Steps</h2>
To begin this project, we first have to login to Microsoft Azure portal. In order to create a virtual machine, a remote desktop, we have to make one using microsft Azure. We name it osticket-vm and set the username and password for this virtual machine. 

![image](https://github.com/user-attachments/assets/d5038f24-a6ad-441b-b2c8-0b080eb851d8)


Once we create the virtual machine, locate the public ip address. We will use this to connect to vm using remote desktop. If you are a Mac user you will have to download Microsoft Remote Desktop(RDP). Use the username and passowrd you entered while creating the VM.
![image](https://github.com/user-attachments/assets/e03b2166-85a9-4633-8acd-0f0c44e50d37)

<p>Once we are logged into the virtual machine, we will have to go into the control panel and enable Internet Information Services(IIS). Access the control panel then select uninstall a program. Off to the left select "Turn windows features on or off". A list will appear then you will enable Internet Information Services. Within IIS, you will select world wide web services, then go to "Application Development features". Make sure to enable CGI.

![image](https://github.com/user-attachments/assets/e60ebd9c-ddf8-47f6-acc5-67b2305e9025)

In order for the osTicket service to work, we have a folder of all the programs that we need to install. The list of programs needed are all included in the photo below. 

![image](https://github.com/user-attachments/assets/ab200f2c-4fb7-46c6-b068-8a12c89b05a9)

After we install all the programs needed for osTicket to run properly, we can extract the files to install the actual osTicket client. We use IIS to configure the last few things we need to get osTicket to run. We use HeidiSQL and create a database name osTicket inside.  Now we can use the MySQL credentials we made earlier to install osTicket. 

![image](https://github.com/user-attachments/assets/9cb73b96-fe26-4c5b-94b5-0c937bd0fc2d)
![image](https://github.com/user-attachments/assets/d05df7d5-d99a-449f-973d-13e0f764f70b)


After all that, you should be able to log in to osTicket and start using the platform. Success! 

![image](https://github.com/user-attachments/assets/d98616d6-cec7-4143-8eff-7baf236fcf08)







