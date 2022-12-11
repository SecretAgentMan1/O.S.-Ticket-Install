# O.S.-Ticket-Install
This tutorial shows how to download O.S. support ticket.
## Video Demonstration
https://youtu.be/TJLXLykXqo0
## Technologies and Environments Used
- Virtual Box
  - Windows V.M.s
- Internet Information Services
  - For Connecting our services together. 
- Heidi Sql
  - For Database
 ## Operating System Used
 - Windows 10 Pro
 ## Installation Steps
Ok, welcome to my first tutorial! First things first we will have to create a Virtual machine using Oracle VirtualBox. 
We will be using a VM which is a remote computer. We are using a VM in order to protect our physical machine just in case something breaks. 
In this case it's a windows 10 Pro V.M.
 
![image](https://user-images.githubusercontent.com/23139364/206923552-6cc91c02-0e0d-46d8-a52d-33211ffc55f8.png)

### Step 1: The first thing you need to do is download these programs, and envrionments.
- [Heidi Sql](https://www.heidisql.com/download.php)
- [PHPManager](https://www.php.net/releases/8.2/en.php)
- [WebPlatformInstaller](https://www.microsoft.com/web/downloads/platform.aspx)
- [osTicket](https://osticket.com/editions/)

### Step 2: The second step is to enable I.I.S.
This can be done by going into Control Panel > Programs > Programs and Features then enable Internet Information Services in the Windows Features panel where it says turn features on or off.

![Image](https://camo.githubusercontent.com/53b44f25c4fca037622e4384d661fd8708ab0eedc33d72521d22a185a79b2bf6/68747470733a2f2f692e696d6775722e636f6d2f7174456e7557752e706e67)

### Step 3: Install Microsoft Web Platform Installer
Just keep clcking next until install.

![Image](https://camo.githubusercontent.com/3d7bf59fdc2aa176e6b763227ca1c426ec74c75ea1bd5a1be171e8e129c662dd/68747470733a2f2f692e696d6775722e636f6d2f417848436651362e706e67)


### Step 4: Install Open Web Installer Platform

Open Web Installer Platform after installation. You will set up MySQL 5.5 from within the program. Install PHP's x86 version up to version 7.3 after that. There are some unsuccessful files that can be accessed with the install link, including the C++ redistributable package, PHP 7.3.8, and PHP Manager for IIS.

![Image](https://camo.githubusercontent.com/0a217e07ac4c8c87c854c62c873ee404f9f3400306dcd2925b41210630df1f85/68747470733a2f2f692e696d6775722e636f6d2f4a4a38625a654a2e706e67)


### Step 5: Install osTicket

Then download osTicket. Then extract and copy the "upload" folder into c:\inetpub\wwwroot. Afterwards rename the folder to osTicket.
-[osTicket](https://osticket.com/editions/)

![Image](https://camo.githubusercontent.com/2dbc29620ca28bb970a4446c4c876181149d6280e1ed9f242b69cbe8ab6ae35f/68747470733a2f2f692e696d6775722e636f6d2f54554769534b692e706e67)

### Step 6 
