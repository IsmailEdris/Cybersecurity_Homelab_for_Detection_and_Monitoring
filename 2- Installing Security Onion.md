# Description
In this part of the project, I downloaded Security Onion which served as the intrusion detection system (IDS) and intrusion prevention system (IPS).

## Step 1: Creating the Security Onion VM

- Downloaded the latest Security Onion .iso image and configured it with the following settings:
    - OS: Linux
    - Version of OS: CentOS 7 64-bit
    - Storage: 250 GB
    - RAM: 12 GB
    - Two extra network adapters one of them was mapped to vmnet4 which will be connecting to pfSense. The second network adapter was mapped to vmnet5 which will be the spam port.

        ![adf](https://i.postimg.cc/vBn58BcH/image.png)


