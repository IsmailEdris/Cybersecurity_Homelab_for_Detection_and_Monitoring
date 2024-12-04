# Descripton
In this part of the lab, I will be setting up an Active Directory for security monitoring. The AD domain will be set up with a Windows 2019 Server as the Domain Controller and 2 Windows 10 machines. 

## Step 1: Downloading and configuring Windows 2019 Server
In this step, I will be downloading the .iso disc image of the 2019 Windows Server and will be doing basic configuration on it. 

- Downloaded the .iso image from [microsoft.com](https://www.microsoft.com/en-us/evalcenter/evaluate-windows-server-2019)

![af](https://i.postimg.cc/ZKMBdB0c/image.png)

- Removed the Floppy Desk for a smoother start-up.
- Changed the PC name to "HomeLab-DC" indicating that this PC will be used as the Domain Controller.

![adf](https://i.postimg.cc/zvRCLC59/image.png)

## Step 2: Configuring the AD 
In this step, I will be setting up server roles such as Active Directory Domain Services (AD DS), Active Directory Certificate Services (AD CS), and adding users to the domain. 

## Creating Server Roles
- Created an AD DS server role to mimick a corporate environment and to learn about directory services. The AD DS was also promoted to a Domain Controller (DC) 

![afd](https://i.postimg.cc/yNdv1Sgz/image.png)

- Created a new forest with the root domain name "HomeLab.local"

![adfa](https://i.postimg.cc/2yF4Fzbw/image.png)

- Created an AD CS server role to simulate an enterprise environment. 

- Configured the AD CS to be valid for 99 years.
  > This is not considered best practice. It was only for the simplicity of this lab.

![afdaf](https://i.postimg.cc/RVWSHgk3/image.png)

## Adding Users

- Added a user with the username john.jacob

![adffd](https://i.postimg.cc/25GRJvpR/image.png)

- Added a second user with the username caleb.smith

![adfa](https://i.postimg.cc/pTgHYvbp/image.png)

## Turning Windows Firewall Off

In this step, I turned the Windows Firewall off. 

> NOTE: This is not considered best practice. You should always have your firewall on. This was only done to make weak configurations for educational purposes.

## Assigning a Default Gateway to the DC

In this step, I will be assigning a static IP address to the DC and changing the default gateway to pfSense (192.168.2.1).

> The pfSense firewall will also act as the DNS server.

![adfaf](https://i.postimg.cc/DZ36qpp7/image.png)

