title: Register Zabbix manager
Description: Register and maintain the managers responsible for monitoring the configuration items whose status will be queried in Zabbix.
# Register Zabbix manager

Zabbix is a tool to monitor networks, serves and services, designed to monitor
the availability, user experience and service quality.

The purpose of this feature is to register and maintain the managers responsible
for monitoring the configuration items whose status will be queried in Zabbix.
It allows the user to associate the configuration items to their respective
triggers and to the actions that must be taken in the occurrence of events.

This feature provides a variety of actions, such as including, changing, and
deleting a Zabbix manager.

Before getting started
--------------------------

To register the Zabbix manager, it's necessary to previously register the
CITSmart Event Monitor connection, time, occurrence category, automatic action
and CITSmart Inventory connection.

Procedure
-------------

1.  Access the functionality through the main menu Processes \> Event Management
    \> Zabbix \> Zabbix Manager;

2.  Complete the fields available in each area;

3.  In the parent configuration item area, it's possible to register the CI in
    CITSmart, with the data of the Host selected. Click on "Create CI". Remember
    that this registration will only be possible if there is no CI with the same
    Host identification:

    - Enter the data of the child configuration item;

    - Conduct a relationship between the Host service and the child configuration
    item. Each host service must be related to its respective child
    configuration item.

1.  Click on "Save".

Related
-------

[Register occurrence category](/en-us/citsmart-7/processes/event/configuration/register-occurence-category.html)

[Register Event Monitor Connection](/en-us/citsmart-7/processes/event/configuration/register-event-monitor-connection.html)

[Register time](/en-us/citsmart-7/processes/event/configuration/register-time.html)

[Set Inventory connection](/en-us/citsmart-7/processes/event/configuration/set-inventory-connection.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/04/2019 – Anna Martins
