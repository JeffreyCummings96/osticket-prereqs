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

- IIS
- PHP Manager
- IIS Rewrite Module
- c++ Redistributable
- MySQL

<h2>Installation Steps</h2>

<p>
<img src=https://i.imgur.com/2aFtJIO.png
</p>
<p>
Configure IIS doing the following:
Right Click -> start menu -> "Run"
</p>
<br />

<p>
<img src="https://i.imgur.com/gHDnukV.png"
</p>
<p>

</p>
<br />
type "control" in the "run" bar when the control panel pops up click programs -> Turn Windows features on or off.
<p>
<img src=https://i.imgur.com/FDdW0OJ.png/>
</p>
<p>
check Internet Information Services -> World Wide Web Services -> CGI
</p>
<br />
<p>
On Windows Features locate "Common HTTP Features" make sure every box is checked off and then click "Ok."
After completing the above steps IIS will begin installing, IIS is a web server that osTicket runs on.        
</p>
<br />
<p>
<img src=https://i.imgur.com/43Bon4d.png/>
</p>
<p>
To test the connection go to a web browser and type 127.0.0.1 the page should look like the image above that shows the default IIS web page.
</p>
<br />
<p>
<img src=https://i.imgur.com/RlEKanC.png/>
</p>
<p>
  Next is to install PHP Manager for IIS
</p>
<p> 
<img src=https://i.imgur.com/zYjUOR9.png/>
</p>
<p>
 Once PHP Manager is Downloaded the next step is to install  IIS Rewrite Module
</p>
<p>
<img src=https://i.imgur.com/jiQT0v8.png/>
</p>
<p>
  Create the directory C:\PHP on local hard drive 
</p>
<p>
<img src=https://i.imgur.com/LQ8QJAe.png/>  
</p>
<p>
install c++ Redistributable  
</p>
<p>
  <img src=https://i.imgur.com/fkKhFQh.png/> 
</p>
<p>
  Next Install MySQL Server -> Choose Setup Type -> Typical 
</p>
<p>
 <img src=https://i.imgur.com/UKKwsgR.png/>   
</p>
<p>
  Next configure MySQL Configuration Wizard -> Standard Configuration -> Configure Root Password -> execute
  
<b>This Configuration is setting up a database on the computer because osTicket needs a database to store tickets onto.</b>
</p>
<p>
<img src=https://i.imgur.com/YIaKOtH.png/>
</p>
<p>
Go to the start searchbar type in "IIS" right click and run as admin in order to register PHP within IIS
</p>
<p>
  <img src=https://i.imgur.com/3rdx21V.png/>
</p>
<p>
  Double Click PHP Manager -> Register New PHP version -> Select the PHP folder in C: Drive  -> PHP Cgi -> Ok
</p>
<p>
<img src=https://i.imgur.com/z3kZlMZ.png/>  
</p>
<p>
  Extract and copy “upload” folder to c:\inetpub\wwwroot -> Within c:\inetpub\wwwroot, Rename “upload” to “osTicket”
</p>
<p>
  <img src=https://i.imgur.com/4p5fu3v.png/>  
</p>
<p>
  Go to sites -> Default -> osTicket
On the right, click “Browse *:80”
</p>
<p>
  <img src=https://imgur.com/tTGX4ax/> 
</p>
<p>
  some extensions are not enabled
Go back to IIS, sites -> Default -> osTicket
Double-click PHP Manager
Click “Enable or disable an extension”
Enable: php_imap.dll
Enable: php_intl.dll
Enable: php_opcache.dll
Refresh the osTicket site in your browse.

</p>
