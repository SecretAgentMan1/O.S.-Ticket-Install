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
- [osTicket](https://osticket.com/editions/)

![Image](https://camo.githubusercontent.com/2dbc29620ca28bb970a4446c4c876181149d6280e1ed9f242b69cbe8ab6ae35f/68747470733a2f2f692e696d6775722e636f6d2f54554769534b692e706e67)

### Step 6: Open up the osTicket Webserver

Restart the server and then open IIS Manager. Once inside IIS Manager, navigate to Sites-> Default-> osTicket and select "Browse*.80"; the osTicket webserver should then open in your default browser.

![image](https://user-images.githubusercontent.com/23139364/206926755-2fa97e46-866b-4c53-8a61-72bc96cf5fe4.png)

### Step 7: Enable Php Extensions in I.I.S.

Reopen IIS Manager and turn on a few extensions. You must navigate to Sites->Default->osTicket to complete this. then click PHP manager twice. "Disable or enable an extension" should be clicked. Refresh the osTicket webserver to observe the changes after enabling "php intl.dll" and "php opcache.dll." Now, "Intl Extension" must be activated.

![Image](https://camo.githubusercontent.com/5926d9b6541207c854540b86aa1532fead2da5c412d773d3a925c0f6367eac05/68747470733a2f2f692e696d6775722e636f6d2f41505a675554542e706e67)

### Step 8: Configure http extensions.

Go return to ost-sampleconfig.php in the c:inetpubwwwrootosTicket directory. The file should now be called c:inetpubwwwrootosTicketincludeost-config.php. Give ost-config.php permissions. Eliminate inheritance Remove all New Permissions, -> everyone, -> all.

![Image](https://camo.githubusercontent.com/0a89dc3d5a476c0a5d2a90e808776c26c1c24397702e3064076650c9e6fcd040/68747470733a2f2f692e696d6775722e636f6d2f316e59615947652e706e67)

### Step 9:  

![Image](https://camo.githubusercontent.com/0a89dc3d5a476c0a5d2a90e808776c26c1c24397702e3064076650c9e6fcd040/68747470733a2f2f692e696d6775722e636f6d2f316e59615947652e706e67)

Afterwards continue setting up osTicket in the browser (click continue) then you will name the Helpdesk to your liking. Select a default email that will receive emails from customers who submit tickets.
