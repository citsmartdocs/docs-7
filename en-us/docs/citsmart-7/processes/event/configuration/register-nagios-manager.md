title: Register Nagios manager
Description: Register and maintain the managers that will be responsible for monitor the configuration items and event occurrences captured from the Nagios.
# Register Nagios manager

Nagios is a network monitoring tool. It can monitor both hosts and services,
warning when happening the problems and also when the problems are solved. The
Hosts are equipment and Services are resources offered by the equipment.

The objective of this functionality is register and maintain the managers that
will be responsible for monitor the configuration items and event occurrences
captured from the Nagios. It allows the user to inform when the Manager will be
processed, which configuration items it will manage and the actions to be taken
automatically.

This feature provides a variety of actions, such as including, changing, and
deleting a Nagios manager.

Before getting started
--------------------------

To register Nagios manager, it's necessary to previously register the CITSmart
Event Monitor connection, time, occurrence category, automatic action and the
CITSmart Inventory connection.

Procedure
-------------

1.  Access the functionality through the main menu Processes \> Event Management
    \> Nagios \> Nagios Manager;

2.  Complete the fields available in each area;

3.  In the parent configuration item area, it's possible to register the CI in
    CITSmart with the data of the Host selected. Click on "Create CI". Remember
    that this registry can only be made if there is no CI with the same Host
    identification:

    - Enter the data of the child configuration item;

    - Conduct a relationship between the Host service and the child configuration
    item. Each host service must be related to its respective child
    configuration item.

1.  Click on "Save".

Related
-------

[Register occurrence category](/en-us/citsmart-7/processes/event/configuration/register-occurence-category.html)

[Register Event Monitor Connection](/en-us/citsmart-7/processes/event/configuration/register-event-monitor-connection.html)

[Register Nagios/Zabbix connection](/en-us/citsmart-7/processes/event/configuration/register-nagios-zabbix-connection.html)

[Register time](/en-us/citsmart-7/processes/event/configuration/register-time.html)

[Register automatic action](/en-us/citsmart-7/additional-features/automation-of-operation/configuration/register-automatic-action.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/04/2019 – Anna Martins
