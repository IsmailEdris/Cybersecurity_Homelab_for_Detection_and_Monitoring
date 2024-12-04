# Description
In this step, I will be configuring pfSense & firewall rules on the pfSense firewall.

# Step 1: Configured pfSense 
In this step, I logged into pfSense via the web interface on the Kali machine.

> Google's DNS server (8.8.8.8) was used as the DNS

![fdaf](https://i.postimg.cc/sfW1XpL9/image.png)



## Step 2: Changing the interface names

In this step, I changed the interface names to match the network. The following changes were made:

- OPT1 -> VictimNetwork
- OPT2 -> SecOnion
- OPT3 -> SpanPort
- OPT4 -> Splunk

![of](https://github.com/user-attachments/assets/6e5cf803-0201-49b6-a13d-c8c67c129946)

## Step 3: Configured bridges and firewall rules

- Created a bridge between the "victim network" and the "span port" to connect the networks together.

![adf](https://github.com/user-attachments/assets/a779c7d4-15a7-41cf-90ce-8ba513cdf928)

- Created a firewall that allows any TCP traffic to analyze incoming and outgoing traffic patterns, study potential attack vectors, and test the effectiveness of security measures in a controlled and isolated environment.

![adf](https://i.postimg.cc/XYg6DvzC/image.png)




