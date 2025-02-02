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
This project requires a few different item or resources to be installed, we will install Internet Informatin Services (IIS) and enable CGI for this, intall PHP manager, and install a rewrite module to support the PHP applications. We will also unzip a file called PHP 7.3.8 and register it in IIS. Doing so will allow the web server to execute PHP scripts. In conclusion this step establishes the web server infrastructure needed to run osTicket efficiently
</p>
<br />

<h2>3. installing and configuring MySQL</h2>
<p>
<img src="https://i.imgur.com/fLxBTtS.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/eJvhCuk.png" height="50%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
I then installed a file called "MySQL 5.5.62" which is a database management system that will help store, manage, and retrieve structured data efficiently. I wil configure it with my selected credentials. I then installed a program called HeidiSQL which I can create a database for my tickets in osTicket. THis step is important because it provides my ticketing system with a structured data solution.
</p>
<br />

<h2>4. Deploying and Configuring osTicket</h2>
<p>
<img src="https://i.imgur.com/EAMunWc.png" height="70%" width="60%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/bIL6HtW.png" height="50%" width="40%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/byublq8.png" height="50%" width="40%" alt="Disk Sanitization Steps"/>
</p>
<p>
After the web server and database is set up and in place, it's finally time to deploy and set up osTicket, I make sure to enable essential extensions in PHP Manager for IIS. We can finally see soemthing show up on a website. I finish by configuring osTicket with my desired credentials and details. This step is critical since it integrates osTicket with the web server and makes sure everything functions correctly before finishing.
</p>
<br />

<h2>5. Finalizing Installation and set up</h2>
<p>
<img src="https://i.imgur.com/KkQ3Yh1.png" height="40%" width="50%" alt="Disk Sanitization Steps"/>
<img src="https://i.imgur.com/SIjnJ7c.png" height="60%" width="50%" alt="Disk Sanitization Steps"/><img src="https://i.imgur.com/fGO08sq.png" height="60%" width="50%" alt="Disk Sanitization Steps"/>
</p>
<p>
The installation is now complete and you have a login site for admins to login and configure the help desk and agents who can login and work tickets. In addition you have a site in order to create tickets for users. Beware, the help desk is very bare bones right now and lacking many things like departments, teams, SLAs and other things which will be handled in the next sections.
</p>
<br />
