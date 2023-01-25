# Nessus Credentialed Scan Lab

 ### [YouTube Demonstration](https://www.youtube.com/watch?v=feCKKUBmFUo)

<h2>Description</h2>
In this lab, a credentialed scan using Nessus was conducted on a Windows 10 virtual machine. The host and Nessus were configured, and the scan results were analyzed. An older version of the Firefox browser was then downloaded and re-scanned to show critical vulnerabilities. Remediation options were evaluated and applied by uninstalling the outdated browser and running updates on the virtual machine. The scan was re-run to confirm that all critical vulnerabilities had been removed.

** NOTE ** The Virtual Machine we are using is Vmware with Windows 10 installed and configured. In a later video I will demonstrate on how I created teh virtual machine and installed Windows 10. 

 
<br />


<h2>Languages and Utilities Used</h2>

- <b>Nessus</b> 

<h2>Environments Used </h2>

- <b>Windows 10</b> (21H2)
- <b>VMware Virtual Machine</b>

<h2>Program walk-through:</h2>

<p align="center">
We will first start with pulling up CMD on our desktop to conduct a ping on VM Host. The request times out on the first try.: <br/>
<img src="https://imgur.com/0z95X92.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Due to our machine being unable to ping the VM, we will disable a few firewall settings on the VM to allow the ping to go through. This will help in ensuring the the Nessus scan can be conducted on the Virtual Machine. To disable the firewall settings, we will go to the virtual machine and search wf.msc-> Windows Defender Firewall Properties. Switch to Off on all three profile tabs. :  <br/>
<img src="https://imgur.com/bXRghIW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Now we are getting a reply and succesful ping from the Virtual Machine: <br/>
<img src="https://imgur.com/4OVSQus.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Now that we are able to ping the Virtual Machine, we will go to Nessus, click on new scan-> Basic Network Scan. Here we will enter the information needed for our new scan, including the IP address of the Virtual Machine. Click on save to continue :  <br/>
<img src="https://imgur.com/2dtSwKX.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
We will now click on the play button to run the scan.. This can typically take about 5-10 min :  <br/>
<img src="https://imgur.com/RHWHj5j.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
After waiting a few minutes, we can now see that there are vulnerabilites appearing from our scan. Each vulnerability is measured by risk and remediations and recommendations are provided for each vulnerability. Everything checks out good from this scan. This concludes our lab:  <br/>
<img src="https://imgur.com/1NegEXg.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
