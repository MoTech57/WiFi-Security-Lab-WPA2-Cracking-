<h1>Wi-Fi Security Lab: WPA2 Cracking</h1>


<h2>Description</h2>
This project demonstrates a controlled Wi-Fi security lab where I captured and cracked a WPA2 password using Linux, Kali VM, and Raspberry Pi. The process involved packet capture, WPA2 handshake analysis, and a dictionary-based attack with aircrack-ng, successfully revealing the test password “test123!”. The lab highlights how WPA2 remains vulnerable to weak passwords and reinforces the importance of strong passphrases and migration to WPA3.
<br />


<h2>Languages and Utilities Used</h2>

- <b>Bash/Shell scripting</b> 
- <b>Linux networking utilities</b>
- <b>Wireshark</b> 
- <b>SSH</b>

<h2>Environments Used </h2>

- <b>Fedora Linux</b> 
- <b>Kali Linux (VM)</b> 
- <b>Raspberry Pi (Raspberry Pi OS)</b> 
- <b>Lab Router</b> 

<h2>Attack Workflow:</h2>

<p align="center">
Lab network created with spare router + Raspberry Pi 4 Password: test123!: <br/>
<img src="https://i.imgur.com/iKyEhx8.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Monitordn.sh create to enable monitor mode:  <br/>
<img src="https://i.imgur.com/pry0CVu.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Monitorup.sh create to enable managed mode: <br/>
<img src="https://i.imgur.com/4adI6dW.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Discover nearby Wi-Fi networks using airodump-ng:  <br/>
<img src="https://i.imgur.com/kcFgVPw.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Deauthentication to Forces client reconnection Confirm handshake in Wireshark:  <br/>
<img src="https://i.imgur.com/YNtAQoF.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Locate file and send to VM with ssh:  <br/>
<img src="https://i.imgur.com/PprrkzP.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
<br />
<br />
Use aircrack-ng with dictionary wordlist successfully cracked - “test123!”:  <br/>
<img src="https://i.imgur.com/6pENfVx.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
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
