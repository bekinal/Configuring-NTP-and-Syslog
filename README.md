<h1>Configuring NTP and Syslog</h1>

<h2>Description</h2>
Project consists of configuring a syslog server and an NTP server to log events across the network. Then, a router is configured to send system logs to the syslog server.
<br />


<h2>Utilities Used</h2>

- <b>VirtualBox</b> 
- <b>Cisco Packet Tracer</b>

<h2>Environments Used </h2>

- <b>Windows 10</b>

<h2>Event logging and NTP review:</h2>
A syslog server is a computer that runs syslog software. The syslog software concentrates logs from all devices (PC, router, etc.) on the network into one centralized location, which makes management and log backup easier.<br/>
The following table lists syslog severity levels with their corresponding numbers:<br/>
<img src="https://imagizer.imageshack.com/img923/8952/GCABYn.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
An NTP server (Network Time Protocol) is responsible for the synchronization of the time and date across all devices on the network. NTP is a simple client-server protocol and is implemented on networks everywhere.<br/>
<br />
<br />

<h2>Configure syslog:</h2>
Network Topology:<br/>
<img src="https://imagizer.imageshack.com/img922/2325/nLeNkY.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The syslog server is accessed, and syslog services are turned on:<br/>
<img src="https://imagizer.imageshack.com/img922/2750/P1TI8Y.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
The syslog server is pinged from router 1 to verify connectivity:<br/>
<img src="https://imagizer.imageshack.com/img924/852/I3qPvG.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Security severity level 7 (debugging) is permitted, and global configuration mode is exited:<br/>
<img src="https://imagizer.imageshack.com/img923/2107/vYlRHP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Debugging for the ICMP protocol is enabled and PC1 is pinged from the router:<br/>
<img src="https://imagizer.imageshack.com/img924/253/N4rskc.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Syslog is verified as running by opening the server:<br/>
<img src="https://imagizer.imageshack.com/img922/5522/GoOjkd.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />


<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
