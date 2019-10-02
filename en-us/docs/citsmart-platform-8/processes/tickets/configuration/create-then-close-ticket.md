title: How to create, and then, close the ticket  
Description: configure for the creation and closing of the ticket at the same time. 
# How to create, and then, close the ticket


For activities that do not require an SLA, where the attendant only wishes to
formalize the request and execution of the activity, it's possible to configure
for the creation and closing of the ticket at the same time.

Procedure
-------------

1 - It's possible to define the creation and close flow in two different ways:

*  **1st Way - Import flow**: it's possible to import the flow with script already
registered. Download the attachment "JSON Flow" and access the flow
functionality (Workflow \> Flow Design), click on "New", then click on
"Import" and select the option "JSON". Upload the attachment and click on
"Import". Then, to verify the script, click on the tab "Diagram" and on the task
icon, next, click on "Input Action";

*  **2nd Way - Copy the script**: to copy only the script, copy the attachment
"Script" content and access the functionality flow (Workflow \> Flow Design),
click on "New" and complete the field necessary. Then, click on the tab
"Diagram", design the flow about the creation and closure of a task, select and
click on this task (small gray box next to the task) and in the tab "Input
Action". It's necessary to copy the RhinoScript in the expressions builder and
click on "Build expressions" and select the register expression.

!!! Abstract "NOTE"

    No controls have been implemented for catch information, because the time
    of attendance and closing of the ticket is very short, if it's necessary to
    do the same, it'll be necessary to implement the registration of the
    information in the capture tables.

Attachment
---------
[Download - Fluxo JSON][1]

[Download - Script][2]


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RNemh0QXhtOXntvZ6G6o2B_)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/03/2019 – Anna Martins


[1]:/en-us/citsmart-7/processes/tickets/images/fluxo-JSON.json
[2]:/en-us/citsmart-7/processes/tickets/images/script.zip
