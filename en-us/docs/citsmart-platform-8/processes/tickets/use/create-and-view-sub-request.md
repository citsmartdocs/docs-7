title: Create and view sub-ticket
Description: It's possible to create sub-ticket through the main request and view them after created.
# Create and view sub-ticket

This functionality allows to register a ticket with activities related to the original ticket.

Before getting started
--------------------------

It's necessary to previously register the employee, contract and unity. It's
also necessary to link the group to the contract, unit to the contract and
contract to the service.

Register the portfolio with services and activities of request and incident. Set
the time of attendance for the activities of request and incident.

Link the activities of request and incident to the service contract. Set the
parameter 385 with value 'Y'.

Procedure
-------------

1.  Access the functionality Ticket Management through the main menu Processes
    \> Ticket Management \> Ticket;

2.  Click on the ticket you want and select "Create sub-ticket" in the
    options menu;

3.  Complete all mandatory fields and click on "Save'. The sub-ticket will
    be directed to the executor group defined in the activity link registration,
    to the executor group defined in the parameter 9;

4.  Note that the system will send notification e-mail about the creation,
    escalation, capture, close and other changes in the related tickets to the
    executor group of the main ticket.
    
5.  To search for tickets related, it'll be necessary to select the filter "Show related" in ,
    the search area in the main screen of the functionality.


        
!!! Abstract "NOTE"
    
    The sub-ticket has its own flow, therefore, it's not finished along with the
    closure of the origin ticket. It should, then, be executed and closed autonomously.
    
!!! Abstract "NOTE"
    
    The sub-ticket can be reopened at any time, regardless of the status of the parent 
    request (whether it's reopened or closed).

Related
-----------

[Register group](/en-us/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Create ticket](/en-us/citsmart-7/processes/tickets/use/create-ticket.html)

[Register employee](/en-us/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Register unit](/en-us/citsmart-7/platform-administration/region-and-language/register-unit.html)

[Configure access permission of request/incident management](/en-us/citsmart-7/processes/tickets/configuration/access-ticket-management.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RNrJnhiXj3dbmgsm9-quhfz)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/03/2019 – Larissa Lourenço

