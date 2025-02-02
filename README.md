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

<h2>Installation Steps</h2>
<h2>1. Creating a virtual machine in order to create project</h2>
<p>
<img src="https://i.imgur.com/cfeDIxl.png" height="70%" width="70%" alt="Disk Sanitization Steps"/>
</p>
<p>
You will need a microsoft azure subscription to create this project there is a pay as you go option or a free trial for $200 credit, after you make this subscription we will need a resource group that will house the vnet that then houses our virtual machine.
  
To begin the osTicket deployment, we first set up a Windows 10 virtual machine (VM) in Microsoft Azure. This VM serves as the foundation for hosting the ticketing system. We configure it with 4 vCPUs to ensure adequate performance but 2 vCPUs will do the trick. The machine is going to be named osticket-vm. In the creation of the vm you will create a new resource group when prompted and vnet, for the "image section we will use windows 10 pro, and we will create a username and password to access the machine (Username: labuser, Password: Password123). Once provisioning is complete, we use Remote Desktop Protocol (RDP) to log into the VM if you are using windows, preparing it for software installations and further configurations.
</p>
<br />

<h2>2. Setting up IIS and Required Components</h2>
<p>
<img src="https://i.imgur.com/YxHR2F8.png" height="40%" width="50%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/UcHxM03.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
This project requires a few different item or resources to be installed, we will install Internet Informatin Services (IIS) and enable CGI for this, intall PHP manager, and install a rewrite module to support the PHP applications. We will also unzip a file called PHP 7.3.8 and register it in IIS. Doing so will allow the web server to execute PHP scripts
</p>
<br />

<h2>3. Creating a virtual machine in order to create project</h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<h2>4. Creating a virtual machine in order to create project</h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />

<h2>5. Creating a virtual machine in order to create project</h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
