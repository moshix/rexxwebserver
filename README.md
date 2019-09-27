# rexxwebserver
Beyond web server in REXX with CGI capabilities and demo cgis for monitoring z/VM

Here is an example of what this web server can do with just a few commands as a z/VM service machine:

Welcome to the z/VM Mainframe!

This website is helps me monitor my z/VM mainframe. On this system I run the following operating systems as guest machines:

 	z/OS 2.2
	z/OS 2.3

Some of these guest machines have up to 12GB of storage assigned to them. Som e others only 16 megabytes. 

What do I do on this mainframe?

Here are some of the activities going on here:

HLASM, REXX and PL/I programming under z/VM and z/OS 
zLinux porting of parity blockchain software
performance benchmarking
time sharing use for about 60 users


What hardware is this mainframe running on?

This server is running inside an IBM z/PDT mainframe, type 1090, on top of a Lenovo Cube c730 computer. The advantage of a gaming computer is quick processors, fast ram, and tons of very fast NVME and SSD disks. < /p>

This Lenovo computer has 64GB of RAM, an i7 CPU, and about 20TB of a mix of NVME, SSD, and spinning disks (mostly for backup)&nb sp;

Monitor this mainframe

Monitor load

Monitor files

Monitor IPL time

Monitor everything

 
 
 Or just check out http://104.198.173.201:8080/cgi-bin/cms?load
 
 How to install and operate
 ==========================
 
 1. create a G-permissioned guest machine for your z/VM
 -give it like 64MB of RAM
 -30 cyls 191 minidisk
 -link to the 592 TCPIP minidks
 
 2. format the 191 minidisk with any volume label you like
 
 3. copy the vmarc utility to the minidisk and your basic PROFILE EXEC to access the TCPIP 592 disk as B
 
 4. upload the VMARC archive in this repository to the 191 minidisk by FTP or terminal file transfer or smoke signal protocol
 
 5. vmarc unpk webserve vmarc a  (this will unpack the archive)
 
 6. change the included sample INDEX HTML to your heart' content
 
 7. start the webserver with HTTPD, voila' 
 
 8. you can test it by going to the IP of your z/VM and port 8080 like so: http://1.1.1.1:8080/
 
 Change port as you wish
 
 have fun!
 
 moshix
 
 
