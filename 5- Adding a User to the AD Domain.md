# Description

In this step, I will be adding a Windows user to the Active Directory Domain. However, before that, I made the following configurations on the pfSense web interface.

- Added the Domain Controller as a DNS server on pfSense

![afdaf](https://i.postimg.cc/rpDZGY1H/image.png)

## Adding a Windows 10 User

- Created a Windows 10 VM with the following configurations:
    - Added the Windows 10 VM to vmnet3 (victim network)
    - Removed unnecessary hardware accessories such as sound card
    - Removed the Floppy Disk

![adfafd](https://i.postimg.cc/tRd1CqKr/image.png)

- Renamed the PC with a name that matches the first and last name of the user previously created (John Jacobs).

![adfafd](https://i.postimg.cc/QNPWyYrD/image.png)

- Assigned a static IP (192.168.2.31)
- Changed the default gateway to pfSense (192.168.2.1)
- Changed the DNS server to the Domain Controller (192.168.2.10)

![FDA](https://i.postimg.cc/fb2xTw1t/image.png)

- Joined the Windows VM to the AD Domain

![adfa](https://i.postimg.cc/DZ6RzbnQ/image.png)

> Windows 10 VM is successfully joined to the AD.

![afaf](https://i.postimg.cc/5yxYwDcd/image.png)


 



