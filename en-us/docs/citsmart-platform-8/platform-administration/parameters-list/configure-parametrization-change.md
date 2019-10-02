title: Configure parametrization - change
Description: Process responsible for evaluating, coordinating and deciding on making proposed changes to the Services and/or Configuration Items (CIs).
# Configure parametrization - change

Change Management is the process responsible for evaluating, coordinating and
deciding on making proposed changes to the Services and/or Configuration Items
(CIs). The parameters to be configured allow to adjust the notification
submission, inform the email templates to escalate the request for change,
inform the name of the application flows and define the type of voting used in
the change advisory board, among other actions.

Procedure
-------------

1.  Access the functionality through the main menu Parametrization \> Change
    Management;

2.  Define the values for the parameters (attributes);

3.  Click on "Save";

4.  The list below presents the parameters of "Change" and their purpose:

|  #  |                                               Name                                              |   Possible Values   |                                                                                                                                                                                     Purpose                                                                                                                                                                                     |                                                       Additional Guidance                                                      |
|:---:|:-----------------------------------------------------------------------------------------------:|:-------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------:|
|  47 |                                  Default flow name for changes                                  | E.g.: RequestChange |                                                                                                                                    Enter the name of the "default" request for change flow. This flow is defined in the "Flow Design" screen.                                                                                                                                   |                                                         Not applicable                                                         |
| 120 |             Email template ID for sending notification to the Change Advisory Board             |       E.g.: 29      |                                     Inform the notification email template (ID) for the Change Advisory Board. The email template defined in this parameter will be used to send the request for change notifications. This notice will be sent to the Change Advisory Board. This email template ID is set on the "Email Template" screen.                                     |             If you do not enter the ID number of the email template, you may not be able to send the correct email.            |
| 122 | ID of the email template that will be sent to the target group when escalating a change request |       E.g.: 30      |                                             Enter the request for change escalation email template identification number (ID). When escalating a request for change, a notification is sent to the target group, according to the template defined in this parameter. This email template ID is set on the "Email Template" screen.                                             |          If you do not enter the identification number (ID) of the email template, you may not send the correct email.         |
| 133 |                   Email template ID for sending scheduled meeting notification                  |       E.g.: 39      |                        Enter the identification number (ID) of the scheduled meeting notification email template. When scheduling a meeting for a request for change on the Change Management screen, an email will be sent to the responsible party, notifying about the meeting schedule. This email template ID is set on the "Email Template" screen.                       |          If you do not enter the identification number (ID) of the email template, you may not send the correct email.         |
| 146 |                                    Questionnaire template ID                                    |       E.g.: 13      |                                                                                                      Enter the identification number (ID) of the template for the checklist for the changes and release. This template ID is set on the "Service Request Template" screen.                                                                                                      |                                                         Not applicable                                                         |
| 193 |   Enable the escalation of changes defined in the escalation rules? (Eg: Y or N - Default 'N')  | Y or N (Default: N) |                                                                                           Define if the escalation of changes determined in the escalation rules will be enabled. This change escalation rule is defined in the "Escalation Rules and Automatic Notifications" screen.                                                                                          |                    If you do not enter the parameter value, the system default value will be set: "N" (No).                    |
| 268 |                        Email template ID to notify when finish the change                       |                     | Enter the identification number (ID) of the email template used to notify the closure of a request for change. When closing a request for change, the "Change Management" screen will be used to send the notification of closure defined in the email template. This notification will be sent to the requester. This email template ID is set on the "Email Template" screen. | If you do not enter the identification number (ID) of the email template, you may not send the correct email to the requester. |
| 279 |                                   Normal flow name for changes                                  |                     |                                                                                                                                     Enter the name of the normal request for change flow. This flow is defined in the "Flow Design" screen.                                                                                                                                     |               If you do not enter the parameter value, an error message appears on the Request for Change screen.              |
| 280 |                                Name of emergency flow for changes                               |                     |                                                                                                                                    Enter the name of the emergency request for change flow. This flow is defined in the "Flow Design" screen.                                                                                                                                   |               If you do not enter the parameter value, an error message appears on the Request for Change screen.              |
| 303 |    RFC voting using the rule of absolute majority (50% + 1) (Values: "Y" or "N" Default: "Y")   | Y or N (Default: Y) |                                                                                                                                     Define which type of voting will be used in the request for change: absolute majority rule or all vote.                                                                                                                                     |                                                         Not applicable                                                         |                                                                                               




Table 1 - Parameters list


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/08/2019 – Anna Martins

