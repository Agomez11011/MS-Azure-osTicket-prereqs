<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>MS Azure + osTicket - Prerequisites and Installation</h1>
This tutorial outlines the prerequisites and installation of the open-source help desk ticketing system osTicket.<br />


<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>List of Prerequisites</h2>

- Computer + Internet
- Microsoft Azure (Microsoft Azure offers a free credits)
- Create Virtual Machine (Within Microsoft Azure)
- Downloading requirements for osTicket (Within the Virtual Machine)

<h2>Installation Steps</h2>

- <p> Our first step in the process after creating a free microsoft azure account is to click on "Virtual Machines"
<p>
<img src=https://github.com/user-attachments/assets/9ea62438-5965-4b93-9656-98d4f4f0537b
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />


- <p>Next we click on create, and select Azure Virtual Machine</p>

<p>
<img src=https://github.com/user-attachments/assets/b72463dc-c794-4e16-b043-852ffca67a5a
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />


- <p>From here we need to create a new resource group, click "Create New"</p>
- <p>You will get a pop-up to input a name. You can choose any name, I used "osTicket"</p>
- <p>On Virtual Machine Name give it any name, I chose "osTicket-vm"</p>
- <p>Region - I usually choose Canada Central as it allows me to pick a virtual machine with 2 vcpus / 8 GiB memory</p>
- <p>Image - select Windows 10 Pro Version 22h2</p>

<p>
<img src=https://github.com/user-attachments/assets/8d8992fe-f5a3-4a39-8597-c959545aebba
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />


- <p>As we scroll down we see <b>Size</b>, pick Standard_D2s_v3 as this will give us a VM with better performance</p>
- <p>Now set a username and password, make sure to write it down on a notepad so you don't forget</p>
- <p>Scroll to the end and check the box under Licensing</p>
- <p><B>Click "Review+Create"</B></p>

<p>
<img src=https://github.com/user-attachments/assets/ed9f54dc-1b0f-45e6-9236-dcd2d0cd1345
 height="80%" width="80%" alt="Disk Sanitization Steps"/>

  <img src=https://github.com/user-attachments/assets/3b34a17d-1b9b-4083-8f5e-afcfc370f159
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>It will take you to this screen, just click create again.</p>
- <p>Now wait until deployment is complete.</p>

<p>
<img src=https://github.com/user-attachments/assets/ed5b105b-58d7-4e2f-95d8-50b37d614e4a
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>After deployment completes, Go back to Virtual Machines and you will see your new VM up and running.</p>
- <p>On the right side you will see Public IP, copy it.</p>
- <p>Click the start button on the bottom of your screen and search for "Remote Desktop" and click on the remote desktop connection.</p>

<p>
<img src=https://github.com/user-attachments/assets/50eab50c-8ad5-4eb6-8694-9e7815fa84d0
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/80d22760-84a7-46cc-8be6-24f47c746a4d
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>With the public ip you just copied, paste it or type it into the text box and click connect</p>
- <p>A new box will appear, click more choices, use a different account and finally sign in with the credentials we made earlier that we saved on a notepad.</p>
- <p>Click OK</p>

<p>
<img src=https://github.com/user-attachments/assets/1080753d-ca36-4e7b-9bc5-dbc9e650f671
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/afb39e99-1c1f-447f-9914-7d7bf5b62742
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>A new box will open, click yes and your VM will open</p>
- <p>Now your VM will start the setup process, click no on everything and accept (this step does not really matter, I usually click no on everything anyways)</p>
- <p>And we have our VM open now!</p>

<p>
<img src=https://github.com/user-attachments/assets/b63d635a-5265-4091-b76e-1ffe7d2d2e31
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/c670ede1-5894-4bbb-8a93-dbd9e168c96a
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Open up microsoft edge and type in <b><i>osticket.com/download/</i></b> in the search bar</p>
- <p>Click on osTicket Core v1.18.1 or which ever is the latest</p>
- <p>Click next step</p>
- <p>Language - I will choose english and click on the small arrow to transfer the language over and click next</p>

<p>
<img src=https://github.com/user-attachments/assets/b249278e-82b8-4534-9797-3380e48c1705
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/69368052-555e-48c5-80e1-f3c8a2d87934
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Plugins - Don't worry about these, click next</p>
- <p>A mailing list pop-up will appear, click no thanks and osTicket will download onto your VM</p>

<p>
<img src=https://github.com/user-attachments/assets/5a6f23ae-4451-49d9-991e-1b6e8c39898c
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Now on the same page that we are on, we need to click on the "Visit Our Wiki" button because we still need to download the system requirements so osTicket can work on our machine.</p>
- <p>On the next page we click on the Installation link</p>
- <p>And we download the 4 recommended links</p>
- <p>For the last link (PHP Manager) we need to download it on github here --> https://github.com/phpmanager/phpmanager/releases</p>


<p>
<img src=https://github.com/user-attachments/assets/4f980281-45ea-4a9e-86a1-3e4524a1fd63
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/6393d2e4-f329-40ae-aae4-7b8f0c614e9e
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/06adfd61-037e-47eb-8137-bf12a540ae5b
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/059f9a75-48f2-447e-994d-a49e47b7f198
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/84954097-c6cc-4b2a-988b-d52f1825a295
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/167c279f-8f36-46e6-a5c7-1ca631d6a0f2
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/0629a2e5-1c9a-486c-a4ef-07f6887951a8
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>We also need to install a URL Rewrite module</p>
- <p>visit https://www.iis.net/downloads/microsoft/url-rewrite</p>
- <p>Download URL Rewrite Module 2.1 and install</p>

<p>
<img src=https://github.com/user-attachments/assets/83568f73-2e14-4520-bb84-ea51233dcc32
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Now lets install IIS</p>
- <p>Click the windows start menu and type in "Turn windows features on or off" and click on the program</p>
- <p>Find "Internet Information Services" and check the box</p>
- <p>Click the + to expand, expand "World Wide Web Services", expand "Application Development Features", check CGI and click OK</p>
- <p>Let it apply the changes</p>

<p>
<img src=https://github.com/user-attachments/assets/3c0d8339-f65d-4bbc-8934-05128c025844
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/cc64cca7-79f9-4ccf-a612-65e491dc64bf
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/f51075b8-4363-4fb6-95a2-60bcee5ea958
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>We can now install PHP manager, find your downloads folder and double click PHP Manager for IIS --> Hit next on everything</p>
- <p>Create a new folder in your (C:)Drive called "PHP"</p>
- <p>Go back to your downloads and extract php-8.3.13 into the PHP folder we made in the (C:)Drive</p>

<p>
<img src=https://github.com/user-attachments/assets/65ef1d94-0964-4161-9586-045a4bbd9d48
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/df2aaa69-b1d1-40bc-9b6e-68201852755b
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/acf8132e-f289-423f-aaf7-643944544277
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/7cfc9041-67df-48a8-8177-2b37ba652885
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Now we go back into our downloads folder and install MySQL, Server Only, click on the requirement and hit execute</p>
- <p>In Type and Networking click next, Authentication Method click next</p>
- <p>Accounts and Roles create a Root Password (IMPORTANT - DO NOT LOSE PASSWORD) click next</p>
- <p>Windows Service click next, Server File Permissions click next</p>
- <p>Apply Configuration --> Click Execute</p>

<p>
<img src=https://github.com/user-attachments/assets/190f31c7-fd6e-4088-a162-4494998b87f2
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/3fdac6b4-8a6b-49d2-ad09-94f0343a0af1
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/6f00228d-a974-48f4-a00a-ec83b44a0122
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/78663087-1fe7-430d-ba9e-0dc44acb458c
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/748d2ab6-1f0c-451d-869e-08ae2211217f
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/b521afc4-4b23-4a9f-80b0-809d5a0303ca
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/da4a00c8-dfad-4830-a4ce-f6c30497f6ae
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/de9adcb8-342a-4549-999a-d879e63968f5
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/d4b47473-3bb3-44f4-a40f-6213af1c9cf0
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Now lets click on the start menu and search IIS and run as administrator</p>
- <p>Double click PHP Manager and click Register new PHP Version</p>
- <p>Browse and find the PHP folder we made and click on php-cgi</p>
- <p>Then back in the IIS home page stop and start the server</p>

<p>
<img src=https://github.com/user-attachments/assets/b0744cbb-0cf7-4c7a-a42a-51c41e41be8e
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/5ed3d2af-d5e5-4955-9b1d-40f8959cef40
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/fce0b6dc-e914-4aa2-89b7-e036fdf8fe00
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/42c14703-3c8a-4eb7-a1dc-d90ad1de4ec6
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/71f8bc64-1366-4c00-8822-a9d1f4464eb6
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Now go back into the downloads folder and extract osTicket --> There should be another osTicket zip file, extract it.</p>
- <p>Open another file explorer and go into the (C:)Drive and find inetpub, double click inetpub</p>
- <p>Now in the osTicket folder you should see a folder called "Upload" copy it and paste into a folder called "wwwroot" that is found within inetpub</p>
- <p>Inside the wwwroot folder, Rename the upload folder --> osTicket</p>

<p>
<img src=https://github.com/user-attachments/assets/38a4240e-773b-4c09-88e7-6926aa187b52
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/aff641aa-7430-4cef-9524-bf81a0d29c20
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/0e875c90-bb3a-4019-be7a-77f43ff08c16
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/c76e20cb-889d-49cd-bb49-2de32aed32ad
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/fbb88580-0a48-4cc7-b273-a4c8aaa52d41
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/9ebd2d2e-9c84-4b80-9b2a-905c170a8851
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>We are now going to open IIS as admin, stop and start the server</p>
- <p>On the left side click the drop downs until you see osTicket, click osTicket and then double click PHP Manager</p>
- <p>Click "Enable or disable an extension</p>
- <p>Enable these 3 extensions: php_imap.dll, php_intl.dll, php_opcache.dll</p>

<p>
<img src=https://github.com/user-attachments/assets/d5a81712-738d-4eed-a807-eed1876ad336
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/bc3335f3-0223-4454-ba0a-2900face3949
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Open up file explorer and once again locate the osTicket folder and open it</p>
- <p>Inside the osTicket folder open up a folder called "Include"</p>
- <p>Find a file called "ost-sampleconfig.php" and rename it to "ost-config.php"</p>

<p>
<img src=https://github.com/user-attachments/assets/08a8cb3f-b587-49dd-bc87-4d0a1ba1687c
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/94b3a51e-11a5-4a70-991e-332ad7e6df1f
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/139e703e-fd21-448e-b3e1-bfb9429ba057
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Go to downloads and install MariaDB</p>
- <p>Click next on everything until you reach where it says to enter root password, put the same root password you created earlier</p>
- <p>Continue hitting next and finish install</p>
- <p>You should now have HeidiSQL automatically installed on your desktop</p>

<p>
<img src=https://github.com/user-attachments/assets/202c96a4-07c2-4405-8441-427229f09567
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/5540d88d-f32e-4134-89a5-e8df67c3fb51
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/4a434a6e-80e8-430b-a402-6daf309b8f36
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Open HeidiSQL</p>
- <p>Click "New" type in your root username and password (NOTE: if your username does not work type in "root"), click open</p>
- <p>Right click on "Unnamed" and click create new and then database</p>
- <p>Name it exactly "osTicket"</p>
- <p>Open windows powershell as administrator</p>
- <p>Change directory by putting in this command line and press enter --> cd C:\inetpub\wwwroot\osTicket</p>
- <p>Then paste or type in and press enter --> icacls include\ost-config.php /grant 'Everyone:F'</p>

<p>
<img src=https://github.com/user-attachments/assets/d7bfd96b-c94e-49b1-bbed-0dbeca42ff57
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/7a995e10-e541-421d-94d1-d658797834b0
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/36cc1acd-fa2a-4bc7-abb2-219d1e9e2cc2
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/a85a8269-aea8-42c4-ac16-af0a62ac66d4
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<br />

- <p>Now from here open up IIS and restart the server by clicking "Restart" on the right side of the screen</p>
- <p>Go into osTicket in the drop downs and click on browse</p>
- <p>osTicket will open and click continue</p>
- <p>Set up all your information - refer to the pictures below (SQL Database must be named osTicket)</p>
- <p>Click Install Now</p>
- <p>Congratulations, osTicket is now installed</p>
- <p>Click on the staff link and sign in with your admin credentials</p>
- <p><b>DONE</b></p>

<p>
<img src=https://github.com/user-attachments/assets/5d46615d-02a4-43b0-8a2c-c57c0bef2b36
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/0c63e1da-a475-40e3-8282-17895c55d23c
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/1c489302-b72b-42f6-9909-5acdb9e2d461
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/a6f86b61-c44d-48ac-a80b-62d9f2c6056a
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/2310870d-a657-4d59-9436-ad066e27d14b
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src=https://github.com/user-attachments/assets/9d6961ac-20da-4ddd-97b1-d0c16e4b6a2f
 height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
