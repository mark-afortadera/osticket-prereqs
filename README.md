<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Prerequisites and Installation</h1>
This project outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10 Pro</b> (21H2)

<h2>List of Prerequisites</h2>

- Create an Azure Virtual Machine Windows 10, 2 vCPUs
- Log into the VM with Remote Desktop
- Install / Enable IIS in Windows WITH CGI
- Install PHP Manager for IIS (PHPManagerForIIS_V1.5.0.msi)
- Install the Rewrite Module (rewrite_amd64_en-US.msi)
- Install VC_redist.x86.exe.
- Install MySQL 5.5.62 (mysql-5.5.62-win32.msi)
- Install osTicket v1.15.8

<h2>Installation Steps</h2>

![Screenshot 2025-02-12 175859](https://github.com/user-attachments/assets/9d62edf1-7903-43fc-92b6-eaa37c6f55ea)

![Screenshot 2025-02-12 180512](https://github.com/user-attachments/assets/cd9eb47f-560e-4531-a611-4ee31cf88080)

<p>
Create an osTicketing system using a virtual machine in Microsoft Azure Cloud based Platform.
</p>
<br />

![Screenshot 2025-02-12 180710](https://github.com/user-attachments/assets/2f64acb5-0d92-47a5-9d31-a979d183c6d0)

<p>
Open the virtual machine using Remote Desktop.
</p>
<br />

![Screenshot 2025-02-12 181034](https://github.com/user-attachments/assets/3089b0a2-c942-4859-866e-1c64c3ef59c9)

<p>
Download the osTicketing system file from the source then extract the files into the desktop.
</p>
<br />

![Screenshot 2025-02-12 183441](https://github.com/user-attachments/assets/54c6681e-8d7f-46bf-80a5-600958b532f3)

<p>
Install/ Enabled IIS in Windows WITH CGI
World Wide Web Services-> Application Development Features-> [X] CGI</p>
<br />

![Screenshot 2025-02-12 184154](https://github.com/user-attachments/assets/407942c7-2a85-4ee3-a07e-a242e17cddbe)

<p>
From the “osTicket-Installation-Files” folder, Install PHP Manager for IIS
 (PHPManagerForIIS_V1.5.0.msi)</p>
<br />

![Screenshot 2025-02-12 184247](https://github.com/user-attachments/assets/d43b963b-39ce-4d50-9479-5dc78deda72c)

<p>
From the “osTicket-Installation-Files” folder, Install the Rewrite Module
 (rewrite_amd64_en-US.msi)</p>
<br />

![Screenshot 2025-02-12 184458](https://github.com/user-attachments/assets/b718be95-db4f-4b06-9cc0-fc35c39eeae3)
![Screenshot 2025-02-12 184639](https://github.com/user-attachments/assets/8d18a845-f930-413d-a4a1-ce9ca3b2e28f)

<p>
Create the directory C:\PHP and from the “osTicket-Installation-Files” folder, unzip PHP 7.3.8
 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder</p>
<br />

![Screenshot 2025-02-12 184920](https://github.com/user-attachments/assets/4db0574a-22d2-4687-a0c4-aa2b188f7fbc)

<p>
From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe.</p>
<br />

![Screenshot 2025-02-12 185122](https://github.com/user-attachments/assets/2ecfae23-df05-4261-8aca-02b269bf31d2)
![Screenshot 2025-02-12 185301](https://github.com/user-attachments/assets/9d7a6a46-5528-41e6-b5c0-eb4a2daa2c11)
![Screenshot 2025-02-12 185424](https://github.com/user-attachments/assets/ee157f32-4497-4e19-a069-f7d05a2e544d)


<p>
 From the “osTicket-Installation-Files” folder, install MySQL 5.5.62
 (mysql-5.5.62-win32.msi)</p>
<p>-> Typical Setup</p>
<p>- Launch Configuration Wizard (after install)</p>
<p>- Standard Configuration</p>
<p>- Username: root</p>
<p>- Password: root</p>
<br />

![Screenshot 2025-02-12 194533](https://github.com/user-attachments/assets/30ff9614-f14a-4b8d-91d3-4b9f5f539fcf)

<p>Open IIS as an Admin</p>
<br />

![Screenshot 2025-02-12 194711](https://github.com/user-attachments/assets/8237f721-3b8f-4e2c-a081-6d4668f376a8)
![Screenshot 2025-02-12 194728](https://github.com/user-attachments/assets/687504a3-6762-40c2-be4f-7e8dc8f2f46e)
![Screenshot 2025-02-12 194815](https://github.com/user-attachments/assets/d8131bfc-4d7b-432e-a565-e11e6c340743)
![Screenshot 2025-02-12 194827](https://github.com/user-attachments/assets/07971246-8183-4421-b596-f738cfbf834d)

<p>Register PHP from within IIS (PHP Manager-> C:\PHP\php-cgi.exe)</p>
<br />

![Screenshot 2025-02-12 195016](https://github.com/user-attachments/assets/75ac7983-be30-4326-85a2-ed5c0dd64cd4)

<p>Reload IIS (Open IIS, Stop and Start the server)</p>
<br />

![Screenshot 2025-02-12 195205](https://github.com/user-attachments/assets/63b0746d-81f0-4cc6-bd9f-4380998efb50)
![Screenshot 2025-02-12 200828](https://github.com/user-attachments/assets/e03ea69e-6b92-4a10-9e90-793d7200e1ab)

<p>Install osTicket v1.15.8</p>
<p>- From the “osTicket-Installation-Files” folder, unzip “osTicket-v1.15.8.zip” and
 copy the “upload” folder into “c:\inetpub\wwwroot”</p>
<br />

![Screenshot 2025-02-12 200848](https://github.com/user-attachments/assets/b9765770-4096-42d0-8040-07347a30ac1f)

<p>Within “c:\inetpub\wwwroot”, Rename “upload” to “osTicket”</p>
<br />

![Screenshot 2025-02-12 202131](https://github.com/user-attachments/assets/86d81be3-c680-45db-aa2f-3d8f28c3c009)
![Screenshot 2025-02-12 202207](https://github.com/user-attachments/assets/099f7dbf-e1d4-4b81-a78b-10b362928593)

<p>Go to sites-> Default-> osTicket</p>
<p>- On the right, click “Browse *:80”</p>
<br />

![Screenshot 2025-02-12 204758](https://github.com/user-attachments/assets/94ec883c-b0fe-460b-a927-1aa104aefea5)
![Screenshot 2025-02-12 204850](https://github.com/user-attachments/assets/eb2691f0-0f9b-4759-b3e4-aa58b8afcce2)

<p>*Note that some extensions are not enabled</p>
<p>- Go back to IIS, sites-> Default-> osTicket</p>
<p>- Double-click PHP Manager</p>
<br />

![Screenshot 2025-02-12 204912](https://github.com/user-attachments/assets/8c511149-b9ef-4d86-9f62-b529357d2073)
![Screenshot 2025-02-12 205105](https://github.com/user-attachments/assets/656d6126-8ffd-40f4-970d-257b027324dd)

<p>Click “Enable or disable an extension</p>
<p>- Enable: php_imap.dll</p>
<p>- Enable: php_intl.dll</p>
<p>- Enable: php_opcache.dll</p>
<br />

![Screenshot 2025-02-12 205836](https://github.com/user-attachments/assets/169240a5-d4fa-492b-99c6-e3056f417b8f)

<p>Refresh the osTicket site in your browser, observe the changes</p>
<br />

![Screenshot 2025-02-12 210932](https://github.com/user-attachments/assets/a0f6d60e-70af-45c1-8362-9245eca9096a)
![Screenshot 2025-02-12 211052](https://github.com/user-attachments/assets/9fbc9df5-7fed-4203-98f7-16de8ef60dee)

<p>Rename: ost-config.php</p>

![Screenshot 2025-02-12 211146](https://github.com/user-attachments/assets/e3cf3d9d-f5bb-4994-9e9a-5462ad5b15e9)
![Screenshot 2025-02-12 211210](https://github.com/user-attachments/assets/09477d83-57a2-442b-a6eb-1a09b84b115b)
![Screenshot 2025-02-12 211243](https://github.com/user-attachments/assets/5417f081-7645-4deb-9341-95877276d31b)

<p>Assign Permissions: ost-config.php</p>
<p>- Disable inheritance-> Remove All</p>
<br />

![Screenshot 2025-02-12 211305](https://github.com/user-attachments/assets/be8733e1-b4a3-489f-af26-fd01f3eee51c)
![Screenshot 2025-02-12 212413](https://github.com/user-attachments/assets/02a6f725-23ee-4c95-bf68-83795dd18605)
![Screenshot 2025-02-12 212438](https://github.com/user-attachments/assets/498174d8-9bd6-4a46-9d5a-b2cbf6b9e06a)
![Screenshot 2025-02-12 212509](https://github.com/user-attachments/assets/f853c79d-7fde-4045-a2a2-5efc88672245)
![Screenshot 2025-02-12 212531](https://github.com/user-attachments/assets/bf917a49-a462-4ba9-b993-c391025e03af)

<p>New Permissions-> Everyone-> All</p>
<p>(*Note: for the sake of this example, I'll be assigning permissions to "everyone" on this demonstration)</p>
<br />

![Screenshot 2025-02-12 214451](https://github.com/user-attachments/assets/f5ff2e20-7e17-4e0e-8eda-2742f9ede9ce)

<p>From the “osTicket-Installation-Files” folder, install HeidiSQL.</p>
<br />

![Screenshot 2025-02-12 214605](https://github.com/user-attachments/assets/34f8b428-400d-4342-9a76-da10061e7709)
![Screenshot 2025-02-12 214652](https://github.com/user-attachments/assets/687cf079-e5fe-4b19-834b-dabeb1e31787)

<p>Open Heidi SQL</p>
<br />

![Screenshot 2025-02-12 214733](https://github.com/user-attachments/assets/09173de2-ea96-404a-9e03-9688892175f9)

<p>Create a new session, root/root</p>
<br />

![Screenshot 2025-02-12 214845](https://github.com/user-attachments/assets/3517acf8-7197-4ce9-b6e3-6fa07dedf9c4)

<p>Create a database called “osTicket”</p>
<br />

![Screenshot 2025-02-12 214923](https://github.com/user-attachments/assets/a62b2f9d-59ed-4e84-b38b-b7327a555f15)
![Screenshot 2025-02-12 214948](https://github.com/user-attachments/assets/043c058f-430a-4f73-a53f-200957fbbd4e)

<p>Connect to the session</p>
<br />

![Screenshot 2025-02-12 213945](https://github.com/user-attachments/assets/2db36a30-2cac-41ea-aa6a-d8a926a3a081)
![Screenshot 2025-02-12 214058](https://github.com/user-attachments/assets/82499e3c-cc2b-452a-8b8e-b2a85b80bad1)
<p>Continue Setting up osTicket in the browser</p>
<br />

![Screenshot 2025-02-12 220731](https://github.com/user-attachments/assets/ebd347d3-8373-4187-825d-c543e9a63fab)

<p>- MySQL Database: osTicket</p>
<p>- MySQL Username: root</p>
<p>- MySQL Password: root</p>
<p>- Click “Install Now!”</p>
<br />

![Screenshot 2025-02-12 221357](https://github.com/user-attachments/assets/9ca8550c-dfd1-44a2-991a-483a2892563d)

<p>osTicketing system installed!</p>
<br />

![Screenshot 2025-02-12 221728](https://github.com/user-attachments/assets/78b83e7b-c0ee-4952-a249-166030014f41)
![Screenshot 2025-02-12 221748](https://github.com/user-attachments/assets/5a036cd9-3103-43ee-ab32-b7a8ec630825)

<p>Browse to your help desk login page: http://localhost/osTicket/scp/login.php</p>
<br />

![Screenshot 2025-02-12 221958](https://github.com/user-attachments/assets/6369d5b4-9f3d-4adb-8f9d-a8449877fdfe)

<p>End Users osTicket URL: http://localhost/osTicket/</p>
<br />
