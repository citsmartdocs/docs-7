title: Create workflow
Description: It's possible to create workflows that best fit to the users' reality

# Create workflow

 It's possible to create workflows that best fit to the users' reality, customizing the scenario of each organization.

Procedure
------------

1.  Access the main menu Workflow \> Flow Design;

2.  Click on "New";

3.  In the tab "Flow Data", it's necessary to complete the mandatory data: name 
    (its internal identifier, it must be informed without space, accents and special characters); the process to which it's linked (the flow will be only visible to the process to which it's linked) and the option that allow to reopen the service regardless of group settings. It's also possible to view the version of the flow.

3.  In the “Diagram” tab, it's presented the tool to design the flow by entering
    elements that represent the scenario. To do so, simply click on the element and drag it to the design area. When you do this, a screen will be displayed to set the properties. We must take into account that a flow starts with the "Start Event" element and ends with the "End Event".

    !!! Abstract "IMPORTANT"
    
        The conditional paths of a flow must be defined in the Connection (Sequence Flow). 
        To access these options, click once on the connection and then on the properties icon.
        It's possible to identify the connection (eg. approved) and indicate a Condition, Action or State. [See Build Expression][2].

4.  The properties of an element can be defined by double-clicking the element 
    and then the icon next to it (properties icon). Define the data for this
    property by entering the required data in each of the property tabs. Here it is also liberated to link a knowledge to the "Knowledge Base" tab and implement functionalities in the flow on the activity by clicking on the "Interface" tab;

    !!! Abstract "NOTE"

        The "Interface" tab allows you to choose which interaction mode (form
        standard, questionnaire or neuro form) that will be applied to the service. 
        However, if a service request template is not linked to this tab, the system 
        will sub-understand and apply the configurations of a standard form, enabled 
        configuration item link, change, problem and request related to the ticket in
        ticket management screen.  
        We can also cite another rule referring to this tab: the regulations here
        will have priority over the template service request, as this is a complement 
        to the flow of.  

5.  Besides, the functionality allows to import flows when click on "Import". It'll be
    possible to import in "JSON" or "XML".

6.  After define the flow, click on "Save".

Related
------------

[Register ticket template](/en-us/citsmart-7/platform-administration/questionnaires/ticket-template.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/21/2019 – Larissa Lourenço

[2]:/en-us/citsmart-7/workflow/configuration/expressions-creator.html
