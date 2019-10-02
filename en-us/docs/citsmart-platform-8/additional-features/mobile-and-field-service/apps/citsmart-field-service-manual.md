title: CITSmart GO application manual
Description: The purpose of the CITSmart GO application is to make offline technical attendance (when the attendant has no connection).
# CITSmart GO application manual

The purpose of the CITSmart GO application is to make offline technical attendance (when the attendant has no connection).

Before getting started
--------------------------

1.  Have configured the application in the ITSM instance;

2.  Install the CITSmart GO application in the mobile (Android and iOS);

3.  It's necessary to delegate technical tasks in the CITSmart website so it'll
    be possible to field attendance in offline.

Procedure
-------------

!!! Abstract "NOTE"

    When logging into the CITSmart GO application, the first synchronization can take 
    a few moments, because to work offline, you have to download all the requests and 
    send the ones that have changed, so that the application works correctly.

1.  Enter the login data of the application;

2.  Select and click on the ticket you want. It'll be presented a screen with
    the request data, including the location map where it'll make the
    attendance;

3.  Click on "Execute request" and then on "Other data" (this option will
    be only available if exists a questionnaire linked to the ticket activity).
    Complete the data about the request execution and  click on "Save";
    
    !!! Abstract "NOTE"
    
        Only simple components of Neuro, for example, forms, can be rendered in the Mobile GO.
        These forms cannot have any JavaScript logic linked to them, they should be similar to 
        the existing questionnaire in CITSmart SM.
        
    !!! Abstract "RULE"
    
        It's not possible to link a CI and a knowledge base through the GO mobile.
    
4.  If you want to add some file, click on the tab "Attachments";

5.  Click on "Notes" and report the occurrence referring to the ticket and the date that it happened. It's also possible to save the         time taken to solve the problem. It's available the visualization of this report by the requester and the sending of the same to         his/her email by selecting the options "Visible to the requester" and "Send to e-mail". Click on "Save";

6.  Click on "Finish" and complete the data about the attendance conclusion.
    Select the attendance status (in progress, solved or canceled) and detail
    it;

7.  Click on "Collect Signature and Foward Flow" (see related document) or "Save and keep current task" to complete
    the operation. It'll be automatically synchronized the changes. If the
    application does not find network to complete the synchronization, it'll be
    presented the icon "Automatic update" to wait for a connection and complete the
    synchronization;

8.  Manual synchronization of requests is available as soon as the application
    finds an accessible network. To do so, simply slide the screen down with
    your finger or click on the icon "Update list";

9.  There are filters that make easier to find the required ticket, access it
    through the search box, or click on the icon "Filters".

Related
-------------  

[Configure instance to use CITSmart GO application](/en-us/citsmart-7/additional-features/mobile-and-field-service/configuration/configure-field-service-application.html)

[Get signature in field service](/en-us/citsmart-7/additional-features/mobile-and-field-service/use/get-signature-in-attendance.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/07/2019 – Anna Martins
    

