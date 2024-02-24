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
Verify your info and Install:  <br/>
Wait for the instal to finish and the computer to restart:  <br/>
This server will be headless, we will login into the Proxmox server over the network:  <br/>
<img src="https://i.imgur.com/7CO1IN5.png" height="80%" width="80%" alt="Desk"/>
<br />
<br />
Verfy your server IP is outside of your DCHP:  <br/>
Fix your IP address on your network for your new server: <br/>
<img src="https://i.imgur.com/FyWXyk9.png" height="80%" width="80%" alt="Desk"/>
<br />
<br />
Navigate to your Proxmox server address in a web browser:  <br/>
User name, root:  <br/>
Use your admin password and login:  <br/>
<img src="https://i.imgur.com/pEEyKWe.png" height="80%" width="80%" alt="Desk"/>
<br />
<br />
Click OK for No valid subscription, Proxmox does not require a subscription:  <br/>
Under your data center select your server, then open your sell:  <br/>
Ensure your local file is using all of your space:  <br/>
First delete your local file with the following command <br/> 
lvremove /dev/pve/data <br/>
Alocate the entire drive to your local storage for your VM <br/> 
lvresize -l +100%FREE /dev/pve/root  <br/>
Last resize command <br/> 
resize2fs /dev/mapper/pve-root:  <br/>
<img src="https://i.imgur.com/c2uExS0.png" height="80%" width="80%" alt="Desk"/>
<br />
<br />
We navigate to Storage in the Datacenter tab:  <br/>
Highlight local-lvm and click remove: <br/>
This is not a required step, but it is good practice to clear any links to folders you have deleted:  <br/>
<img src="https://i.imgur.com/Eaa0zi4.png" height="80%" width="80%" alt="Desk"/>
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
