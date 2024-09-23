<h1>Active Directory Lab</h1>


<h2>Project Overview</h2>
The goal of this project is to create a full Active Directory lab environment on a personal computer using VirtualBox. This setup helps users gain hands-on experience with Windows networking, Active Directory, DHCP, and PowerShell automation. It involves configuring a domain controller, creating multiple user accounts, and connecting a Windows 10 client to the domain, simulating a basic enterprise network environment for learning and practice.

<p align="center">
<img src=https://i.imgur.com/wZbcgiC.png"" height="80%" width="80%" alt=""/> <br/>


<h2>Languages and Utilities Used</h2>

- <b>Active Directory</b> 
- <b>PowerShell</b>
- <b>Windows Server</b> 
- <b>Virtualization (Oracle VirtualBox)</b>

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)

<h2>Program walk-through:</h2>

<p align="center">

<!--
1. Download and Install Oracle VirtualBox
 VirtualBox will be used to run the virtual machines.
2. Download Windows 10 ISO and Server 2019 ISO
 These ISO files will be used to install two separate operating systems on the virtual machines.
3. Create a Virtual Machine for the Domain Controller
 Set up the first virtual machine to house Active Directory.
  Configure two network adapters:
   a. One for connecting to the outside internet.
   b. One for connecting to the VirtualBox private network for the clients.
4. Install Server 2019 on the Virtual Machine
 Assign IP addressing for the internal network. The external network will get an IP address from your home router automatically.
5. Name the Server and Install Active Directory
 Create a domain and configure routing to allow clients on the private network to access the internet through the domain controller.
6. Set Up DHCP on the Domain Controller
 This will allow the Windows 10 machine to automatically obtain an IP address.
7. Run a PowerShell Script to Create 1,000 Active Directory Users
8. Create a Virtual Machine for the Windows 10 Client
 Install Windows 10 on this machine.
 Connect the client virtual machine to the private VirtualBox network.
9. Name the Client Machine and Join It to the Domain
 Log into the client machine using one of the domain accounts created earlier.
10. Complete the Lab Setup
 This setup creates a basic Windows networking environment with Active Directory and a few essential networking services.
 --!>
<br />
<br />
Users Name List to input in PowerShell: <br/>
<img src="https://i.imgur.com/C79ylHN.png" height="80%" width="80%" alt=""/>
<br />
<br />
Inputing user list into PowerShell script:  <br/>
<img src="https://i.imgur.com/1nXLyo7.png" height="80%" width="80%" alt=""/>
<br />
<br />
Can now find users after running script:  <br/>
<img src="https://i.imgur.com/7NjkmL7.png" height="80%" width="80%" alt=""/>
<br />
<br />


 
<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
