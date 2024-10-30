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

- Sever Setup
- Web Server
- IIS and CGI enabling
- PHP Installation
- Directory
- Database Setup
- Database Management Tool
- Email Configuration
- Directory Permissions

<h2>Sever Set Up</h2><p>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
This screenshot shows the Azure portal where I set up a virtual machine (VM). Using Azure provides a flexible and powerful environment for installing an operating system tailored to my development needs. It allows for quick deployment of a VM, enabling me to test and develop applications without being limited by local hardware.
</p>
<br />

<h2>Web Server</h2><p>
  
  
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Through the Microsoft 10 virtual machine, I opened the osTicketing system zip file obtained from the osTicket website. Downloading the oSticket-Installation-Files 
crucial for setting up the osTicket system, as they contain the core components needed for its operation, including PHP scripts and configuration files.
</p>
<br />

<h2>IIS AND CGI Installation</h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enabling IIS (Internet Information Services) with CGI (Common Gateway Interface) when setting up a Windows OS is really important if you want to host web applications. IIS acts as a reliable web server, and with CGI, you can interact with scripts to create dynamic content. This setup is perfect for testing your web apps locally, ensuring everything works smoothly before going live. Plus, it helps with compatibility across various technologies and boosts performance.
</p>
<br />

<strong>Insalltion Steps</strong>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open Control Panel:
Press the Windows key, type "Control Panel," and hit Enter.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Go to Programs:
Click on Programs, then select Turn Windows features on or off.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable IIS:
In the Windows Features dialog, scroll down and find Internet Information Services.
Check the box next to it. Expand it by clicking the plus sign to see additional features.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Enable CGI:
Under Web Management Tools and World Wide Web Services, look for Application Development Features.
Check the box for CGI.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Confirm and Install:
Click OK to start the installation. Windows will apply the changes, which may take a few minutes.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Verify Installation:
Once complete, you can verify by opening a web browser and typing http://localhost. You should see the IIS welcome page if it’s working correctly.
</p>
<br />

<h2>PHP Installation</h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
In the screenshot above we are installing PHP Manager. This is a user-friendly tool that lets you install, run, and manage different PHP versions on a Windows server using Internet Information Services (IIS). It makes it easy to enable or disable PHP extensions and adjust PHP settings through the php.ini file, ensuring everything runs smoothly for your hosted applications.

  PHP - PHP scripts are files that contain code written in the PHP (Hypertext Preprocessor) programming language. They are primarily used for server-side web development, enabling dynamic content generation and interaction with databases. When a user requests a PHP page, the server processes the PHP code and returns the resulting HTML to the user's browser. PHP scripts can handle tasks like form submissions, user authentication, data retrieval from databases, and session management, making them essential for building interactive and dynamic web applications
</p>
<br />

<strong>Installation Steps</strong>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Run the Installer:
Once the download is complete, locate the .msi file in your Downloads folder and double-click it to run the installer.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Follow Installation Prompts:
Follow the on-screen instructions to install PHP Manager. Accept the license agreement and choose the installation options as needed.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Complete the Installation:
After installation, you may need to restart IIS. You can do this by opening a Command Prompt as an administrator and typing iisreset.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Verify Installation:
Open IIS Manager and look for "PHP Manager" in the features view for your server. This indicates that the installation was successful.
</p>
<br />

<strong> Rewrite Module (rewrite_amd64_en-US.msi) Installtion/Steps</strong>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Installing the Rewrite Module (rewrite_amd64_en-US.msi) for IIS is essential for effective URL management on your web server. It enables you to create clean, user-friendly URLs that enhance SEO and user experience. The module also allows for easy redirects, helping users find the right content even when URLs change. Additionally, it offers features like custom error pages and advanced URL rewriting, providing greater flexibility for your applications. Overall, it’s a crucial tool for optimizing your IIS server and improving website performance.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Run the Installer:
Locate the downloaded .msi file in your Downloads folder and double-click it to launch the installer.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Follow the Installation Prompts:
A setup wizard will appear. Click Next to proceed through the installation steps.
Read and accept the license agreement, then click Next.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Choose Installation Options:
If prompted, select the installation options that suit your needs. The default settings are usually sufficient.
</p>
<br />

<h2>Creating the directory C:\PHP</h2>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Creating the directory C:\PHP is essential when setting up a web server or developing PHP applications. It promotes organizational structure by keeping scripts and libraries separate, simplifies web server configuration as it can serve as the document root, and aligns with the directory requirements of many PHP frameworks. This dedicated directory also facilitates local development, makes path management easier, and supports proper PHP installation and deployment practices. Overall, establishing a clear directory structure from the outset enhances project manageability and efficiency.
<br />

<strong>Insalltion Steps</strong>
<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Open File Explorer: You can do this by pressing Windows + E or clicking on the File Explorer icon in the taskbar.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Navigate to the C: Drive: Click on "This PC" or "Computer" in the left sidebar, then double-click on the C: drive.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Create a New Folder:
Right-click in an empty space in the directory.
Select New > Folder from the context menu.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rename the Folder: The new folder will be highlighted for renaming. Type PHP and press Enter.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Rename the Folder: The new folder will be highlighted for renaming. Type PHP and press Enter.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
From the “osTicket-Installation-Files” folder, unzip PHP 7.3.8 (php-7.3.8-nts-Win32-VC15-x86.zip) into the “C:\PHP” folder
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
FRight-Click the Zip File: Right-click on the php-7.3.8-nts-Win32-VC15-x86.zip file.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Extract the Files:
Select Extract All... from the context menu.
In the dialog that appears, set the destination to C:\PHP. If it’s not automatically filled, type C:\PHP in the text box.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start Extraction: Click the Extract button to begin unzipping the files.
</p>
<br />

<strong>From the “osTicket-Installation-Files” folder, install VC_redist.x86.exe.
</strong>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Installing VC_redist.x86.exe (the Visual C++ Redistributable) is essential when setting up an osTicket system, as it provides the necessary runtime components that many PHP applications rely on. This installation ensures compatibility with various PHP extensions and libraries, preventing runtime errors related to missing or incompatible C++ libraries. By including the redistributable, you simplify the setup process, ensuring that all required components are present for a smooth and effective osTicket operation.
</p>
<br />

<h2>Database Setup</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Installing MySQL 5.5.62 from the “osTicket-Installation-Files” folder is essential for setting up an osTicket system, as it provides the necessary database management for storing tickets, users, and settings. This specific version ensures compatibility with osTicket, minimizing potential issues from using unsupported database versions. It is optimized for the performance needs of osTicket, streamlining the setup process and enabling key features like ticketing and user management. Overall, installing MySQL is crucial for ensuring a reliable and efficient operation of the osTicket system.
</p>
<br />

<strong>Here are the steps to install MySQL 5.5.62 </strong>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Locate the Installation File
Open the “osTicket-Installation-Files” Folder: Navigate to the directory where you have the osTicket installation files.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Find the MySQL Installer: Look for the file named mysql-5.5.62-win32.msi.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
 Run the Installer
Double-Click the Installer: Right-click on mysql-5.5.62-win32.msi and select Run as administrator. This ensures you have the necessary permissions for installation.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
  Follow the Installation Wizard
Welcome Screen: Click Next to begin the installation.
License Agreement: Read the license agreement, select I accept the terms in the license agreement, and click Next.</p>
<br />








