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

- Windows 10 Enterprise</b> (22H2)

<h2>List of Prerequisites</h2>

- Set up a virtual machine (VM) in Microsoft Azure
- Download [OsTicket Installation Files](https://drive.google.com/uc?export=download&id=1b3RBkXTLNGXbibeMuAynkfzdBC1NnqaD)
   

<h2>Installation Steps</h2>

<p>
Log into Microsoft Azure and create a VM. Feel free to use any username/password at your own discrestion.
</p>
<p>
<img <img width="957" height="678" alt="Screenshot 2026-08-13 131200" src="https://github.com/user-attachments/assets/44f38f1c-7212-4f6b-ab1e-f66f09e3272a" />
</p>
<p>
<img <img width="1082" height="767" alt="Screenshot 2026-08-13 131444" src="https://github.com/user-attachments/assets/235d8ee6-993b-45aa-8c0a-75c696c5ceec"/>
</p>
<p>
<img <img width="995" height="572" alt="Screenshot 2026-08-13 131507" src="https://github.com/user-attachments/assets/00b96fbc-1f3b-42ad-a1af-294c9a46d36c" />
</p>
<p>
<img <img width="1067" height="468" alt="Screenshot 2026-08-14 194901" src="https://github.com/user-attachments/assets/2de6843d-7afe-4eb2-bbc1-b53399c98719" />
</p>


<br />

<p>
Copy the public IP address for the VM, then log into the VM using the username and password created in the initial setup.
<p>
<img <img width="1310" height="397" alt="Screenshot 2026-08-13 133226" src="https://github.com/user-attachments/assets/4407b6df-ba7d-4700-88ee-0c9e35e11976"/>
</p>
<p>
<img <img width="543" height="302" alt="Screenshot 2026-08-13 133548" src="https://github.com/user-attachments/assets/bfcf3ecf-b119-4093-a393-3076091698c9"/>
</p>
<p>
<img <img width="560" height="415" alt="Screenshot 2026-08-13 133935" src="https://github.com/user-attachments/assets/71d82f91-9bc3-4780-8fcb-9b7eff9eb2cb"/>
</p>

<br />

<p>
Once logged into the VM, download the osTicket installation zip file (linked above in the Prerequisites) and unzip it to the desktop. Leave the file name defaulted to "osTicket-Installation-Files".
<p>
<img <img width="1917" height="507" alt="Annotation 2026-08-14 221436" src="https://github.com/user-attachments/assets/3d56a250-689d-4cbd-8aa2-a69957d2f614"/>
</p>

<p>
Open Control Panel, Programs -> Programs and Features -> then Turn Windows features on or off.
</p>
<p>
<img <img width="1402" height="586" alt="Screenshot 2026-08-13 205557" src="https://github.com/user-attachments/assets/a4ed9519-1b32-4bca-9a57-4be813fb503d"/>
<p>
Select Internet Information Services and expand the folder -> expand World Wide Web Services -> expand Application Development Features -> select CGI.
</p>
<p>
<img <img width="552" height="490" alt="Screenshot 2026-08-13 205739" src="https://github.com/user-attachments/assets/8ff6673f-5862-4fa5-96c3-2807af4728e9" />
</p>

<p>
Within the osTicket-Installation-Files folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0).
</p>
<p>
<img <img width="1060" height="468" alt="Screenshot 2026-08-13 205907" src="https://github.com/user-attachments/assets/04f6f154-844d-498a-9d3d-c38cdbfebbee"/>
</p>
<p>
Within the osTicket-Installation-Files folder, install Rewrite Module (rewrite_amd64_en-US).
</p>
<p>
<img <img width="1137" height="493" alt="Screenshot 2026-08-13 210011" src="https://github.com/user-attachments/assets/851a2ba8-b90f-4b62-b8be-420fc7892944" />
</p>

<p>
Navigate to the C drive and create a new folder, PHP. 
</p>
<p>
<img <img width="1020" height="466" alt="Screenshot 2026-08-13 210137" src="https://github.com/user-attachments/assets/e1435724-aa57-4b0a-ba56-d8cf4071845f"/>
</p>
<p>
Within the osTicket-Installation-Files folder, right-click PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and extract all to C:\PHP.
</p>
<p>
<img <img width="1257" height="706" alt="Screenshot 2026-08-13 210329" src="https://github.com/user-attachments/assets/1d5312f0-1bfc-49e4-9c8f-81d105863693"/>
</p>
<p>
<img <img width="697" height="585" alt="Screenshot 2026-08-13 210430" src="https://github.com/user-attachments/assets/cb0e6421-deba-48e6-82fd-51163c7f402d" />
</p>
<p>
Within the osTicket-Installation-Files folder, install VC_redist.x86 
</p>
<p>
<img <img width="1097" height="465" alt="Screenshot 2026-08-13 210552" src="https://github.com/user-attachments/assets/3d9fa461-01a9-4e5d-b180-7a48e8185ebd"/>
</p>

<p>
Within the osTicket-Installation-Files folder, install MySQL 5.5.62 (mysql-5.5.62-win32). Select Typical Setup -> on the next screen ensure to select Launch Configuration Wizard -> then Finish
</p>
<p>
<img <img width="1141" height="482" alt="Screenshot 2026-08-13 210657" src="https://github.com/user-attachments/assets/7489ad0b-bb8a-4c6a-9d69-f41eba0cf0cc"/>
</p>
<p>
<img <img width="612" height="475" alt="Screenshot 2026-08-13 210745" src="https://github.com/user-attachments/assets/b4675efc-20eb-499b-a481-2bace432ecbd"/>
</p>
<p>
<img <img width="612" height="477" alt="Screenshot 2026-08-13 210842" src="https://github.com/user-attachments/assets/79f0c154-ee3b-4870-be09-3b81ce5c1724"/>
</p>
<p>
Within the Configuration Wizard, select Standard Configuration.
</p>
<p>
<img <img width="618" height="471" alt="Screenshot 2026-08-13 210941" src="https://github.com/user-attachments/assets/eb86598c-18a5-4131-87f1-622d09a0c1f7"/>
</p>
<p>
Next you will create a new root password. MAKE SURE YOU KEEP A RECORD OF THIS FOR LATER! Then Execute.
</p>
<p>
<img <img width="617" height="472" alt="Screenshot 2026-08-13 211057" src="https://github.com/user-attachments/assets/2ab98108-3417-46d8-80ce-bad5834203d6"/>
</p>
<p>
<img <img width="617" height="467" alt="Annotation 2026-08-14 222441" src="https://github.com/user-attachments/assets/0a62cbce-38a4-466d-a1ca-dc098d203145" />
</p>

<p>
Open Internet Information Services Manager (IIS) as an Admin.
</p>
<p>
<img <img width="975" height="842" alt="Annotation 2026-08-14 222628" src="https://github.com/user-attachments/assets/6801b886-0c5e-4806-9f28-db03c23184ec"/>
</p>
<p>
Within IIS, select PHP Manager and register new PHP version. Click the box with three dots to browse files and select "php-cgi" within C:\PHP
</p>
<p>
<img <img width="1920" height="837" alt="Annotation 2026-08-14 222742" src="https://github.com/user-attachments/assets/e78aa2c8-1d3a-467a-ae97-678d5a3a31d1"/>
</p>
<p>
<img <img width="1038" height="800" alt="Annotation 2026-08-14 222839" src="https://github.com/user-attachments/assets/d5c8865f-55d3-4a8c-b1f7-8ffbf763eefd"/>
</p>
<p>
<img <img width="627" height="262" alt="Annotation 2026-08-14 223033" src="https://github.com/user-attachments/assets/7dad87d8-137a-4200-b75b-74e5e2034756"/>
</p>
<p>
<img <img width="932" height="582" alt="Annotation 2026-08-14 222947" src="https://github.com/user-attachments/assets/b28d1c4e-2a55-4ffa-bcbd-0ed12ecc7226"/>
</p>
<p>
<img <img width="627" height="275" alt="Annotation 2026-08-14 223122" src="https://github.com/user-attachments/assets/d7a96180-e13c-4fb1-9fb5-f556089941ac"/>
</p>

<p>
Return to the IIS Manager and Reload IIS. To the right under Manage Server you click restart or stop -> start.
</p>
<p>
<img <img width="1918" height="822" alt="Annotation 2026-08-14 223225" src="https://github.com/user-attachments/assets/f90a809a-7015-4cf6-88db-6fb5d0534a17"/>
</p>

<p>
To the left under Connections, navigate to Sites -> Default Web Site -> osTicket. Then to the right, under Browse Folder select "Browse*:80".
</p>
<p>
<img <img width="1917" height="657" alt="Annotation 2026-08-14 224530" src="https://github.com/user-attachments/assets/a9cb40e3-081e-40de-afe2-64280e951484"/>
</p>
<p>
<img <img width="1915" height="1027" alt="Annotation 2026-08-14 224806" src="https://github.com/user-attachments/assets/e423dd37-9792-43c2-b7dc-faec73c3db76"/>
</p>

<p>
You will notice there are a few recommended extensions that are disabled. Return to IIS -> Sites -> Default Web Site -> osTicket. Open PHP Manager. Select enable or disable an extension.
</p>
<p>
<img <img width="1195" height="910" alt="Annotation 2026-08-14 225051" src="https://github.com/user-attachments/assets/b2b42bbc-ea9c-4af9-b6e8-4e654a68e3f6"/>
</p>
<p>
Select php_imap.dll from the disabled list. Then on the top right select Enable. Repeat this process for php_intl.dll and php_opcahe.dll.
</p>
<p>
<img <img width="1918" height="973" alt="Annotation 2026-08-14 225227" src="https://github.com/user-attachments/assets/5dd2d1a2-e2c5-4c9f-8dea-351a90c6a0ae"/>
</p>
<br />
