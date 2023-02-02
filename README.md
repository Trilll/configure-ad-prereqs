<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2022
- Windows 10 (21H2)

<h2>Deployment and Configuration Details</h2>

- Using Microsoft Azure; I deployed a Resource Group called AD-Lab within my main Azure Subscription. Within the resource group; I configured 2 virtual      networks. My first Virtual Network being DC-1 was a deployment of a Microsoft Server. The Second was called Client-1, and a deployment of a regular enterprise computer to act as working associates of a company. 


<h2>Deployment and Configuration Steps</h2>

<p>
<img src="https://imgur.com/BnNEt0G.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
After Configuring Azure Virtual Machines within the Resource Groups created; I have to change the DNS Server form Dynamic to Static.
</p>
<br />

<p>
<img src="https://imgur.com/FIyYcog.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
After changing the DNS Server from Dynmic to Static. I was able to connect the Client-1 Computer to the DC-1.
</p>
<br />

<p>
<img src="https://imgur.com/QFsgWz1.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
After downloading Active Directory onto the DC-1 Virtual Network; I was able to configure an Administrator account.
</p>
<br />

<p>
<img src="https://imgur.com/CfJC65F.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
Afer doing so, I utilized a powershell script in order to create 1000 users simulating a Business Enterprise enviornment.
</p>
<br />

<p>
<img src="https://imgur.com/yPEmc1R.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
After the users were created; I played around in the Active Directory administrator account. Fixing common problems within the infrastructure.
</p>
<br />

<p>
<img src="https://imgur.com/sDzXS3T.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
After the Active Directory server was created. I utilized password reset, account lock, and denying account access. 
</p>
<br />
