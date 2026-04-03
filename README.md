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
<br />

<p>
<img width="1172" height="810" alt="image" src="https://github.com/user-attachments/assets/9d700f39-d5e0-4edc-8fdf-91de2fb19656" />

</p>
<p>
3rd After logging into the VM, locate the osTicket installation files, unzip them, and begin the installation process.


</p>
<br />

<p>
<img width="1297" height="681" alt="image" src="https://github.com/user-attachments/assets/dba43260-3428-4070-a792-f603f9a295fb" />

</p>
<p>
4th Enable IIS by opening the Control Panel and selecting Turn Windows features on or off. Locate Internet Information Services (IIS), enable it, then navigate to:

World Wide Web Services → Application Development Features → CGI

Enable CGI and click OK to apply the changes.
</p>
<br />

<p>
<img width="1402" height="737" alt="image" src="https://github.com/user-attachments/assets/85f8ac58-4818-4570-bdaf-7619085cb6a0" />

</p>
<p>
5th Next, install PHP Manager for IIS by right-clicking the installer and selecting Install.


</p>
<br />

<p>
<img width="1267" height="638" alt="image" src="https://github.com/user-attachments/assets/4953d1d3-7da7-487e-a1f8-49fd20d7cd4c" />

</p>
<p>
6th Install the URL Rewrite Module and configure the environment as required.

</p>
<br />

<p>
<img width="980" height="640" alt="image" src="https://github.com/user-attachments/assets/d785ee96-5ef9-439d-bb02-041a63db2a4b" />

</p>
<p>
6th Create a new folder named PHP in the root of the C:\ drive.

</p>
<br />
<p>
<img width="1021" height="640" alt="image" src="https://github.com/user-attachments/assets/74bf965c-0654-46e2-a199-683707543fe1" />

</p>
<p>
7th Locate php-7.3.8-nts-Win32-VC15-x86.zip, extract it, and move its contents into the newly created C:\PHP directory.
</p>
<br />
<p>
<img width="1157" height="901" alt="image" src="https://github.com/user-attachments/assets/295501a8-b7e6-4c84-8f59-f9e6694ee210" />

</p>
<p>
8th Install VC_redist.x86.exe.

</p>
<br />


<p>
<img width="1382" height="782" alt="image" src="https://github.com/user-attachments/assets/f58160f5-4638-4ccd-938a-fbabb3d99507" />

</p>

<p>
9th When prompted for database credentials during setup, use root as both the username and password for this lab environment, then click Execute.</p>
<br />
<p>
<img width="1382" height="785" alt="image" src="https://github.com/user-attachments/assets/353f1b43-dde0-417e-8edb-e559a026bb38" />
<img width="625" height="472" alt="image" src="https://github.com/user-attachments/assets/b6107235-5e90-4906-b8a2-ebc15eaf9d5f" />

</p>

<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
<p>
<img width="1297" height="681" alt="image" src="https://github.com/user-attachments/assets/dba43260-3428-4070-a792-f603f9a295fb" />

</p>

<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
<p>
<img width="1297" height="681" alt="image" src="https://github.com/user-attachments/assets/dba43260-3428-4070-a792-f603f9a295fb" />

<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
<p>
<img width="1297" height="681" alt="image" src="https://github.com/user-attachments/assets/dba43260-3428-4070-a792-f603f9a295fb" />

<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
<p>
<img width="1297" height="681" alt="image" src="https://github.com/user-attachments/assets/dba43260-3428-4070-a792-f603f9a295fb" />

<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
<p>
<img width="1297" height="681" alt="image" src="https://github.com/user-attachments/assets/dba43260-3428-4070-a792-f603f9a295fb" />

<p>
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
</p>
<br />
<p>
<img width="1297" height="681" alt="image" src="https://github.com/user-attachments/assets/dba43260-3428-4070-a792-f603f9a295fb" />
