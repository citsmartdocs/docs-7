title: Report about cost of unavailability of a service
Description: Is intended to verify the report that demonstrates the cost per hour of unavailability of a service
# Report about cost of unavailability of a service

This document is intended to verify the report that demonstrates the cost per hour of unavailability of a service, where:

•	Time Available: time (within the working day) that incidents of the service became available in the period;

•	Time of Unavailability: time in hours (within the working day) that service incidents became unavailable during the period;

•	Number of breakdowns: number of service incidents;

•	MTBSI = Time available / Nº of breakdowns;

•	MTBF = (Time available - Time of unavailability) / Nº of Breakdowns;

•	MTRS = Time of Unavailability / Nº of breakdowns.

Before getting started
--------------------------

In a service portfolio, a service must have the attribute **Incident** with the
field "Cause of unavailability" set as "YES".

In the attribute **Contract** of a service chose, the incident must be linked,
as well as define the Cost of Unavailability, Availability Agreement and also
link the Calendar.

The report available in the attachment should be imported in the Smart Report
Creator.

Procedure
-------------

*Step 1*

1.  Access Reports \> Smart Reports \> Smart Report Creator;

2.  Click on "Import";

3.  Select the file available (attachment) and click on "Open";

4.  In the reports list page, click on "Edit" of the report imported;

5.  Select the option *None* in the field **Module(s) where it will be
    displayed** and define the group(s);

6.  Click on "Save".

*Step 2*

1.  Access the main menu Processes \> Portfolio and Catalog Management \>
    Portfolio;

2.  Choose the portfolio you want and click on "Advance";

3.  Choose the service you want and click on "Advance";

4.  Click on the attribut **Incidents**, then on "New Incident" (the field "Type
    of Demand" must be Incident, as well as the field "Cause Unavailability"
    must be "YES");

5.  Click on "Save";

6.  Click on "Link Incident" and link the incident previously created.

*Step 3*

1.  Click on the attribute **Contracts** of the service;

2.  Select a contract and click on "Advance";

3.  Click on the attribute **Incidents** of the contract and then on "Link
    Incident";

4.  Complete the fields available adding the incident created previously;

5.  Click on "Save";

6.  Click on the attribute **Cost of Unavailability**, define the value and
    click on "Save";

7.  Click on the attribute **Availability Agreement**, click on "Link
    Availability Agreement" and define a SLA;

8.  Click on the attribute **Calendar**, click on "Link Calendar" and define a
    calendar.

What to do next
-------------------

Access the management panel in Smart Portal, add the previously imported report,
define the dates and check the report.

The report can also be viewed in Smart Reports.

Related
-----------

[Register a service](/en-us/citsmart-7/processes/portfolio-and-catalog/use/register-a-service.html)

[Configure service attributes](/en-us/citsmart-7/processes/portfolio-and-catalog/use/configure-services-attributes.html)

[Configure service contract attributes](/en-us/citsmart-7/processes/portfolio-and-catalog/use/service-contract-attributes.html)

[Create the portfolio](/en-us/citsmart-7/processes/portfolio-and-catalog/use/create-the-portfolio.html)

[Service level requirement](/en-us/citsmart-7/processes/service-level/use/service-level-requirement.html)

[Customize management panel (Smart Decision)](/en-us/citsmart-7/additional-features/reports/create/dashboard-customize-management-panel-smart-decision.html)

[Emit report using Smart Report](/en-us/citsmart-7/additional-features/reports/create/smart-reports/configuration/create-smart-report.html)

[Build and maintain smart reports](/en-us/citsmart-7/additional-features/reports/create/smart-reports/configuration/build-maintain-smart-report.html)


Attachment
---------

[Download-Reliability][1]

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/10/2019 – Larissa Lourenço

[1]:/en-us/citsmart-7/additional-features/reports/use/images/reliability.citreport
