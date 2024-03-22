# Install and Test VPN Functionality

<h3>Purpose</h3>

- Install and test the functionality of a Virtual Private Network (VPN) on an Azure virtual machines.

<h3>Prerequisites</h3>

- Create a Windows 10 VM.
- Register for a Proton VPN account, choose free account option (https://protonvpn.com/).

<h2>Actions and Observations</h2>

<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vpn-functionality-images/main/0.png"/>

When creating the Windows 10 VM, choose a region that is different from your current location.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vpn-functionality-images/main/1.png"/>

On your host computer, go to whatismyipaddress.com to check the public IP address used by your computer, as well as the location.

This public IP address is the one used by your ISP.

The location indicated may not be your exact location depending on the quality of ISP package you are subscribed to. Higher quality service has more accurate location compared to lower quality services.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vpn-functionality-images/main/2.png"/>

Connect to the Windows 10 VM through RDP and visit the same site from above to check the IP address and location of your VM.

The location should be the same as the VM location you chose when setting up the VM in Azure.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vpn-functionality-images/main/3.png"/>

While still on the VM, install Proton VPN for Windows (protonvpn.com/download) and sign in using the account you registered during the lab prerequisites.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vpn-functionality-images/main/4.png"/>

Here is the interface of the Proton VPN application. On the right-hand side are the servers you can connect to using the free account. 

For this lab, we will be connecting to a VPN server in Japan – select “Connect” (it doesn’t show in the screenshot, but the connect option is visible when you hover your curser over the Japan option).

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vpn-functionality-images/main/5.png"/>

You can see the connection being made.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vpn-functionality-images/main/6.png"/>

The RDP connection may momentarily disconnect as the VPN connection is being established. It should reconnect on its own.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vpn-functionality-images/main/7.png"/>

The VPN has connected!

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vpn-functionality-images/main/8.png"/>

Going back to whatismyipaddress.com, refresh the page to see the new IP address and location information.

NOTE: you may need to clear the browser history + cookies to get the true location if you keep getting random locations that are not Japan. Proton has change the functionality of their free VPN tier as of this lab.

#
<img src="https://raw.githubusercontent.com/melisaaaaaaaaa-er/vpn-functionality-images/main/9.png"/>

Going to google.com on the VM with the VPN connection takes us to the Google Japan page.
