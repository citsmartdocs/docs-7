title: Register service request priority
Description: 
# Register service request priority

The Service Request Priority functionality allows to set the priority matrix to dynamically calculate the attendance time (SLA) of the service request. The priority will be used to identify the relative importance of the service request and to identify the time required for an appropriate action to be taken.

This feature provides a variety of actions, such as including, changing, and deleting a service request priority.

Before getting started
--------------------------

To register a service request priority, it's necessary to set the parameter 104
with value "Y".

Procedure
-------------

1.  Access the functionality Service Request Priority through the main menu
    Processes \> Portfolio and Catalog Management \> Service Request Priority;

2.  Complete all mandatory fields to Impact, click on "Save Impact";

3.  Complete all mandatory fields to Emergency, click on "Save Urgency";

4.  Complete all mandatory fields to the Priority Matrix, click on "Save
    Priority Matrix".

!!! Abstract "RULE"

    Note that after register the priority matrix, when registering a service
    request, the time of attendance (SLA) will be established according to the
    level of impact and urgency entered, being considered the priority matrix.
    Remember that for this to happen, the parameter must be enabled.


Related
-----------

[Configure parametrization - ticket](/en-us/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RPsG8HdkE7qEHB39yEI_T8y)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/03/2019 - Anna Martins
