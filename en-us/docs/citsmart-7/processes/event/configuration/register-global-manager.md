title: Register Global manager
Description: 
# Register Global manager

This functionality is intended to create rules to monitor several types of
events.

Each global event manager contains an EPL for *Information*, *Warning*, and/or
*Exception*. EPL is an event correlation language used by Esper (Espertech). In
the initialization of CITSmart Event Monitor, these EPLs are imported into the
Esper engine so that a new correlated event will be created each time the
condition set in the EPL is satisfied. Example of an EPL that correlates between
CITSmart Inventory and Nagios events: \@Description ('For any Nagios event that
occurs after any Inventory event in the last 10 minutes) select \* from pattern
[every a = EventCheckInventory- \> b = EventServiceNagios where timer: within
(10minutes)].

This feature provides a variety of actions, such as including, changing, and
deleting a global manager.

Before getting started
--------------------------

To register the Global manager, it's necessary to previously register the
CITSmart Event Monitor connection, time, occurrence category, automatic action
and the CITSmart Inventory connection.

Procedure
-------------

1.  Access the functionality through the main menu Processes \> Event Management
    \> Global Events Manager;

2.  Complete the fields available in each area:

       - Enter the data of **Action to Information**:

         - Select the action that will be triggered when there is an event of type
           *information*, the degree of urgency and impact. The rules for this action
           are defined using the Event Processing Language (EPL). Click
           the *Validate EPL Information* button to validate the informed EPL.

       - Enter the data of **Action to Warning**:

         - Select the action that will be triggered when there is an event of type
           *warning*, the degree of urgency and impact. The rules for this action are
           defined using the Event Processing Language (EPL). Click on
           the *Validate EPL from Warning* button to validate the informed EPL.

       - Enter the data of **Action to Exception**:

         - Select the action that will be triggered when there is an event
           occurrence of type *exception*, the degree of urgency and impact. The
           rules for this action are defined using the Event Processing Language
           (EPL). Click the *Validate EPL of Exception* button to validate the EPL
           entered.


1.  Click on "Save".

Related
-------

[Register occurrence category](/en-us/citsmart-7/processes/event/configuration/register-occurence-category.html)

[Register Event Monitor Connection](/en-us/citsmart-7/processes/event/configuration/register-event-monitor-connection.html)

[Register time](/en-us/citsmart-7/processes/event/configuration/register-time.html)

[Set Inventory connection](/en-us/citsmart-7/processes/event/configuration/set-inventory-connection.html)

[Register automatic action](/en-us/citsmart-7/additional-features/automation-of-operation/configuration/register-automatic-action.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/04/2019 – Anna Martins
 
