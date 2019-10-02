title:  Search ticket in the advanced mode
 
Description: This functionality allows to refine the ticket search through filters.

# Search ticket in the advanced mode
This functionality allows to refine the ticket search through filters.

Before getting started
--------------------------

To make an advanced search of tickets, it's necessary to previously register a
ticket and have opened calls, in any situation and set the parameters: 40, 41,
261, 260 (with the default value 1-List without Restriction), 343 (with default
value "Y") and the parameter 378 (if the user informs the value 0, the system
will always download in background. If the user leaves the field blank, the
system limits the download in the background to five thousand records. If the
user places a value greater or less than five thousand records, the system
considers the value entered by the user).

Procedure
-------------

1.  Access the functionality Ticket Management through the main menu Processes
    \> Request and Incident Management \> Service Request and Incident;

2. Click the menu button located in the upper left corner of the screen and then on "Advanced Search";

3.  Complete the fields with the information you want. Remembering that the
    effectiveness of the search depends on following some rules of permission by
    the filter, for example: execution, delegation, monitoring, visualization,
    user group, contract link, units and employee logged in. Therefore, if
    parameter 61 is enabled, only will be availabe the units linked to the
    contract, to which it has links with the groups in which it belongs to;

4.  Click on "Search";

5.  Choose one of the formats of the file (PDF, XLS and CSV) to generate the
    report. After choose the format, the system verifies the parameter 261 and
    if it find a register greater than the amount allowed, it will present the
    following message:

    -   "The amount of registers found exceed the maximum amount allowed for
        viewing. Please, redefine the search filters";

6.  However, if the amount of registers returned in the search is less than the
    limited in the parameter 261, the system verifies the configuration of
    parameter 378;

7.  It's verified the amount of registers to generate the report in background,
    if the amount is greater than the amount parametrized, than the system will
    present the following message:

    -   "The report is being processed. A notification will be sent to you when
        it's ready"

8.  In case the file to be created is too long, the system triggers a
    notification in the main screen, informing that its download is finished.
    When finished, click on "View" to access the report through the link
    available.

Related
-----------

[Create ticket](/en-us/citsmart-7/processes/tickets/use/create-ticket.html)

[Configure parametrization - ticket](/en-us/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)

[Configure parametrization - system](/en-us/citsmart-7/platform-administration/parameters-list/configure-parametrization-system.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RNrJnhiXj3dbmgsm9-quhfz)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/03/2019 – Larissa Lourenço

