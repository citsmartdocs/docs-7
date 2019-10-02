title: Notification through delegated email ticket
Description: Implement the way of sending email from a delegated ticket, so the delegated tickets will have an email template to send to the technician. 
# Notification through delegated email ticket

This document allows to implement the way of sending email from a delegated ticket, 
so the delegated tickets will have an email template to send to the technician.

Before getting started
--------------------------

An email template must have been previously registered and, the keys to be used
in your body of text, should be the following:

```html
${IDSERVICEREQUEST}

${SERVICENAME}

${REQUESTERNAME}

${DESCRIPTION}
```

Procedure
-------------

1.  Access the functionality through the main menu Processes \> Portfolio and
    Catalog Management \> Portfolio;

2.  Choose a portfolio and click on "Advance";

3.  Choose a service and click on "Advance";

4.  Click on *Contracts*;

5.  Select the contract and click on "Advance";

6.  Click on the tab *Requests* and click on "Edit";

7.  Choose the activity;

8.  In the field **Email Template Delegation** choose by the previously
    registered e-mail template;

9.  Click on "Save".

10.  In the parametrization screen, enable the parameters 438 (informe email
    template for delegation) and 439 (option "YES");
    
11.  In the group registration screen, in the field "Employees", select the checkbox
    "Email" for the people that will receive the email of that group.
    

What to do next
---------------

Access a ticket and delegate it.

Related
-------

[Delegate ticket](/en-us/citsmart-7/processes/tickets/use/delegate-ticket.html)

[Configure email template](/en-us/citsmart-7/platform-administration/email-settings/email-templates-configure-email-template.html)

[Register group](/en-us/citsmart-7/initial-settings/access-settings/user/register-groups.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RNemh0QXhtOXntvZ6G6o2B_)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/03/2019 – Anna Martins
