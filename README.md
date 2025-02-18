<p align="center">
<img src="https://i.imgur.com/pU5A58S.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>On-premises Active Directory Deployed in the Cloud (Azure)</h1>
This tutorial outlines the implementation of on-premises Active Directory within Azure Virtual Machines.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How to Deploy on-premises Active Directory within Azure Compute](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Active Directory Domain Services
- PowerShell

<h2>Operating Systems Used </h2>

- Windows Server 2025
- Windows 11 (21H2)

<h2>High-Level Deployment and Configuration Steps</h2>

- Create a Resource Group
- Create a Windows 10 Virtual Machine (VM)
  - While creating the VM, select the previously created Resource Group
  - While creating the VM, allow it to create a new Virtual Network (Vnet) and Subnet
- Create a Linux (Ubuntu) VM
  - While creating the VM, select the previously created Resource Group and Virtual Network—the Virtual Network MUST BE THE SAME.
  - Authentication type: Username/Password
- Ensure both VMs are in the same Virtual Network / Subnet
- End the lab

<h2>Deployment and Configuration Steps</h2>

<p>
<img width="953" alt="Microsoft Azure VM Creation Screen Shot" src="https://github.com/user-attachments/assets/e9fffd4a-a531-4ef9-8295-dc6df71c328c" />

</p>
<p>
This screenshot shows a Windows and a Linux virtual machine (VM) successfully created in Microsoft Azure. Both VMs are now deployed and ready for use
</p>
<br />

<p>
<img width="757" alt="Screenshot RDP traffic capture in wireshark" src="https://github.com/user-attachments/assets/588c8d01-2216-42e0-b4b4-bbbe69987d34" />

</p>
<p>
This screenshot shows RDP (Remote Desktop Protocol) traffic being observed in Wireshark. You can see captured network packets that display the communication between a remote client and the Windows VM.
</p>
<br />

<p>
<img width="925" alt="Screenshot nslookup disney com DNS" src="https://github.com/user-attachments/assets/c97b85e6-0c6a-4241-a6b0-1cc9692c1b19" />

</p>
<p>
This screenshot shows the use of nslookup for disney.com while monitoring DNS traffic in Wireshark. You can see the DNS query being sent and the corresponding response resolving the domain to an IP address.
</p>
<br />
