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
<img width="957" height="678" alt="Screenshot 2026-08-13 131200" src="https://github.com/user-attachments/assets/44f38f1c-7212-4f6b-ab1e-f66f09e3272a" />
</p>
<p>
<img width="1082" height="767" alt="Screenshot 2026-08-13 131444" src="https://github.com/user-attachments/assets/235d8ee6-993b-45aa-8c0a-75c696c5ceec"/>
</p>
<p>
<img width="995" height="572" alt="Screenshot 2026-08-13 131507" src="https://github.com/user-attachments/assets/00b96fbc-1f3b-42ad-a1af-294c9a46d36c" />
</p>
<p>
<img width="1067" height="468" alt="Screenshot 2026-08-14 194901" src="https://github.com/user-attachments/assets/2de6843d-7afe-4eb2-bbc1-b53399c98719" />
</p>


<br />

<p>
Copy the public IP address for the VM, then log into the VM using the username and password created in the initial setup.
<p>
<img width="1310" height="397" alt="Screenshot 2026-08-13 133226" src="https://github.com/user-attachments/assets/4407b6df-ba7d-4700-88ee-0c9e35e11976"/>
</p>
<p>
<img width="543" height="302" alt="Screenshot 2026-08-13 133548" src="https://github.com/user-attachments/assets/bfcf3ecf-b119-4093-a393-3076091698c9"/>
</p>
<p>
<img width="560" height="415" alt="Screenshot 2026-08-13 133935" src="https://github.com/user-attachments/assets/71d82f91-9bc3-4780-8fcb-9b7eff9eb2cb"/>
</p>

<br />

<p>
Once logged into the VM, download the osTicket installation zip file (linked above in the Prerequisites) and unzip it to the desktop. Leave the file name defaulted to "osTicket-Installation-Files".
<p>
<img width="1917" height="507" alt="Annotation 2026-08-14 221436" src="https://github.com/user-attachments/assets/3d56a250-689d-4cbd-8aa2-a69957d2f614"/>
</p>

<p>
Open Control Panel, Programs -> Programs and Features -> then Turn Windows features on or off.
</p>
<p>
<img width="1402" height="586" alt="Screenshot 2026-08-13 205557" src="https://github.com/user-attachments/assets/a4ed9519-1b32-4bca-9a57-4be813fb503d"/>
<p>
Select Internet Information Services and expand the folder -> expand World Wide Web Services -> expand Application Development Features -> select CGI.
</p>
<p>
<img width="552" height="490" alt="Screenshot 2026-08-13 205739" src="https://github.com/user-attachments/assets/8ff6673f-5862-4fa5-96c3-2807af4728e9" />
</p>

<p>
Within the osTicket-Installation-Files folder, install PHP Manager for IIS (PHPManagerForIIS_V1.5.0).
</p>
<p>
<img width="1060" height="468" alt="Screenshot 2026-08-13 205907" src="https://github.com/user-attachments/assets/04f6f154-844d-498a-9d3d-c38cdbfebbee"/>
</p>
<p>
Within the osTicket-Installation-Files folder, install Rewrite Module (rewrite_amd64_en-US).
</p>
<p>
<img width="1137" height="493" alt="Screenshot 2026-08-13 210011" src="https://github.com/user-attachments/assets/851a2ba8-b90f-4b62-b8be-420fc7892944" />
</p>

<p>
Navigate to the C drive and create a new folder, PHP. 
</p>
<p>
<img width="1020" height="466" alt="Screenshot 2026-08-13 210137" src="https://github.com/user-attachments/assets/e1435724-aa57-4b0a-ba56-d8cf4071845f"/>
</p>
<p>
Within the osTicket-Installation-Files folder, right-click PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) and extract all to C:\PHP.
</p>
<p>
<img width="1257" height="706" alt="Screenshot 2026-08-13 210329" src="https://github.com/user-attachments/assets/1d5312f0-1bfc-49e4-9c8f-81d105863693"/>
</p>
<p>
<img width="697" height="585" alt="Screenshot 2026-08-13 210430" src="https://github.com/user-attachments/assets/cb0e6421-deba-48e6-82fd-51163c7f402d" />
</p>
<p>
Within the osTicket-Installation-Files folder, install VC_redist.x86 
</p>
<p>
<img width="1097" height="465" alt="Screenshot 2026-08-13 210552" src="https://github.com/user-attachments/assets/3d9fa461-01a9-4e5d-b180-7a48e8185ebd"/>
</p>

<p>
Within the osTicket-Installation-Files folder, install MySQL 5.5.62 (mysql-5.5.62-win32). Select Typical Setup -> on the next screen ensure to select Launch Configuration Wizard -> then Finish
</p>
<p>
<img width="1141" height="482" alt="Screenshot 2026-08-13 210657" src="https://github.com/user-attachments/assets/7489ad0b-bb8a-4c6a-9d69-f41eba0cf0cc"/>
</p>
<p>
<img width="612" height="475" alt="Screenshot 2026-08-13 210745" src="https://github.com/user-attachments/assets/b4675efc-20eb-499b-a481-2bace432ecbd"/>
</p>
<p>
<img width="612" height="477" alt="Screenshot 2026-08-13 210842" src="https://github.com/user-attachments/assets/79f0c154-ee3b-4870-be09-3b81ce5c1724"/>
</p>
<p>
Within the Configuration Wizard, select Standard Configuration.
</p>
<p>
<img width="618" height="471" alt="Screenshot 2026-08-13 210941" src="https://github.com/user-attachments/assets/eb86598c-18a5-4131-87f1-622d09a0c1f7"/>
</p>
<p>
Next you will create a username and password. MAKE SURE YOU KEEP A RECORD OF THIS FOR LATER! Then Execute.
</p>
<p>
<img width="617" height="472" alt="Screenshot 2026-08-13 211057" src="https://github.com/user-attachments/assets/2ab98108-3417-46d8-80ce-bad5834203d6"/>
</p>
<p>
<img width="617" height="467" alt="Annotation 2026-08-14 222441" src="https://github.com/user-attachments/assets/0a62cbce-38a4-466d-a1ca-dc098d203145" />
</p>

<p>
Open Internet Information Services Manager (IIS) as an Admin.
</p>
<p>
<img width="975" height="842" alt="Annotation 2026-08-14 222628" src="https://github.com/user-attachments/assets/6801b886-0c5e-4806-9f28-db03c23184ec"/>
</p>
<p>
Within IIS, select PHP Manager and register new PHP version. Click the box with three dots to browse files and select "php-cgi" within C:\PHP
</p>
<p>
<img width="1920" height="837" alt="Annotation 2026-08-14 222742" src="https://github.com/user-attachments/assets/e78aa2c8-1d3a-467a-ae97-678d5a3a31d1"/>
</p>
<p>
<img width="1038" height="800" alt="Annotation 2026-08-14 222839" src="https://github.com/user-attachments/assets/d5c8865f-55d3-4a8c-b1f7-8ffbf763eefd"/>
</p>
<p>
<img width="627" height="262" alt="Annotation 2026-08-14 223033" src="https://github.com/user-attachments/assets/7dad87d8-137a-4200-b75b-74e5e2034756"/>
</p>
<p>
<img width="932" height="582" alt="Annotation 2026-08-14 222947" src="https://github.com/user-attachments/assets/b28d1c4e-2a55-4ffa-bcbd-0ed12ecc7226"/>
</p>
<p>
<img width="627" height="275" alt="Annotation 2026-08-14 223122" src="https://github.com/user-attachments/assets/d7a96180-e13c-4fb1-9fb5-f556089941ac"/>
</p>

<p>
Return to the IIS Manager and Reload IIS. To the right under Manage Server you click Restart or Stop -> Start.
</p>
<p>
<img width="1918" height="822" alt="Annotation 2026-08-14 223225" src="https://github.com/user-attachments/assets/f90a809a-7015-4cf6-88db-6fb5d0534a17"/>
</p>
<p>
Within osTicket-Installation-Files folder, extract osTicket-v1.15.8. Open osTicket-v1.15.8, and copy the upload folder to C:\inetpub\wwwroot. Rename the copied upload folder to osTicket. Return to the IIS Manager and Reload IIS.
</p>
<p>
<img width="1390" height="608" alt="Annotation 2026-08-14 223453" src="https://github.com/user-attachments/assets/5c74d383-9c4c-4976-9d39-86f95ca5ae2e"/>
</p>
<p>
<img width="1920" height="651" alt="Annotation 2026-08-14 224000" src="https://github.com/user-attachments/assets/1817d1a2-94d9-4b89-82a3-9e1943ab6664"/>
</p>
<p>
<img width="957" height="622" alt="Annotation 2026-08-14 224103" src="https://github.com/user-attachments/assets/0ea85213-d372-444d-8c2d-c672d37f2358"/>
</p>

<p>
To the left under Connections, navigate to Sites -> Default Web Site -> osTicket. Then to the right, under Browse Folder select "Browse*:80".
</p>
<p>
<img width="1917" height="657" alt="Annotation 2026-08-14 224530" src="https://github.com/user-attachments/assets/a9cb40e3-081e-40de-afe2-64280e951484"/>
</p>
<p>
<img width="1915" height="1027" alt="Annotation 2026-08-14 224806" src="https://github.com/user-attachments/assets/e423dd37-9792-43c2-b7dc-faec73c3db76"/>
</p>

<p>
You will notice there are a few recommended extensions that are disabled. Return to IIS -> Sites -> Default Web Site -> osTicket. Open PHP Manager. Select enable or disable an extension.
</p>
<p>
<img width="1195" height="910" alt="Annotation 2026-08-14 225051" src="https://github.com/user-attachments/assets/b2b42bbc-ea9c-4af9-b6e8-4e654a68e3f6"/>
</p>
<p>
Select php_imap.dll from the disabled list. Then on the top right select Enable. Repeat this process for php_intl.dll and php_opcahe.dll.
</p>
<p>
<img width="1918" height="973" alt="Annotation 2026-08-14 225227" src="https://github.com/user-attachments/assets/5dd2d1a2-e2c5-4c9f-8dea-351a90c6a0ae"/>
</p>

<p>
Refresh the osTicket setup site in the browser and confirm the extensions are enabled.
</p>
<p>
<img width="1902" height="1021" alt="Annotation 2026-08-14 225353" src="https://github.com/user-attachments/assets/0b3859a9-9f47-4c5f-ad34-7e7a9c26759e" />
</p>

<p>
Navigate to the C Drive -> inetpub -> wwwroot -> osTicket -> include. Within the include folder, rename ost-sampleconfig.php -> ost-config.php
</p>
<p>
<img width="952" height="997" alt="Annotation 2026-08-14 225654 (2)" src="https://github.com/user-attachments/assets/16fe59bb-2425-42aa-8f0c-b6bdfb9c7bee"/>
</p>
<p>
<img width="957" height="1028" alt="Annotation 2026-08-14 225806" src="https://github.com/user-attachments/assets/980cf20d-e561-4a74-bfd4-4c606aa48a09"/>
</p>

<p>
Right-click ost-config.php -> Properties -> Security -> Advanced. Select Disable Inheritance -> Remove all inherited permissions from this object.
</p>
<p>
<img width="1910" height="1022" alt="Annotation 2026-08-14 225937" src="https://github.com/user-attachments/assets/b0d48163-17e4-4041-a898-9c7c5f94d723"/>
</p>
<p>
<img width="651" height="367" alt="Annotation 2026-08-14 230040" src="https://github.com/user-attachments/assets/dabdee64-5d19-4966-9b0c-025be4637e77"/>
</p>
<p>
Click Add -> Select a principal -> in the text box enter "Everyone" -> check names -> OK
</p>
<p>
<img width="1022" height="636" alt="Annotation 2026-08-14 230208" src="https://github.com/user-attachments/assets/44087f39-47ee-49d2-9329-a2db6a489d69" />
</p>
<p>
<img width="1213" height="721" alt="Annotation 2026-08-14 230250" src="https://github.com/user-attachments/assets/6844aedf-b284-4ea6-9804-ff30fc66fc42"/>
</p>
<p>
<img width="601" height="305" alt="Annotation 2026-08-14 230348" src="https://github.com/user-attachments/assets/e2d22463-3919-49b3-ab5c-df729ab5ced4" />
</p>
<p>
Click full control -> OK, then Apply -> OK
</p>
<p>
<img width="1212" height="722" alt="Annotation 2026-08-14 230440" src="https://github.com/user-attachments/assets/b2b4d821-0d8e-4911-8a41-6e26bc52c5a7" />
</p>
<p>
<img width="1013" height="630" alt="Annotation 2026-08-14 230539" src="https://github.com/user-attachments/assets/757a39b6-7adb-4110-9253-33f3e12d8bac" />
</p>

<p>
Return to the browser and click continue to continue setting up osTicket. Enter the name and email address for the help desk. Also enter the name, email address, username, and password for the primary administrator account. 
</p>
<p>
<img width="1917" height="1026" alt="Annotation 2026-08-14 231130" src="https://github.com/user-attachments/assets/e415c727-1f87-4a70-9a1b-31c7ece63032" />
</p>

<p>
Within the osTicket-Installation-Files folder, install HeidiSQL (HeidiSql_12.3.0.6589_Setup). Click the Launch HeidiSQL box, then Finish. Skip the Donation window, then at the bottom left click New and create a new session.
</p>
<p>
<img width="957" height="682" alt="Annotation 2026-08-14 230701" src="https://github.com/user-attachments/assets/5f367a74-22ea-49a9-8012-b2d9f26b7533"/>
</p>
<p>
<img width="692" height="565" alt="Annotation 2026-08-14 231256" src="https://github.com/user-attachments/assets/5bbc258b-b8b6-44f5-b13d-9b85d11d8112" />
</p>
<p>
<img width="475" height="562" alt="Annotation 2026-08-14 231346" src="https://github.com/user-attachments/assets/2fc2832f-2a11-4272-9b1c-0261aa37028d" />
</p>
<p>
<img width="852" height="597" alt="Annotation 2026-08-14 231433" src="https://github.com/user-attachments/assets/04592b7b-5818-4910-8230-adb09b377a65" />
</p>
Enter the username and password recorded when setting up MySQL. Then click Open to open the session. To the left, you will see various other databases. Right-click in that area and create a new database. Name the database osTicket.
<p>
<img width="851" height="598" alt="Annotation 2026-08-14 231557" src="https://github.com/user-attachments/assets/53f746d4-1fe1-4c4c-bb2b-9590f53e0853" />
</p>
<p>
<img width="1166" height="735" alt="Annotation 2026-08-14 231702" src="https://github.com/user-attachments/assets/e03c9910-428a-423f-a6d2-13572673af26"/>
</p>
<p>
<img width="393" height="317" alt="Annotation 2026-08-14 231808" src="https://github.com/user-attachments/assets/64d069c1-4d94-4442-bd69-c30b6b749d83" />
</p>


<p>
Return to the browser to finish setting up osTicket. Enter the MySQL Database (osTicket) and the MySQL username and password. Then click Install Now
</p>
<p>
<img width="1036" height="470" alt="Annotation 2026-08-14 231918" src="https://github.com/user-attachments/assets/89157bee-a842-4bb9-a9a4-75c85d7325ee" />
</p>
<p>
The installation is complete and ready for use! You can access the help desk login page (http://localhost/osTicket/scp/login.php) and End User page (http://localhost/osTicket/)
</p>
<p>
<img width="1920" height="997" alt="Annotation 2026-08-14 232026" src="https://github.com/user-attachments/assets/d7071ea6-a82f-45f0-aee5-1b3be3a19991" />
</p>
<p>
<img width="1920" height="922" alt="Annotation 2026-08-14 232224" src="https://github.com/user-attachments/assets/0f1f98ec-c6d3-4ff3-95a6-866212f35d87" />
</p>
<p>
<img width="1920" height="820" alt="Annotation 2026-08-15 175307" src="https://github.com/user-attachments/assets/e04da4a6-1920-46ba-8a67-0cf5c8c8f2d8" />
</p>
<p>
The installation is complete but there is a bit of clean up left to do. 
Navigate to C: -> inetpub -> wwwroot -> osTicket and delete the setup folder.
</p>
<p>
<img width="950" height="706" alt="Annotation 2026-08-14 232428" src="https://github.com/user-attachments/assets/fabe66eb-8d24-46c0-b365-fbad8d5bdd9a" />
</p>

<p>
Navigate to C: -> inetpub -> wwwroot -> osTicket -> include, and right-click ost-config.php -> Properties. On the General Tab -> click Read-only -> Apply -> OK.
</p>
<p>
<img width="957" height="1013" alt="Annotation 2026-08-14 232609" src="https://github.com/user-attachments/assets/fb7547a5-84c4-467b-b526-4f91858dd84a"/>
</p>
<p>
<img width="477" height="623" alt="Annotation 2026-08-14 232735" src="https://github.com/user-attachments/assets/04520ab0-ab40-4d30-b5d9-e42f7ce0380c" />
</p>

<p>

</p>

<br />
