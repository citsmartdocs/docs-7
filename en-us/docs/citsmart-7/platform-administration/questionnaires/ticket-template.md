title: Register ticket template
Description: This feature provides a variety of actions, such as including, changing, and deleting ticket template. 
# Register ticket template

This functionality is intended to enable some functionalities in the service request screen (ticket).
This feature provides a variety of actions, such as including, changing, and deleting ticket template.

Before getting started
--------------------------

The ticket template of type Questionnaire, requires the previous registration of
a questionnaire.

The ticket template of type Neuro, requires the previous registration
of **Neuro** form.

Procedure
-------------

1.  Access the functionality through the main menu System \> Ticket Template;

2.  Click on "New";

3.  The type of template selected will define the fields to completion:

    -   **JSP**: this functionality allows to customize the services screen with
    reference mainly to the management of purchases and travel. Within the JSP
    type there are sub-types previously registered. The utility of this type of
    template is only observed in versions previous to 7.2.3.9. This template
    class should be handled by an analyst who has knowledge of JAVA programming;

    -   **Questionnaire**: even if the "Enable edit questionnaire" option is
    disabled, this edition will be possible when the ticket registration occurs.
    There are two approval functions that can be configured in the service
    request template or flow maintenance screen. As a rule, for the system, only
    the settings made on the flow screen will be valid. The approval function on
    the service request template screen is valid only if linked to the
    registration of a JSP form in the older models of the system. Enabling
    fields, although selected by default, will have their view unavailable at
    the time of ticket creation, this visualization will occur with the
    completion of the registration. At the time of registration of the ticket
    that has a form of the standard type, will be available on the first button
    in the upper left corner, the functionalities: Requester CI, Attachments,
    Agenda, Release, Project, Knowledge and email Reading. All enabling
    functionalities that will be presented both in the service request template
    screen and flow maintenance will be only valid as marks configured in the
    flow screen, because the first one is mentioned is a complement of the
    second one. If the service request template is only linked to the portfolio
    activities, the system will assume that the form is standard, so it will not
    meet the template's enabling (or not enabling) rules. For the
    reclassification rule, where the questionnaire or Neuro service template has
    to be presented for the user response, it's necessary that the template or
    form is linked to the service request template concomitantly with the flow
    maintenance screen and the portfolio activity;  

    -   **Neuro**: when you select this option, the Neuro form link field and Neuro
    page are made available. You can also elect the **version** of the form by
    clicking the "Specific Version" button on the form. The template rules of
    the Questionnaire type are valid for the Neuro type template.

Related
-----------

[Create workflow](/en-us/citsmart-7/workflow/use/create-flow.html)

[Register questionnaire](/en-us/citsmart-7/platform-administration/questionnaires/questionaires-management/register-questionnaire.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/10/2019 – Larissa Lourenço

