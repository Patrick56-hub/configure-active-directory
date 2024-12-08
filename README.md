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
On the Server Manager, I carried out the post-deployment configuration to promote the Server to a Domain Controller.
</p>
<br />
<br />
<p>

![image](https://github.com/user-attachments/assets/6ffce264-94a5-47ce-9f8f-65124a2892af)
</p>
<p>
Added a new Domain forest and finished setting up the domain controller.
</p>
<br />
<br />
<p>

![image](https://github.com/user-attachments/assets/87cd79a7-ae9f-4a3d-8b48-151f905eb5ba)
</p>
<p>
The machine automatically signed out and I reconnected to it using Remote desktop protocol, signed in using Fully Qualified Domain Name of 'kaelodomain.com\Twist DC'. 
</p>
<br />
<br />

<h4>Creating the accounts:</h4>
<p>

![image](https://github.com/user-attachments/assets/1ff7ffec-abb2-4daf-a5df-7707e8f197c2)

On the Server Manager, I created new departmental accounts;  Administrators, Employees and Clients accounts.
</p>
<br />
<br />
<p>

![image](https://github.com/user-attachments/assets/66f4c84a-a066-4224-a947-b9a9186b3be4)


Under the Administrator account, I created a new Administrative User account named 'Patrick Sekai' that has domain privileges.
</p>
<br />
<br />
<p>

![image](https://github.com/user-attachments/assets/ebf8f71f-b69b-4019-9a31-560eb1dab952)

Logged out of the domain controller and logged back in using the new administrative user account and a Fully Qualified Domain Name.
</p>
<br />
<br />
<p>
<h4>On the Client computer:</h4>
</p>
<p>

  ![image](https://github.com/user-attachments/assets/99075e2d-b283-4bed-af58-727de04d0782)

  Changed the device's DNS Server IP address to 10.0.0.4 which is the Domain Controller's private IP address.  

</p>
<br />
<br />
<p>
  
![image](https://github.com/user-attachments/assets/324e7b84-a4de-4299-bef1-3fc4d0c0469a)

 I logged in as a normal user on client's personal computer, added the device to the established domain forest.
</p>
