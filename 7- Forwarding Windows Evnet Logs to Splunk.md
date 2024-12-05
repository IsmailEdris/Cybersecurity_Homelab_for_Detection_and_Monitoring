# Description
In this section of the lab, I will be configuring Windows to send logs to Splunk. Splunk's widely known Universal Forwarder will be used to gain log information from the remote Windows machines. 

## Step 1: Enabling the Receiving Port on Splunk

In this step, I enabled receiving on Splunk. Enabling receiving gives Splunk the ability to allow logs to come into its server. 

> Splunk listens for receivers on the port of your choosing. The default is 9997 which was used in this lab.

![adf](https://i.postimg.cc/Qx2nfQbt/image.png)

## Step 2: Creating an Index 

In this step, I created an index on Splunk. Indexes are blocks of storage where logs are stored. You can use "search heads" to search for data within the index. 

- Created an index called "wineventlog" to store Windows event logs from the Domain Controller.

![afdas](https://i.postimg.cc/XJBsKXCF/image.png)

## Step 3: Downloading the Splunk Universal Forwarder on the Windows Domain Controller

In this step, I downloaded the Splunk Universal Forwarder on the Windows Domain Controller so the Windows DC can send log events to Splunk. 

- Configured Splunk Universal Forwarder to forward logs to 192.168.183.136 (Splunk server) on port 8089

![adfaf](https://i.postimg.cc/WzCQ7MdG/image.png)

## Step 4: Connecting the Domain Controller to Splunk

In this step, I connected the Domain Controller to Splunk via the Splunk web interface on the Ubuntu Server. This allows the Domain Controller to send logs to the Splunk Server for analysis and monitoring. 

The types of logs that the Domain Controller will be sending to Splunk is as follows:
- Application Logs
- ForwardedEvents Logs
- Security Logs
- Setup Logs
- System Logs

I also configured the logs to be forwarded to the "wineventlog" index, ensuring that all logs are centralized and consolidated in a single location for streamlined management and analysis.

![adfaf](https://i.postimg.cc/KcfVvhQP/image.png)



