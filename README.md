# Install and Test VPN Functionality
The purpose of this lab is to test and observe virtual private network (VPN) functionality on a Windows 10 virtual machine.

<h2>Prerequisites</h2>

- Create a Windows 10 VM.
- Register for a Proton VPN account, choose free account option (https://protonvpn.com/).

<h2>Actions and Observations</h2>

![0](https://github.com/melisa-er/Install-and-Test-VPN-Functionality/assets/157723219/d727dc6d-0223-4e03-9598-17e9fb6efb34)

When creating the Windows 10 VM, choose a region that is different from your current location.

#
![1](https://github.com/melisa-er/Install-and-Test-VPN-Functionality/assets/157723219/3bed8816-d1a3-4b8e-a88a-7adbd24c102e)

On your host computer, go to whatismyipaddress.com to check the public IP address used by your computer, as well as the location.

This public IP address is the one used by your ISP.

The location indicated may not be your exact location depending on the quality of ISP package you are subscribed to. Higher quality service has more accurate location compared to lower quality services.

#
![2](https://github.com/melisa-er/Install-and-Test-VPN-Functionality/assets/157723219/c2998509-4c39-48e5-b1ca-f4455369bc63)

Connect to the Windows 10 VM through RDP and visit the same site from above to check the IP address and location of your VM.

The location should be the same as the VM location you chose when setting up the VM in Azure.

#
![3](https://github.com/melisa-er/Install-and-Test-VPN-Functionality/assets/157723219/38d1e7ae-b5f7-4a13-baaf-8460633a75b3)

While still on the VM, install Proton VPN for Windows (protonvpn.com/download) and sign in using the account you registered during the lab prerequisites.

#
![4](https://github.com/melisa-er/Install-and-Test-VPN-Functionality/assets/157723219/bb785d05-fe83-4597-b792-1c180606e680)

Here is the interface of the Proton VPN application. On the right-hand side are the servers you can connect to using the free account. 

For this lab, we will be connecting to a VPN server in Japan – select “Connect” (it doesn’t show in the screenshot, but the connect option is visible when you hover your curser over the Japan option).

#
![5](https://github.com/melisa-er/Install-and-Test-VPN-Functionality/assets/157723219/4fe3c3e4-463b-45c7-8fef-992abe28a3d1)

You can see the connection being made.

#
![6](https://github.com/melisa-er/Install-and-Test-VPN-Functionality/assets/157723219/4549e74b-badf-4324-8495-84b04b2ac813)

The RDP connection may momentarily disconnect as the VPN connection is being established. It should reconnect on its own.

#
![7](https://github.com/melisa-er/Install-and-Test-VPN-Functionality/assets/157723219/8f7a58d0-009a-4738-abae-764b56474ad0)

The VPN has connected!

#
![8](https://github.com/melisa-er/Install-and-Test-VPN-Functionality/assets/157723219/8cdfb4b7-af94-49e2-9038-2cb01573d801)

Going back to whatismyipaddress.com, refresh the page to see the new IP address and location information.

NOTE: you may need to clear the browser history + cookies to get the true location if you keep getting random locations that are not Japan. Proton has change the functionality of their free VPN tier as of this lab.

#
![9](https://github.com/melisa-er/Install-and-Test-VPN-Functionality/assets/157723219/5dbe9cad-e45f-4a42-a8ef-73bc9b76fbee)

Going to google.com on the VM with the VPN connection takes us to the Google Japan page.
