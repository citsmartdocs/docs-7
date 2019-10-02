title: Configure parametrization - problem
Description: Allow the execution/use of this process, it may be possible to define the default flow name for the problem, to define whether the responsible party and the executing group will be notified when the time to workaround the problem has expired , among other viable actions.
# Configure parametrization - problem


Problem management manages the lifecycle of all problems from the first
identification, through to investigation, documentation and eventual removal.
The "Problem" parametrization must be made to allow the execution/use of this
process, it may be possible to define the default flow name for the problem, to
define whether the responsible party and the executing group will be notified
when the time to workaround the problem has expired , among other viable
actions.

Procedure
--------

1.  Access the functionality through the main menu Parametrization \> Problem
    Management;

2.  Define the parameters value (attributes);

3.  Click on "Save";

4.  The list below presents the "Problem" parameters and the purpose of each one
    of them:


|  #  |                                                                       Name                                                                       |    Possible Values   |                                                                                                                                                                                                 Purpose                                                                                                                                                                                                 |                                              Additional Guidance                                              |
|:---:|:------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------:|
| 123 |                                                           Default flow name for problem                                                          | E.g.: DefaultProblem |                                                                                              Enter default flow name for Problem. If no flow is informed to the problem, the flow will be established by the system (as reported in the parameter value). This flow is defined in the "Flow Design" screen.                                                                                             |                                                 Not applicable                                                |
| 124 |                               ID of the email template that will be sent to the requester when a problem is created                              |                      |                  Enter the identification number (ID) of the problem-creating notification email template. When registering a problem in the "Problem Registration" screen, the defined email template will be used to send the problem creation notification. Where this notification will be sent to the requester. This email template ID is entered in the "Email Template" screen.                 | If you do not enter the identification number (ID) of the email template, you may not send the correct email. |
| 125 |                             ID of the email template that will be sent to the requester when a problem is in progress                            |                      |         Enter the identification number (ID) of the notification email template for the progress of the problem. When performing the problem on the "Problem" screen, the defined email template will be used to send the notification of the progress of the problem. Where this notification will be sent to the requester. This email template ID is entered in the "Email Template" screen.         | If you do not enter the identification number (ID) of the email template, you may not send the correct email. |
| 126 |                              ID of the email template that will be sent to the requester when a problem is finalized                             |                      |                        Enter the identification number (ID) of the problem-finishing notification email template. At the end of the problem on the "Problem" screen, the defined email template will be used to send the problem-finishing notification. Where this notification will be sent to the requester. This email template ID is entered in the "Email Template" screen.                       | If you do not enter the identification number (ID) of the email template, you may not send the correct email. |
| 127 |                             ID of the email template that will be sent to the target group when escalating a problem                             |                      | Enter the identification number (ID) of the notification email template for the escalation of the problem. When escalating a problem for the group in the "Problem Management" screen, the defined email template will be used to send the problem escalation notification. Where this notification will be sent to the target group. This email template ID is entered in the "Email Template" screen. | If you do not enter the identification number (ID) of the email template, you may not send the correct email. |
| 128 | ID of the email template that will be sent to the responsible party and executor group when the time to workaround/resolve a problem has expired |                      |              Enter the expiration notification email template ID number of the deadline to workaround/solve the problem. When the time to workaround/solve a problem has expired, the notice of expiration of the time to workaround/solve the problem, as defined, will be sent to the responsible and executing group. This email template ID is entered in the "Email Template" screen.              | If you do not enter the identification number (ID) of the email template, you may not send the correct email. |
| 129 |        Notify the responsible party and the executing group when the solution/workaround of the problem expires (Eg: Y or N - Default: 'Y'       |  Y or N (Default: Y) |                                                                                                                                    Define whether the responsible and the executing group will be notified when the time to workaround/solve the problem has expired.                                                                                                                                   |           If you do not enter the parameter value, the system default value will be used: "Y" (Yes).          |
| 194 |                               Enable problem escalation defined in the escalation rules? (Eg: Y or N - Default 'N')                              |  Y or N (Default: N) |                                                                                                        Define whether the problem escalation determined in the escalation rules is enabled. This problem escalation rule is defined in the "Escalation Rules and Automatic Notifications" screen.                                                                                                       |            If you do not enter the parameter value, the system default value will be set: "N" (No).           |


Table 1 - Parameters list



!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/09/2019 – Anna Martins
