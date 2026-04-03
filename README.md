<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
Deployed and configured the osTicket open-source help desk system within a Microsoft Azure virtual machine environment. This project demonstrates hands-on experience with virtual infrastructure, Windows system configuration, IIS web services, PHP integration, and database connectivity.






<h2>Installation Steps</h2>

1st step , create a new Azure Virtual Machine. Name it something descriptive, such as osTicket-VM. Select Windows 10 Enterprise with 2 vCPUs, check the licensing confirmation box, and proceed with creating the VM.

<p>
<img width="1915" height="872" alt="image" src="https://github.com/user-attachments/assets/d978c2f5-a127-4843-a296-b48597baade7" />

</p>
<p>
2nd Once the VM deployment is complete, open the Remote Desktop application and connect using the VM’s public IP address.
</p>
<p>
<img width="1172" height="810" alt="image" src="https://github.com/user-attachments/assets/9d700f39-d5e0-4edc-8fdf-91de2fb19656" />

</p>
<p>
3rd After logging into the VM, locate the osTicket installation files, unzip them, and begin the installation process.


</p>

<p>
<img width="1297" height="681" alt="image" src="https://github.com/user-attachments/assets/dba43260-3428-4070-a792-f603f9a295fb" />

</p>
<p>
4th Enable IIS by opening the Control Panel and selecting Turn Windows features on or off. Locate Internet Information Services (IIS), enable it, then navigate to:

World Wide Web Services → Application Development Features → CGI

Enable CGI and click OK to apply the changes.
</p>

<p>
<img width="1402" height="737" alt="image" src="https://github.com/user-attachments/assets/85f8ac58-4818-4570-bdaf-7619085cb6a0" />

</p>
<p>
5th Next, install PHP Manager for IIS by right-clicking the installer and selecting Install.


</p>

<p>
<img width="1267" height="638" alt="image" src="https://github.com/user-attachments/assets/4953d1d3-7da7-487e-a1f8-49fd20d7cd4c" />

</p>
<p>
6th Install the URL Rewrite Module and configure the environment as required.

</p>
<p>
<img width="980" height="640" alt="image" src="https://github.com/user-attachments/assets/d785ee96-5ef9-439d-bb02-041a63db2a4b" />

</p>
<p>
7th Create a new folder named PHP in the root of the C:\ drive.

</p>
<p>
<img width="1021" height="640" alt="image" src="https://github.com/user-attachments/assets/74bf965c-0654-46e2-a199-683707543fe1" />

</p>
<p>
8th Locate php-7.3.8-nts-Win32-VC15-x86.zip, extract it, and move its contents into the newly created C:\PHP directory.
</p>
<p>
<img width="1157" height="901" alt="image" src="https://github.com/user-attachments/assets/295501a8-b7e6-4c84-8f59-f9e6694ee210" />

</p>
<p>
9th Install VC_redist.x86.exe.

</p>


<p>
<img width="1382" height="782" alt="image" src="https://github.com/user-attachments/assets/f58160f5-4638-4ccd-938a-fbabb3d99507" />

</p>

<p>
10th When prompted for database credentials during setup, use root as both the username and password for this lab environment, then click Execute.</p>
<p>
<img width="1382" height="785" alt="image" src="https://github.com/user-attachments/assets/353f1b43-dde0-417e-8edb-e559a026bb38" />
<img width="625" height="472" alt="image" src="https://github.com/user-attachments/assets/b6107235-5e90-4906-b8a2-ebc15eaf9d5f" />

</p>

<p>
11th Open IIS Manager as an administrator. Select osTicket, then open PHP Manager and register the php-cgi.exe file.

</p>
<p>
<img width="1418" height="721" alt="image" src="https://github.com/user-attachments/assets/fb15b8e9-476a-4bc5-980d-6845b0200d7e" />

</p>

<p>
12th Restart the IIS server to apply the changes.

</p>
<p>
<img width="1418" height="732" alt="image" src="https://github.com/user-attachments/assets/d005203c-7509-495b-bf1b-3e3cfe15e30a" />

<p>
13th Extract osTicket v1.15.8 and copy all contents into:

C:\inetpub\wwwroot

Rename the folder to osTicket.</p>
<p>
<img width="1077" height="726" alt="image" src="https://github.com/user-attachments/assets/569397be-e2ff-42b6-907b-e5f86edc7e48" />

<p>
14th In IIS Manager, navigate to:

Sites → Default Web Site → osTicket → Browse


</p>
<p>
<img width="1416" height="731" alt="image" src="https://github.com/user-attachments/assets/7248418f-5d6e-41f9-91e1-88dfa297bff7" />

<p>
15th Within PHP Manager, enable the required PHP extensions, restart the server, and verify they are enabled.

</p>
<p>
<img width="1263" height="675" alt="image" src="https://github.com/user-attachments/assets/6ff5a349-a44e-4709-a8ec-45c9bb2bf55e" />

<p>
16th Navigate to:

C:\inetpub\wwwroot\osTicket\include

Rename ost-sampleconfig.php to ost-config.php.

</p>
<p>
<img width="1018" height="633" alt="image" src="https://github.com/user-attachments/assets/9594641b-4f41-4696-9de4-c124998fb1f8" />
<p>
17th Right-click the file, open Properties → Security, disable inheritance, and remove all existing permissions.

Grant Everyone full control.</p>
<p>
<img width="706" height="451" alt="image" src="https://github.com/user-attachments/assets/b0eea705-d74f-45cd-9fdb-fb34998ef225" />

<p>
18th Continue the osTicket web-based setup by clicking Continue. Assign a help desk name and configure a default email address for ticket notifications.</p>
<p>
<img width="1238" height="747" alt="image" src="https://github.com/user-attachments/assets/9b7c7a8f-4fb9-465a-9600-cee0fd0471e0" />

<p>
19th Install HeidiSQL, open the application, and create a new session using root as the username and password.

</p>
<p>
<img width="853" height="598" alt="image" src="https://github.com/user-attachments/assets/aef1e673-d668-47fa-a231-113b02e7921f" />

<p>
20th Create a new database named osTicket.

</p>
<p>
<img width="1227" height="803" alt="image" src="https://github.com/user-attachments/assets/b9425ba1-2204-4c7c-8903-1fcc0b18e288" />

<p>
21 Select Continue to complete the installation.

</p>
<p>
<img width="1297" height="973" alt="image" src="https://github.com/user-attachments/assets/863b0de8-e729-4956-be30-9c5bcb116e99" />

<p>
22nd Congratulations! You have successfully installed osTicket. Additional configuration can be performed to assign user roles and permissions, but the core ticket creation and resolution system is now operational.

</p>
<p>
