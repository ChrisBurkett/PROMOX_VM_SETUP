<h1>Virtual Machines on Proxmox </h1>


<h2>Description</h2>
Setting up first Virtual Machine with Proxmox.


<h2>Virtual Machine Used</h2>

- <b>Parrot</b>

<h2>Sever Used </h2>

- <b>Proxmox</b>

<h2>Add VM ISO to PROMOX:</h2>

<p align="center">
Navigate to your Proxmox server in a web browser: <br/>
Navigate to Local storage, ISO Images, and click Upload on the top of the page: <br/>
Use "select file" and select the ISO image from your computer and click upload: <br/>
This will upload the ISO onto your Promox storage: <br/>
: <br/> 
<img src="https://i.imgur.com/9jE7v71.png" height="80%" width="80%" alt="Creating"/>
<br />
<br />
Click "Create VM" in the top right the GUI:  <br/>
Give your VM a name and click next:  <br/>
<img src="https://i.imgur.com/OMnz9BC.png" height="80%" width="80%" alt="ERD"/>
<br />
<br />
Use the ISO image dropdown to select your iso and click next: <br/>
<img src="https://i.imgur.com/jEEnwr4.png" height="80%" width="80%" alt="Keys"/>
<br />
<br />
The system page you can add a TPM if required or change the bois, then click next:  <br/>
<img src="https://i.imgur.com/Ww3yt18.png" height="80%" width="80%" alt="RMA"/>
<br />
<br />
Change any storage settings needed here:  <br/>
Note! Storage bandwidth settings can be changed with the bandwidth tab here:  <br/>
Click next <br/>
<img src="https://i.imgur.com/gx9uMfE.png" height="80%" width="80%" alt="Records"/>
<br />
<br />
Change CPU settings here:  <br/>
Take special note on how many Cores you are relocating to this machine, default is 1 core:  <br/>
Click Next:  <br/>
<img src="https://i.imgur.com/ugUmjOE.png" height="80%" width="80%" alt="Desk"/>
<br />
<br />
Change memory allocation here and click next:  <br/>
<img src="https://i.imgur.com/69Y0G3l.png" height="80%" width="80%" alt="Desk"/>
<br />
<br />
Choose what network interface card you want your VM to use, click next:  <br/>
<img src="https://i.imgur.com/TB12V0K.png" height="80%" width="80%" alt="Desk"/>
<br />
<br />
Verify your VM info and click Finish:  <br/>
<img src="https://i.imgur.com/7RJGQpl.png" height="80%" width="80%" alt="Desk"/>
<br />
<br />
Locate your VM on the sidebar to the left and right click and left click start:  <br/>
<img src="https://i.imgur.com/5vTYPFM.png" height="80%" width="80%" alt="Desk"/>
<br />
<br />
CLick on your VM on the left panel and click on Console next:  <br/>
Install your VM if required:  <br/>
Click the rigth CTRL button to take your mouse off of the VM:  <br/>
<img src="https://i.imgur.com/q0fxv6a.png" height="80%" width="80%" alt="Desk"/>
<br />
<br />
To shutdown your VM use the shutdown drop down at the top of the page. <br/> 
Reboot will restart the VM, STOP will end the VM immediately:  <br/>
<img src="https://i.imgur.com/uJv3a3y.png" height="80%" width="80%" alt="Desk"/>
<br />
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
