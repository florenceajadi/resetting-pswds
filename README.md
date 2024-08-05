<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Resetting User Pswds In Active Directory Users and Computers</h1>
This tutorial outlines the implementation of resetting user pswds and creating groups in Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Reset Users Pswd and Create Groups](https://youtu.be/cG7M3Z-Cek4)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- 

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Run search through active directory
- Search user
- Verify username/account
- Reset user's Pswd
- Login to user to verify the pswd works
- Creating groups
- Adding members to groups
- Enabling/Disabling members


<h2>Deployment and Configuration Steps</h2>

<p>
<img src="" height="80%" width="80%""/>


</p>
<p>
Diagram
</p>
<br />

<p>
<img src="https://github.com/user-attachments/assets/896fdf09-7071-4495-9209-fb092ec48b9c" height="80%" width="80%""/>


</p>
<p>
Running search through active directory to reset pswd for user Jeremy Collins
</p>
<br />

<p>
  <img src="https://github.com/user-attachments/assets/2008b544-97dc-47b9-8c50-640851add1ee" height="80%" width="80%" />
  <img src="https://github.com/user-attachments/assets/eb65f762-695c-4d75-99c5-c773a996b3ad" height="80%" width="80%""/>




</p>
<p>
We can verify that the pswd for Jeremy Collins has been changed. So when Jeremy Collins logs in with the password, he is able to create his own password next time he logs in.
</p>
<br />

<p>
  <img src="https://github.com/user-attachments/assets/91875093-c5dc-43f0-a76f-24a2c56dcef7" height="80%" width="80%""/>
  <img src="https://github.com/user-attachments/assets/7459abb2-950f-4851-a7ab-35330861ef6f" height="80%" width="80%""/>
</p>

<p>
  Creating a new group called Sales within CyberGirl OUs. I assigned this new group to be in Global so it can be used for assigning permissions within the domain and can be a member of groups in any domain within the forest.
  It is placed in Security which enables the group to be used for assigning permissions to resources like files, folders, and printers. We now have a new group called Sales that is located in the Domain Users of CyberGirl (OUs).
</p>
<br />


<p>
<img src="https://github.com/user-attachments/assets/935d5db6-c1e7-45a7-8a02-3cc11d440aa5" height=80%" width="80%""/>  

</p>

  
<p>
We want to add a new member to the Sales group, so we are adding user Jeremy Collins. </p>
<p>
    <img src="https://github.com/user-attachments/assets/017426ad-f9cb-459d-a7a7-df8efbca3449" height="80%" width="80%""/>
  <img src="https://github.com/user-attachments/assets/7660c494-05c8-493d-af84-4f33c21352a3" height="80%" width="80%" />
</p>

<p>
    Jeremy Collins is now added to the Sales group. We can even look into Jeremy Collins' account to see who is a member of. 

</p>

<br />

<p>
  <img src="https://github.com/user-attachments/assets/02df2e26-989c-40b0-8df6-6ffe9d761c57" height="80%" width="80%""/>
  <img src="https://github.com/user-attachments/assets/7ebabd73-6e05-4931-a620-aeccec7df5af" height="80%" width=80%""/>
  
  
</p>
<p>
  Creating a new Organizational Unit called DISABLED USERS within CYBERGIRL and disabled user Jeremy Collins.
  
</p>
<br />

<p>
  <img src="https://github.com/user-attachments/assets/8778348e-9ef4-47af-b3fb-531d80fde6c6" height="80%" width="80%""/>
  <img src="https://github.com/user-attachments/assets/6da7b926-0155-4592-a1e2-9abb886e6886" height="80%" width="80%""/>


</p>
<p>
  <img src="https://github.com/user-attachments/assets/c2c25506-56f8-481c-829c-7252110f956e" height="80%" width="80%" />
<p>
  I tried logging into Jeremy.Collins account but was unable to do so due to account being disabled.
</p>
<br />
