title: Configure instance to use CITSmart GO application
Description: The application makes possible make attendance in offline mode - in which the attendant does not have an internet.
# Configure instance to use CITSmart GO application


The CITSmart GO application makes possible make attendance in offline mode - in
which the attendant does not have an internet. After the application connects to
the internet, the application will automatically send the information to the
production environment. Remember that the delegation of the request to an
attendant must be carried out manually by the responsible.

The attendant will only see requests that have been delegated to he/she.

Before getting started
--------------------------

1.  Install the application CITSmart GO;

2.  In the environment - CITSmart instance - , configure the following
    functionalities:

    * Webservice: indicate in the item "permissions" the attendance groups that
    can view the tickets;

    * Unit: get the coordinates of the registered unit.

Procedure
-------------

***Webservice***

1.  Access the functionality through the main menu System \> Webservice \>
    Webservice Operation;

2.  On the **Operations Search** tab, search for each of the webservices below,
    then click on "Add Group" and include the group (s) that the attendant (s)
    are linked to:

    * request_add_attachments

    * request_updateRequestList

    * request_userLocation

    * request_saveRequest

    * request_uploadAttachment

    * request_getByUser
    
    * request_saveRequestNote
    
    * request_updateRequestNoteList
    
    * request_updateRequestListGroups
    
    * request_uploadSignature
    
    * parameter_query

1.  Click on "Save" after configure the groups in each webservice.

***Unit***

1.  Access the functionality through the main menu General Registration \>
    Personnel Management \> Unit;

2.  Search for the unit in the tab Search Unit and select the choose;

3.  In the tab Unit Registration with the unit already chosen, click on "Get
    Coordinates";

4.  Click on "Save".

What to do next
-------------------

Log the CITSmart GO application already installed, entering the URL, user and
environment password. Verify the ticket and make the attendance.

Related
-------

[CITSmart GO application manual](/en-us/citsmart-7/additional-features/mobile-and-field-service/apps/citsmart-field-service-manual.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/07/2019 – Anna Martins
