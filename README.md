<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Active Directory Deployment in the Cloud (Azure)</h1>
This tutorial outlines the implementation of On-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Install Active Directory
- Promote Server as a Domain Controller
- Creating Accounts

<h2>Deployment and Configuration Steps</h2>
<br />
<h4>Creating virtual machines:</h4>
<p>

![image](https://github.com/user-attachments/assets/e7f95924-4999-40f9-b19c-849c93678bee)
</p>
<p>
I configured the Windows Server and the Personal computer instance in the cloud environment.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/dcbe0717-0544-42ad-a905-9dfd255dd699)

</p>
<p>
Set the Windows Server virtual machine's private IP address to 'static'.
</p>
<br />

<p>

![image](https://github.com/user-attachments/assets/43cf5f87-4335-4f58-adde-f92f46a7a6f0)


</p>
<p>
Established a remote desktop connection to the Server virtual machine.
</p>
<br />
<h4>Installing Active Directory domain:</h4>
<p>

![image](https://github.com/user-attachments/assets/fde1ef55-3252-464d-aee7-c58cbffb2f61)

</p>
<p>
On the Server Manager, carried out a role-based installation.
</p>
<br />
<br />

![image](https://github.com/user-attachments/assets/051118ac-cb4e-466d-8ebc-751912588d94)

<p>
After selecting a server role of 'Active Directory Domain Services', I installed the application.
</p>
<br />
<br />
<p>
  <h4>Promoting the Server to a Domain Controller:</h4>
</p>
<p>

![image](https://github.com/user-attachments/assets/417ed81c-8219-49bc-9d72-7733989a3beb)
</p>
<p>
On the Server Manager, I carried out the post-deployment configuration of Active Directory Domain Controller.
</p>
<br />
<br />
