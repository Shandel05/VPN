<p align="center">
<img src="https://i.imgur.com/FO2s0fF.png" alt="Microsoft Active Directory Logo"/>
</p>

<h1>Understanding Virtual Private Networks (VPNs) in Azure</h1>
This lab demonstrates the steps I took to setup, install, and use a free Virtual Private Network (VPN) using Azure. We will be observing some behaviors as we browse the internet. <br />

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- ProtonVPN

<h2>Operating Systems Used </h2>

- Windows 10 Pro (21H2)

<h2>Installation Steps</h2>

<p>
<img src="https://i.imgur.com/W8lQlaT.png" height="80%" width="80%" alt="Installation Steps"/>
</p>
<p>
Before creating a VM, on my actual PC I will browse to www.whatsmyipaddress.com. This will tell me my Public IP address along with ISP name, City, Region and Country. In my case the IPv4: 71.104.19.191, ISP: Verizon Business, City: Ashburn, Region: Virginia, Country: United States</p>
<br />

<p>
<img src="https://i.imgur.com/U1WcM3q.png" height="80%" width="80%" alt="Installation Steps"/>
<img src="https://i.imgur.com/wjBMMhV.png" height="80%" width="80%" alt="Installation Steps"/>
<img src="https://i.imgur.com/GGwUDc2.png" height="80%" width="80%" alt="Installation Steps"/>
</p>
<p>
While creating the VM with azure,I made sure the Location was different from my regular PC so I chose the location for the VM in North Europe. I then log into the remote desk top with the Public IP address from the VM. After I was signed into remote desktop I browsed back to www.whatsmyipaddress.com. This time from my VM remote desktop my IPv4: 20.223.146.120, ISP: Microsoft Corporation, City: Dublin, Region: Dublin, Country: Ireland. Since I created my VM with a location in Europe my IP address has changed from when I browesed from my PC.
</p>
<br />

<p>
<img src="https://i.imgur.com/A58YVeB.png" height="80%" width="80%" alt="Installation Steps"/>
<img src="https://i.imgur.com/vDLXWwQ.png" height="80%" width="80%" alt="Installation Steps"/>
<img src="https://i.imgur.com/EMfNt3X.png" height="80%" width="80%" alt="Installation Steps"/>
</p>
<p>
After retrieving my IP address from browsing on my remote desktop, I then installed ProtonVPN within my remote desktop, the dedicated VPN solution that provides secure, unrestricted, high-speed access to the internet. I connected the VPN to a Japan server and browsed one last time to www.whatmyipaddress.com. This time my VM remote desktop that is connected to ProtonVPN sever out of Japan give me a IPv4: 138.199.21.201, ISP: DataCamp Limited, City: Tokyo, Region: Tokyo, Country: Japan.
</p>
<br />

<h2>An Important Note </h2>

Since VPNs can securely link two computers (or networks) together across an insecure network such as the internet, yo can see how my IPv4 has changed 3 different times. A good way to think of VPNs is the link to be able to connect and access resources at work from your home.
