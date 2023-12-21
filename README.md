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
- Item 5

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
