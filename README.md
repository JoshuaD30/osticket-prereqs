<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Video Demonstration</h2>

- ### [YouTube: How To Install osTicket with Prerequisites](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- install/Enable IIS
- PHP manager for IIS
- rewrite module 
- mircosoft C++
- my SQL

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/WTFuH6w.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
after you install IIS PHP MANAGER and rewrite module and  VC_redist.x86.exe.
create the directory C:\PHP
</p>
<br />

<p>
<img src="https://i.imgur.com/R0jB3zr.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
.download MySQL typical setup>Launch Configuration Wizard (after install)Standard Configuration -> then open IIS as admin
Register PHP from within IIS Reload IIS (Open IIS, Stop and Start the server)


</p>
<br />

<p>
<img src="https://i.imgur.com/HMwCb5q.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install osTicket v1.15.8 Extract and copy “upload” folder to c:\inetpub\wwwroot Within c:\inetpub\wwwroot, Rename “upload” to “osTicket” Reload IIS (Open IIS, Stop and Start the server) Go to sites -> Default -> osTicket On the right, click “Browse *:80”

<img src="https://i.imgur.com/gh4XR3g.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

</p>Go back to IIS, sites -> Default -> osTicket Double-click PHP Manager Click “Enable or disable an extension Enable: php_imap.dll Enable: php_intl.dll Enable: php_opcache.dll Refresh the osTicket site in your browse, observe the changes
Rename: ost-config.php From: C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php
To: C:\inetpub\wwwroot\osTicket\include\ost-config.php Assign Permissions: ost-config.php
Disable inheritance -> Remove All
New Permissions -> Everyone -> All


Continue Setting up osTicket in the browser (click Continue)
Name Helpdesk
Default email (receives email from customers)

 download and install HeidiSQL.
Open Heidi SQL
Create a new session, root/Password1
Connect to the session
Create a database called “osTicket”
Continue Setting up osticket in the browser MySQL Database: osTicket MySQL Username: root  MySQL Password: Password1 Click “Install Now!”


<img src="https://i.imgur.com/najC7oT.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>

Congratulations, hopefully it is installed with no errors!





<br />
