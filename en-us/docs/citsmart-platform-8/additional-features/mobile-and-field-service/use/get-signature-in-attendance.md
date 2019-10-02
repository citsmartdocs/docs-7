title: Get signature in field service
Description: This document aims to explain the configuration of CITSmart mobile to receive digital signature in field service.
# Get signature in field service

This document aims to explain the configuration of CITSmart mobile (Experience and GO) so that the
technician receives the digital signature of a validator in field service.

Before getting started
----------------------

It's necessary to previously install the CITSmart mobile. In order for the field technician to see tickets only assigned to
him/her in the request list, the attendant/manager must set the parameter 435 to "Yes".

Procedure
---------

***In CITSmart***

1.  Access the main menu Processes \> Portfolio and Catalog Management \>
    Portfolio;

2.  Search for the portfolio and click on "Advance";

3.  Select the service and click on "Advance";

4.  Click on the tab **Contract**;

5.  Select the contract and click on "Advance";

6.  Click on the tab **Requests**;

7.  Select the activity and click on "Edit";

8.  Configure the option "Yes" the field *Requires signature on Mobile*;

9.  Click on "Save".

***In mobile***

1.  When capture a ticket (using mobile), the technician must complete the
    fields available and, when put the ticket with the status "Solved", the
    field **Signatures** will be enabled so it'll be posible to put the *Number
    of the register*, *Name* and *Signature* of the validator in field. This
    signature will be done with the finger in the mobile screen;

2.  Click on "Options" and then on "Save and advance flow";

3.  The ticket will not appear anymore in the technician list;

4.  The attendant / administrator will only see the request answered by the technician, when searching for the same in the *advanced search* (side menu of the ticket listing screen) and when you open you can see the signature also collected.

Related
------

[Mobile CITSmart Experience application manual](/en-us/citsmart-7/additional-features/mobile-and-field-service/apps/citsmart-app.html)

[Configure mobile options](/en-us/citsmart-7/additional-features/mobile-and-field-service/configuration/configure-mobile-options.html)

[Configure parametrization - ticket](/en-us/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)

[CITSmart GO application manual](/en-us/citsmart-7/additional-features/mobile-and-field-service/apps/citsmart-field-service-manual.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/20/2019 – Anna Martins
