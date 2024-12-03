# Description
**pfSense** will be the primary firewall used to segment our private home lab network. It will only be accessible from our Kali Linux machine. 

## pfSense VM Configuration on VMWare

In this step, the pfSense VM was configured to meet the needs for the network on VMWare

The pfSense VM was set up with the following configurations on VMWare:

- 2 GB of RAM
- 20 GB of storage
- 1 processor
- 6 network adapters (one for each of the other devices that we will be connecting to pfSense)

![ladjf](https://i.postimg.cc/28jYd00T/image.png)

## pfSense Configuration 

In this step, the pfSense VM was configured to meet the needs for the network within the VM itself. 

- Created 4 additional network interfaces inside the pfSense VM mirroring the configuration on VMWare. (pfSense automatically comes with 2 network interfaces)
![dasf](https://i.postimg.cc/j5R3VFwF/image.png)

- Assigned static IP addresses to the LAN and the additional network interfaces that were added. "OPT3" was not assigned any IP address because it is going to have the spam port with traffic that Security Onion is going to be monitoring from our victim network.
> The IP address 192.168.1.1 is going to be used to access the pfSense WebGUI via the Kali Linux machine.

![fj](https://i.postimg.cc/C5G2nnBz/image.png)

> pfSense network configuration

![adf](https://i.postimg.cc/sxr6zf6y/image.png)
