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


- <p>As we scroll down we see <b>Size<b/>, pick Standard_D2s_v3 as this will give us a VM with better performance</p>
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


