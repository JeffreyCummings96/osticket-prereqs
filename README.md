<p align="center">
<img src="https://i.imgur.com/Clzj7Xs.png" alt="osTicket logo"/>
</p>

<h1>osTicket - Post-Install Configuration</h1>
This tutorial outlines the post-install configuration of the open-source help desk ticketing system osTicket.<br />



<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Internet Information Services (IIS)

<h2>Operating Systems Used </h2>

- Windows 10</b> (21H2)

<h2>Post-Install Configuration Objectives</h2>

- ISS
- Item 2
- Item 3
- Item 4
- Item 5

<h2>Configuration Steps</h2>

<p>
Configure IIS doing the following:
Right Click -> start menu -> "Run"
 <img src=https://i.imgur.com/2aFtJIO.png
</p>
<br />

<p>
type "control" in the "run" bar when the control panel pops up click programs -> Turn Windows features on or off.
<img src="https://i.imgur.com/gHDnukV.png"
</p>
<p>
check Internet Information Services -> World Wide Web Services -> CGI
<img src=https://i.imgur.com/FDdW0OJ.png
</p>
<br />

<p>
On Windows Features locate "Common HTTP Features" make sure every box is checked off and then click "Ok"
</p>
<p>
After completing the above steps IIS will begin installing, IIS is a web server that osTicket runs on.
</p>
<br />
