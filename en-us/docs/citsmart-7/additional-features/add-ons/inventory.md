Title: Implementing CITSmart Inventory

# Implementing CITSmart Inventory

CITSmart Inventory is a component of the CITSmart that enables you to collect, register and manage information from IT assets. It enables you to manage the lifecycle of your organization's configuration items from the Configuration Management process.  

![Architecture INV and EVM](images/cloud-arch-inv-evm.png)

## Before getting started

CITSmart Inventory works in conjunction with [CITSmart Event Monitor - EVM][1] and as a data collector (eg XML packages) and EVM serves as a repositories for this information. Therefore, to enable Inventory, you must first configure EVM.  


## Procedure

1. [Install][2] the Wildfly application server;
2. Download the WAR package from the EVM component;  
3. Unpack the files;  
4. Copy the package to the deployment folder of the Wildfly application server;  
5. Configure [System Properties][3] with data of CITSmart instance;

## What to do next

To test the Inventory, [configure][4] the connections in the CITSmart instance.

## Related

[Implement CITSmart Event Monitor][5]

[Asset and Configuration Management][6]


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/22/2019


[1]:/en-us/citsmart-7/additional-features/add-ons/event-monitor.html
[2]:/en-us/citsmart-7/get-started/installation-and-upgrade/perform-installation.html
[3]:/en-us/citsmart-7/get-started/installation-and-upgrade/perform-installation.html#configure-system-properties
[4]:/en-us/citsmart-7/processes/event/configuration/set-inventory-connection.html
[5]:/en-us/citsmart-7/additional-features/add-ons/event-monitor.html
[6]:/en-us/citsmart-7/processes/configuration/overview.html
