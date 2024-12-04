# Description
In this part of the project, I downloaded Security Onion which served as the intrusion detection system (IDS), intrusion prevention system (IPS), and log monitoring system. 

## Step 1: Creating the Security Onion VM

- Downloaded the latest Security Onion .iso image and configured it with the following settings:
    - OS: Linux
    - Version of OS: CentOS 7 64-bit
    - Storage: 250 GB
    - RAM: 12 GB
    - Two extra network adapters one of them was mapped to vmnet4 which will be connecting to pfSense. The second network adapter was mapped to vmnet5 which will be the spam port.

        ![adf](https://i.postimg.cc/vBn58BcH/image.png)

## Step 2: Security Onion Setup

In this step, I set up the virtual machine and completed its configuration. The configurations I set up are as follows:
> NOTE: "so-allow" was not enabled during the initial configuration. It will be enabled later on.

- Username and password
- Instal type: EVAL
- Set up an FQDN (seconion)
- Set up an MIC
- Enabled DHCP
- Enabled direct connectivity to the internet
- Enabled services such as Grafana, osquery, Wazuh, TheHive, Playbook, and Strelka
- Created an e-mail and password
- Enabled NTP services

> The web access URL is https://192.168.183.133

![adf](https://i.postimg.cc/J0YHC6XJ/image.png)

### Step 2.5: Setup an Ubuntu VM and Turn on "so-allow"

In this step, I set up an Ubuntu VM. The Ubuntu VM will be used to access the Security Onion web interface, simulating a SOC Analyst accessing a SIEM or any other tool from their device. 

![dadf](https://i.postimg.cc/9QbdLp8d/image.png)

I also turned on "so-allow" on the Security Onion VM in order to gain access to the web interface. 

> So-allow is a program that allows you to add firewall rules to allow connections from a new IP address. The IP address that was allowed in this case was 192.168.183.134 (the Ubuntu Desktop's IP address).

![FDA](https://i.postimg.cc/jdFKy0KP/image.png)

- Accessed Security Onion through the web interface on the Ubuntu VM.

![jit](https://i.postimg.cc/TPc4qgmF/image.png)



 








