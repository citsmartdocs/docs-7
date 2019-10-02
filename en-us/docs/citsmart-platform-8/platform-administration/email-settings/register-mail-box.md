title: Register mailbox
Description: This functionality is designed to configure the sending and receiving of email from different servers in order to meet different contracts 
# Register mailbox

This functionality is designed to configure the sending and receiving of email from different servers in order to meet different contracts, so a CITSmart can serve different clients and each one will have its own mailbox. In this case, you can use a send/read email account (e.g.: email@company.com) on an XPTO company contract, and another email account belonging to a different business agreement (e.g.: email@company2.com).

Procedure
-------------

1.  Access the functionality through the main menu Parametrization \> Mailbox;

2.  Click on "New";

3.  Choose the type of box. If you opt for the type "Input" (it means that the
    user will parameterize a route where the emails that need to be read will
    arrive), it will open new registration fields, such as: server, server port,
    user (email address), password, provider and inbox folder, therefore it's
    necessary to fill in the fields;

4.  If you opt for the type "Output" (it means that the user will parameterize a
    route where the emails that need to be sent from the system will exit),
    it'll open new registration fields, such as: server, server port, user,
    password, sender, set whether TSL/SSL authentication is required (both are
    security protocols) and user authentication is therefore necessary to fill
    in the fields;

5.  Click on "Save";

6.  Link the email box to the contract. To do so: access the functionality
    Processes \> Portfolio and Catalog Management \> Contract and link the
    previously registered email box in the "Email" field and click on "Save";

7.  Link the email box to a flow. Therefore:

    -   Access the functionality System \> Flow Maintenance and when
        registering/editing a flow, find in the "Diagram" filed the
        figure figure representing an email in the flow and click on edit;

    -   In the option "Configure outbox email", opened when clicking on the tab
        "Message", select the option "Specific" to use the mailbox configured in
        the contract;

    -   Complete the flow parametrization, including the selected "Recipients";

    -   The use of different email outbox can be noticed after a service request
        is opened, which has parameterized the flow that has the selected
        mailbox.

    -   Click on "Save".
    
!!! Abstract "NOTE"

    Linking to the mailbox is not a required step. This functionality will
    only be necessary when registering the flow, the user feels the need to
    direct the email to an output box different from the default. The system's
    default email outbox will continue to function even if this setting is not
    done.
    
    
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/10/2019 – Larissa Lourenço



