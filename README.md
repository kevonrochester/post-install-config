# post-install-config

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Configure osTicket, post-installation](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- OSTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Item 1
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>

![Screenshot 2024-01-03 162140](https://github.com/kevonrochester/post-install-config/assets/155024615/4a01e709-9c95-4666-863c-1b301a89fff9)
![Screenshot 2024-01-03 162227](https://github.com/kevonrochester/post-install-config/assets/155024615/e4033d3f-99a2-480e-8e92-008069ba5ebc)
![Screenshot 2024-01-03 162446](https://github.com/kevonrochester/post-install-config/assets/155024615/9a8c27b5-a6ea-4a9c-bf11-4839d05d3944)
![Screenshot 2024-01-03 163159](https://github.com/kevonrochester/post-install-config/assets/155024615/204e799f-d071-4a6c-a46e-467f79e3d3b5)
![Screenshot 2024-01-08 141411](https://github.com/kevonrochester/post-install-config/assets/155024615/9bd2def6-d226-4e89-bfe3-b0404e07d1ca)




In this tutorial we will show the core differences between "Admin Panel" and the "Agent Panel" and how to set things up

First since we are using a virtual machine for this turtorial . We will go to Portal.azure.com > create a resourse group > Virtual machines > copy the i.p address > use remote desktop ( or a mac equilant ) to sign into the desktop that we created with the credentials we set up for the virtual machine.
</p>
<br />

![Screenshot 2024-01-09 133654](https://github.com/kevonrochester/post-install-config/assets/155024615/373ff6ba-a7eb-43c8-a52c-c8ba50d519a9)


We will login to osTicket with (http://localhost/osTicket/scp/login.php and login with whatever your Credientials you created for the username and password.
</p>
<br />

![Screenshot 2024-01-09 134211](https://github.com/kevonrochester/post-install-config/assets/155024615/58a3c991-73e8-4013-9b77-64c72a42c472)

Now that we are login This is what the Agent Panel interface looks like. Also you can see that you can click Admin Panel in the top right corner so you also know that you are in the "Agent Panel" 
</p>
<br />

![Screenshot 2024-01-09 134436](https://github.com/kevonrochester/post-install-config/assets/155024615/522905db-8eb2-4795-93b1-52532a6b519e)

This is what the "Admin Panel" interface looks like similar as the Agent Panel you can see in the top right that it says Agent Panel so you know you are in the "Admin Panel". Also the "Admin Panel" has a lot more tabs for creative control.

![Screenshot 2024-01-09 135124](https://github.com/kevonrochester/post-install-config/assets/155024615/5d847aeb-2622-440b-bd83-a6ed4504279e)
![Screenshot 2024-01-09 135154](https://github.com/kevonrochester/post-install-config/assets/155024615/b77ccce1-d7b0-428d-bd94-fd3ff9a26c78)
![Screenshot 2024-01-09 135429](https://github.com/kevonrochester/post-install-config/assets/155024615/dce97192-3e68-4d35-8c80-388212203f90)
![Screenshot 2024-01-09 135513](https://github.com/kevonrochester/post-install-config/assets/155024615/196ff506-9e3b-451b-b3e0-b5471c7da2f9)
![Screenshot 2024-01-09 135525](https://github.com/kevonrochester/post-install-config/assets/155024615/cd1c3285-1962-4955-9313-33aa89d1b8b0)
![Screenshot 2024-01-09 135801](https://github.com/kevonrochester/post-install-config/assets/155024615/bdb47bc5-5856-494c-aa3b-33957a031106)

We will be configuring roles on the "Admin Panel" and create a new role called Supreme Admin and give it Permissions ( the name doesn't matter as it can technically be whatever you want it to be). We will Click Agents > Roles > Add New Role > ( Name the Role) > Permissions > Add Role. We went ahead and gave our new role " Supreme Admin " all permissions and when completed it will say "Succuessfully Added Role." at the upper center of the screen in a green bar.













