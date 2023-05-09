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
  Note: I already have an Azure Tenant created as well as an active subscription.  
- Item 1> Creating a resource group
- Item 2> Create VM for Virtual Network  
- Item 3> Create Subnet
- Item 4> Installation of dependencies for osTicket System 
- Item 5> Install osTicket on VM

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/4H6LiM8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
1>I have here where the subscription is present. I then created a resource group called RG-osTicket. 
</p>
<br />

<p>
<img src="https://i.imgur.com/lLpSzBV.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/uHtZrC8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
2>Next up we have the task of creating our virtual machine. 
</p>
<br />

<p>
<img src="https://i.imgur.com/wqxNQGw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
The process of going through the preinstalation steps gets easier with time. I find it quite enjoyable now that navigating thorought the Azure portal is more like seeing a familiar face. 
</p>
<br />


<p>
Item 3> Here we have created our subnet automatically. 
</p>
<p>
<img src="https://i.imgur.com/vHmHSV1.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
<img src="https://i.imgur.com/NUCp9jO.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/50WDtVd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
4> Installation of dependencies for osTicket System 
  In order to install dependancies it requires me to Remote Desktop into the VM. Once we are in our VM we need to enable IIS (Internet Information Services)with CGI. 
</p>

<p>
<img src="https://i.imgur.com/uRGBZ8G.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

<p>
<img src="https://i.imgur.com/Y0NTOdS.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


<p>
<img src="https://i.imgur.com/vPGiXb0.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

</p>
> Pre-Installation continued. 
  In order to make sure our selections are correct for IIS we put in a loopback to get the ISS page. Next we install PHP Manager for IIS.Next we download the Rewrite Module Create a C: folder and call it PHP.Unzip php contents file into PHP folder. 
</p>

<p>
<img src="https://i.imgur.com/giJxLm9.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

</p>
> Pre-Installation continued. 
  Next we download C++ redistributable. 
</p>

<p>
<img src="https://i.imgur.com/rLbwxFD.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

</p>
> Pre-Installation continued. 
  Next we download MySql Server. 
</p>

<p>
<img src="https://i.imgur.com/ZyyeoL2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


<p>
<img src="https://i.imgur.com/HQo0apf.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


</p>
> Pre-Installation continued. 
  Next we configure IIS as an admin by registering a new PHP version to C:\PHP-cgi.exe. 
</p>

<p>
<img src="https://i.imgur.com/SF8kM7P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

</p>
> Pre-Installation continued. 
  Install osTicket and get the upload file from going in and xfer this file to the c:\inetpub\wwwroot folder. In IIS go to PHP manager under osTicket. Enabale the following extensions php_imap.dill, php_intl.dill, php_opcache.dill.
  C:\inetpub\wwwroot\osTicket\include\ost-sampleconfig.php rename to 
  ost-config.php.
  
  Next we will change the file to allow permissions for everyone.
  
  
  Fill out osTicket Basic Installation information. Leave the Database Settings information for a bit later. 
</p>

<p>
<img src="https://i.imgur.com/bdvKgWK.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


</p>
> Pre-Installation continued. 
  Next we download HeidiSQL for connection our database.
</p>


<p>
<img src="https://i.imgur.com/4m32RTj.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>



</p>
> Pre-Installation continued. 
  We are going to create a new connection so click new. Now we are connected to MySQL Server. Right click on Unamed Data Base to Creat new database and named osTicket. 
  
  GO BACK to os Installer to finish putting in the Database Settings information. 
</p>

<p>
<img src="https://i.imgur.com/uNRrlf2.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>

</p>
> Pre-Installation continued. 
  We are going to change the permissions on file ost-config.php to read and execute. 
  
</p>

<p>
<img src="https://i.imgur.com/Bundn5P.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


<p>
5> Finally finish installing osTicket on VM by putting in you credentials. 
</p>

<p>
<img src="https://i.imgur.com/0qt1rLd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>


<p>
<img src="https://i.imgur.com/VxRVbdH.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>



<p>
6>Thank you for taking the time out of your day to look at the growth I have my in my IT journey displayed throught this portfolio project!
</p>


