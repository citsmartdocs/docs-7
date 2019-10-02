title: Configure approval request via email
Description: Intended to approve or reject the ticket request through email, without the need of the manager being logged.
# Configure approval request via email
This functionality is intended to approve or reject the ticket request through email, without the need of the manager being logged.

Before getting started
--------------------------

In order to configure the email in the ticket, it's necessary to pre-register
the user, the group and configure parameters 33 and 370 according to the
guidelines of the system-related parametrization rules. It's also necessary to
know how to design the request approval flow via email registered. In this flow,
there should be the "Approval" task and the design for sending the email,
registering the template with the "Waiting Approval" template attached, and
the e-mail server must be configured with all the parameters for email
parameterization rules.

!!! Abstract "ATTENTION"

    Ticket approval via email is only possible with the following browsers configured as default: Mozilla Firefox, Google Chrome, and Microsoft Edge from version 42.17134.1.0.

Procedure
-------------

1.  Access the functionality through the main menu Workflow \> Flow Design;

2.  Select the request approval flow and click on "Edit";

3.  Click on the **Diagram** tab;

4.  In the request approval flow, click on the connector "Send Message - email" icon and then on the small gray box next to the connector to configure it;

5.  Register, in the **Identification** tab, the name and email template to be
    used;

6.  Configure, in the **Recipient** tab, the type of recipients (group/user) of
    the email to be sent (the system don't search the recipients via
    "Expression").

## Configure the email approval notification

1.  Access the functionality through the menu System \> Settings \> Email
    template;

2.  Paste the email template available in HTML in attachment, in the Text field
    and verify the following guidelines:

    - href="{TOKEN(serviceRequestIncident, \${IDSERVICEREQUEST}, VIEW, 50)};

    - serviceRequestIncident = Interface directing: this field cannot be changed
    by the user;

    - \${IDSERVICEREQUEST} = Key to increment the number of the service
    request: this field cannot be changed by the user;

    - VIEW - calls the command to open the request: this field cannot be changed
    by the user;

    - MM (50) - Token expiration time in Minutes: this field can be changed by the user;

1.  Click on "Save".

Related
-------

[Register group](/en-us/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Register user](/en-us/citsmart-7/initial-settings/access-settings/user/users.html)

[Workflow](/en-us/citsmart-7/workflow/overview.html)

[Configure parametrization – email](/en-us/citsmart-7/platform-administration/parameters-list/configure-parametrization-email.html)

[Configure parametrization - system](/en-us/citsmart-7/platform-administration/parameters-list/configure-parametrization-system.html)


Attachment
----------
[Download - Approval][1]


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RNemh0QXhtOXntvZ6G6o2B_)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/07/2019 – Anna Martins


[1]:/en-us/citsmart-7/processes/tickets/images/Approval.docx
