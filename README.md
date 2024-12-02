# Building a Cybersecurity Homelab for Monitoring and Detection
## Description
In cybersecurity, applying and implementing security concepts can be a challenging task without access to practical and secure infrastructure for testing and experimentation.

This project addresses that challenge by documenting the process of configuring, optimizing, and securing an IT infrastructure within a home lab environment. While the setup is on a smaller scale, the insights and techniques learned from this experience are directly applicable to real-world, large-scale, or enterprise-level infrastructures.

## Topology
The network topology is as follows:

![ad](https://static.wixstatic.com/media/1f97f7_c3819a585fb44cc896e93c99d512ba1a~mv2.jpg/v1/fill/w_740,h_496,al_c,q_90/1f97f7_c3819a585fb44cc896e93c99d512ba1a~mv2.webp)

### Topology explanation

- **Kali Machine:** The Kali Linux VM is going to be used as the attacker machine used to launch attacks against the network.
- **Security Onion:** Security Onion is going to be the IDS/IPS/ for this lab. Kibana will also be used.  
- **pfSense:** pfSense is used as the firewall, router, DHCP server, and network segmentator. It ensures that all the network components are up and running.
- **Victim Network:** The victim network features a Domain Controller and two Windows desktops.
- **Splunk:** Splunk is going to act as the SIEM for the network.

