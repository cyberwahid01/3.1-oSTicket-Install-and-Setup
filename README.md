<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>Ticketing Systems: osTicket Install and Setup 🪟</h1>
This section outlines the process of installing osTicket within a Microsoft Azure Virtual Machine, and setting up the necessary files and folders for osTicket to function correctly. 

(Link Back to Main Project Contents Page is at the Bottom of this Repo)
<h2>Environments and Technologies Used</h2>

- Lenovo Ideapad 5 Pro 16gb AMD Ryzen 7
- Microsoft Azure Resource Group
- Microsoft Azure Windows 10 Pro version 22H2 - x64 Gen2 Virtual Machine
- osTicket Software and File Dependencies

<h2>Operating Systems Used </h2>

- Local Windows 11 Home Version 21H2</b>
- Windows 10 Pro version 22H2 Virtual Machine
  
<h2>List of Prerequisites</h2>

- Microsoft Azure Subscription
- Microsoft Azure Subscription Credit 

<h2>Installation, Setup, Resource Setup, Executing Functions</h2>

1. Having created our Windows 10 Virtual Machine within Microsoft Azure, I proceeded to enable IIS (Internet Information Services), then turned on the CGI (Common Gateway Interface) feature within IIS. Enabling the CGI feature allows us to run scripts and external programmes on our website that will use osTicket. In our case one of those languages will be PHP. CGI can be enabled by accessing Windows Features via control panel, then into IIS, then WWWS (World Wide Web Services), then Application Development Features, then enabling CGI.

<p>
<img src="https://imgur.com/MD1TrW1.png" alt="Disk Sanitization Steps"/>
</p>
<p>
2. At this stage I have installed a PHP Manager, Rewrite Module, Created a folder within our C: Drive named PHP, Unzipped PHP Extensions into this PHP folder. I then opened IIS as an Admin and registered PHP from within IIS. After this I installed osTicket and configured the "upload" folder into c:\inetpub\wwwroot. The reason for this is that we will have 2 domains for our osTicket installation. One will be for our Admin Panel and one for our User Panel. I then enabled some PHP extensions, namely php_imap.dll, php_intl.dll and php_opcache.dll.
</p>
<br />

<p>
<img src="https://imgur.com/V9eSscS.png" alt="Disk Sanitization Steps"/>
</p>
<p>
3. At this stage in the installation process we are choosing the name for our Helpdesk URL, Email and Setting our Primary Admin User Account.
</p>
<br />

<p>
<img src="https://imgur.com/59y8lwX.png" alt="Disk Sanitization Steps"/>
</p>
<p>
4. I then installed HeidiSQL, created a session, connected to the session and created a database for osTicket. Within MySQL, which we installed earlier, chose the database osTicket, with the same password and username as created in HeidiSQL, and then installed osTicket.
</p>
<br />

<p>
<img src="https://imgur.com/1SeLwqg.png" alt="Disk Sanitization Steps"/>
</p>
<p>
5. Below we can see the successful installation of osTicket.
</p>
<br />

<p>
<img src="https://imgur.com/uZAaXMt.png" alt="Disk Sanitization Steps"/>
</p>
<p>
6. Below we can see the osTicket Admin Panel login page with the Helpdesk name "CyberWahidHelpDesk".
</p>
<br />

<p>
<img src="https://imgur.com/Orjdzta.png" alt="Disk Sanitization Steps"/>
</p>
<p>
7. Having successfully logged into osTicket, we can see the layout of our Admin panel.
</p>
<br />

<p>
<img src="https://imgur.com/Ark3COu.png" alt="Disk Sanitization Steps"/>
</p>
<p>
8. Below we can see our User Panel Support Center.
</p>
<br />

<p>
<img src="https://imgur.com/qoD7Gof.png" alt="Disk Sanitization Steps"/>
</p>
<p>
LINK BACK TO THE MAIN PROJECT CONTENTS PAGE - https://github.com/cyberwahid01/Azure-Compute-and-Networking
