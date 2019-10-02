title: Request e-mail key fields
Description:Is intended to provide the list of key fields available for the Service Request e-mail template registration.
# Request e-mail key fields

This document is intended to provide the list of key fields available for the Service Request e-mail template registration.

List of key fields
----------------------

The key fields available for insertion in the e-mail template file related to
the Service Request are listed below:

|         **Key Field**         |                                                    **Description**                                                   |
|:-----------------------------:|:--------------------------------------------------------------------------------------------------------------------:|
|        ${OVERDUESLASTR}       |                         SLA Delay Time. Reports the SLA (Service Level Agreement) delay time.                        |
|        ${CONTRACTNAME}        |           Contract of the Request. Informs the name of the contract regarding the service/incident request.          |
|        ${STARTDATETIME}       |      Start date and time of request record. Informs the date and time the service/incident request was recorded.     |
|         ${ENDDATETIME}        |                 End date of the Request. Informs the date the service/incident request was completed.                |
| ${DATETIMEREACTIVATIONSLASTR} |              SLA start date and time. Informs the start date and time of SLA (Service Level Agreement).              |
|         ${DEADLINESTR}        |                   Deadline for request. Informs the deadline (date and time) to attend the request.                  |
|     ${REQUESTDATETIMESTR}     |            Date and time of request. Informs the date and time of service of the service/incident request.           |
|       ${DEMANDTYPENAME}       |                          Type of Request. Informs the type of request (Incident or Request).                         |
|         ${DESCRIPTION}        |                      Description of the Request. Informs the description of the service request.                     |
|       ${DESCRSITUATION}       |        Description of the Request Status. It informs the description of the Situation in which the Request is.       |
|         ${CAUSEDETAIL}        |                Detail of the Cause of the Incident. Informs the details of the cause of the incident.                |
|        ${CONTACTEMAIL}        |                          Applicant's E-mail for Contact. Inform the e-mail of the applicant.                         |
|        ${CURRENTPHASE}        |                    Current Phase of the Request. Reports the current phase of the service request.                   |
|        ${CURRENTGROUP}        |               Current Attendance Group. Informs the current group, responsible for the service request.              |
|         ${GROUPLEVEL1}        |                      Level 1 Group. Informs the Level 1 group configured to fulfill the request.                     |
|      ${IDSERVICEREQUEST}      |                                  Request Number. Informs the service request number.                                 |
|           ${IMPACT}           |         Impact of Service Request/Incident. Informs the identification of the impact of the service request.         |
|   ${LINKSATISFACTIONSURVEY}   |                    Link to satisfaction survey. Informs the link to evaluate the service request.                    |
|     ${LINKSERVICEREQUEST}     |                   Link to the service request. Reports the link to view the service request record.                  |
|         ${CONTACTNAME}        |                 Name of Applicant for Contact. Please provide the name of the requestor for contact.                 |
|      ${CURRENTGROUPNAME}      |             Returns the description of the Group Name in which the service request is currently located.             |
|         ${SERVICENAME}        |                               Service Name. Informs the name of the requested service.                               |
|     ${OWNERDEPARTMENTNAME}    |           Responsible Unit. Informs the unit of the person responsible for registering the service request           |
|   ${REQUESTERDEPARTMENTNAME}  |                                    Applicant's Unit. Informs the applicant's unit.                                   |
|         ${OBSERVATION}        |                    Applicant Contact Notice. Informs the notice described in the service request.                    |
|         ${ORIGINNAME}         |                           Origin of the Request. Informs the source of the service request.                          |
|          ${PRIORITY}          |             Priority of the Request of the Request. Informs the priority of service request fulfillment.             |
|          ${OWNERNAME}         | Responsible for the Registration of the Request. Informs the person responsible for registering the service request. |
|          ${RESPONSE}          |       Description of the Closing of the Request. Informs the description of the closing of the service request.      |
|         ${SERVICENAME}        |                            Service Requested. Enter the name of the service you requested.                           |
|         ${SITUACTION}         |                      Status of the Request; Informs the situation where the service request is.                      |
|         ${SLATOAGREE}         |                                   SLA "To Combine". Informs if the SLA is to match.                                  |
|        ${REQUESTERNAME}       |                              Name of Applicant. Please state the name of the applicant.                              |
|       ${REQUESTERUNITY}       |        Name of Applicant and Unit. It informs the name of the applicant and the unit in which it is allocated.       |
|        ${CONTACTPHONE}        |             Applicant's Telephone for Contact. Please provide the contact's telephone number for contact.            |
|           ${URGENCY}          |               Urgency of the Request. Informs the identification of the urgency of the service request.              |

Table 1 - List os key fields

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/10/2019 – Larissa Lourenço

