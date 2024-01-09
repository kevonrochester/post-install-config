# post-install-config

<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- OSTicket

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- Agent Panel & Admin Panel
-  Roles
- Departments
- Teams
- Agents
- Users
- SLA
- Help Topics

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

![Screenshot 2024-01-09 140129](https://github.com/kevonrochester/post-install-config/assets/155024615/12ba079a-af08-4548-8c6d-97d1385bbf61)
![Screenshot 2024-01-09 140344](https://github.com/kevonrochester/post-install-config/assets/155024615/b89162fd-8745-47a8-9ced-72b4f785df86)

Now will Create Some departments because Tickets are routed through Departments in the help desk ( again the name of the departments technically doesn't matter but is used to organize the different tickets in a real world scenario ) We will be in the  Admin Panel > Click - Agents > Departments > Add New Department . This is where you will name the department . Configure your SLA ( Service Level Agreement ) , set managers , email settings and all different type of settings associated with configuring the Department the way you would want it to be.

![Screenshot 2024-01-09 140941](https://github.com/kevonrochester/post-install-config/assets/155024615/684c2a83-b161-450d-af72-26c28d6801b3)
![Screenshot 2024-01-09 141138](https://github.com/kevonrochester/post-install-config/assets/155024615/e419cbed-4fbf-4a22-90a8-72167aa27f68)
![Screenshot 2024-01-09 141506](https://github.com/kevonrochester/post-install-config/assets/155024615/a2fc78ef-df37-4874-9585-013af8fef177)

Now i will be showing you how to create a team ( similar to real world scenario there will be different people working on different set of tickets etc and is normally organized but not subjected to different teams ) We will be in the Agent Panel > Click - Agents > Teams > Add New Team. I will be naming the team, Team B ( but again the team name doesn't techanically matter ). We can set a " Team Lead Here " Ect . Then we will click " Create Team " and the Green panel saying successful will indicate that the team was created.

![Screenshot 2024-01-09 142016](https://github.com/kevonrochester/post-install-config/assets/155024615/43efc21f-9b10-443b-8dfc-bf828bf8979f)



Now we will show you how to have anyone create a ticket if you deicde that not only users and agents can make tickets. ( In a real world scenario so people can get help from the help desk who is not in the help desk department or a user but every situation can be different ). Admin Panel > Click -  Settings > Users > Click Require Reigistration and login to create tickets ( keeping the box unchecked )  > Click save Changes. Again greeted by the green successful banner when you know it is complete.

![Screenshot 2024-01-09 142423](https://github.com/kevonrochester/post-install-config/assets/155024615/cf8aa4be-0303-43b3-ab41-fcb870c6e7af)
![Screenshot 2024-01-09 142932](https://github.com/kevonrochester/post-install-config/assets/155024615/1ae70717-4237-45a4-955c-c41f83b31a71)
![Screenshot 2024-01-09 142956](https://github.com/kevonrochester/post-install-config/assets/155024615/2159874f-e1d5-446d-9f6d-80800da16179)


Next We will Create Agents ( basically the people who will be working in the help desk with there own login information so we know in a real world scenario who is working on and assign to what tickets etc ).  We will be in the Admin Panel > Click Agents > Agents > Add New Agent. We will be creating two agents for this demo which will be Jane doe and John Doe. You can set the password for the Agents, sent it to their email and even have them reset it after they login or not again up to you By clicking on Set password and following the Prompt.

![Screenshot 2024-01-09 143443](https://github.com/kevonrochester/post-install-config/assets/155024615/1678d075-083f-4a46-90ba-4b9a23105578)
![Screenshot 2024-01-09 143623](https://github.com/kevonrochester/post-install-config/assets/155024615/cc276265-eeb8-4142-996f-4672a829e614)
![Screenshot 2024-01-09 143637](https://github.com/kevonrochester/post-install-config/assets/155024615/ce01958e-4d17-4096-be8c-7391cdcc7af3)

The "Access" tab is to assign the department and roles of the agent while extended access is if you want the agent in multiple departments. The "Permissions" tab is to set permissions of the agent. The "Teams" tab is to assign them to any teams of your choice. And you can click Create when you are finished Greeted by the green panel again.

![Screenshot 2024-01-09 144221](https://github.com/kevonrochester/post-install-config/assets/155024615/92c45927-edd0-4123-aeb2-02f5f21e8a77)
![Screenshot 2024-01-09 144443](https://github.com/kevonrochester/post-install-config/assets/155024615/8dc051ee-58f0-4216-b195-88b3f43775f4)
![Screenshot 2024-01-09 144536](https://github.com/kevonrochester/post-install-config/assets/155024615/7cd8a79c-f663-4b7c-b8e2-69f944ea97bf)

Moving forward we will create users ( Which is the people who will be creating tickets for the help desk to solve ). We will go to the Agent Panel > Click - Users > Add New. I will be adding new demo accounts called Ryu and Ken to simulate the real world again the names technically doesn't matter. After completeing the information for each User we will click " Add User ".

![Screenshot 2024-01-09 145114](https://github.com/kevonrochester/post-install-config/assets/155024615/45052347-e48c-425e-b975-cf74a634093c)
![Screenshot 2024-01-09 145303](https://github.com/kevonrochester/post-install-config/assets/155024615/59f96df1-ac3d-4246-abae-2fcb324b3bd5)
![Screenshot 2024-01-09 145535](https://github.com/kevonrochester/post-install-config/assets/155024615/e617d2c8-8ff8-4f95-ae00-8ff4df2243f9)

Then we will Create "SLA Plans" ( aka Service Level Agreement which is used to Provide the length of time in which the help desk Admin expects tickets to be Closed ). We will go to the Admin Panel > Click - Manage > SLA > Add New SLA PLAn. We will create SLA A , SLA B , SLA C ( again the names doesnt matter just the settings you choose to create ). Then we will click   "Add Plan "


![Screenshot 2024-01-09 150706](https://github.com/kevonrochester/post-install-config/assets/155024615/90aa3843-694a-45ab-a93a-052a7e62de8f)
![Screenshot 2024-01-09 150725](https://github.com/kevonrochester/post-install-config/assets/155024615/1cf5e01f-2c91-4682-afec-436f3acecf42)
![Screenshot 2024-01-09 155225](https://github.com/kevonrochester/post-install-config/assets/155024615/8874300d-5fce-4416-9be8-e8be007391db)


After that we will Create Help topics. Help topics will determine what Department the tickets is routed to and the priority of an ticket. Admin panel > click - Manage > Help Topics.
We will create Critical Outage , Personal Cpu Issues , Equipment Request , and password Reset but again the names doesn't matter you can make it whatever you want it to be. Click - Add New Help Topic > Add Topic ( when you completed your settings).


That completes this tutorial of the Post-Install Configuration in OsTicket

























