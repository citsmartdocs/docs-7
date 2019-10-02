Description: Release Notes of CITSmart Version 7.0.0.0 from 03/01/2019

# Version 7.0.0.0
_03/01/2019_

## Fixes

### Ticket Management

The Sub-Request and Related Request functionalities were restructured to provide greater compliance to their assignments. The focus of this fix was to bring the functionalities closer to their proposal.

For further information, see [Relate Ticket][1] and [Register Sub-Request][2]

### Webservices

The synchronization for creating new Activities has changed in the business rule, that's because it's not possible to create an activity that doesn't have a link with the Business Service and Portfolio. Therefore, the webservice designated for creation will open a ticket with the parameters in the initial configuration of the service.

The functionality of create a new user, when the data synchronization is enabled, remains consistent.

### Flow

Adjustments to avoid editing native expressions and expressions of same name.

## New functionalities and Improvements

### Quick Access

The quick access allows the user to find main processes through icons that help in the efficiency of fixing and viewing.

**The users only sees the icons of the processes that they have access, with the exception of Simple, Knowledge Portal, Experience Center and User Guide.**

### Configuration of notification via email of delegated ticket

We created the possibility of configuring the functionality of email notification in the ticket delegation
For further information, see [Notification via E-mail of Ticket Delegated][3]

### Configuration of notification via email of reclassified ticket

We created the possibility of configuring the functionality notification via email reclassification
For further information, see [Notification via email of reclassified ticket][4]

### Change Management

Version 7.0.0.0 of CITSmart has improvements in the change management process, bringing the agile world to manage the activities that should occur during the scope of the change.

**Note:** This functionality replaces the default flow parameters for usage of the change process, moreover, the change is necessary for this configuration.


For further information, see [Change Management][5]

### Problem Management

In version 7.0.0.0 of CITSmar,t the problem management process allows adding activities to assist in the management of teams during the root cause diagnosis.

**Note:** This functionality replaces the default flow parameters for usage of the problem process, moreover, the change is necessary for this configuration.


For further information, see [Problem Management][6]

### Usage Configuration for Release Management

The release process is more powerful in planning, testing and approving, allowing the designation of activities and management at sight.

**Note:** This functionality replaces the default flow parameters for usage of release process, moreover, the change is necessary for this configuration.


For further information, see [Release Management][7]

### Comments Review

In version 7.0.0.0 CITSmart allows the evaluation and publication of written comments about a knowledge.

For further information, see [Comments Review][8]

### Access to the knowledge base of external users

We innovate the way of access to the knowledge base for users who don't have login to the CITSmart tool.

In version 7.0.0.0 knowledge with permission of visualization can be accessed by the community in general, just have the link of access.


For further information, see Configure external access to the [Knowledge Portal][9]

### Configuration Item Management

We enhance the user experience by highlighting a dashboard that displays the number of configuration items by group, type, and agglutinated in the Incident, Change, and Release processes, leaving in sight possible CI's that will be changed or involved in some incident.

For further information, see [Configuration Item Management][10]

### Escalation Rule

We simplified the use of ticket escalation rules, with a few steps, it'll be possible to implement the rule that previously had numerous configurations.

**Note:** This functionality replaces the use of several escalation parameters, moreover, it's necessary to change for the effective use of the escalation rules.


For further information, see [Create escalation rule][11]

### Ticket Approval

In version 7.0.0.0 of CITSmart, we included ticket approval through a new direct icon in the attendance list, it's not necessary to open the ticket to perform the attendance, we present the available information and the options configured to accept or refuse the call.

This functionality is available on Mobile SM and on the Service Portal.

For further information, see [Approve ticket][12]

### Automatic update of ticket list

We allow the automatic ticket list updating function to be enabled to refresh the list automatically from time to time.

For further information, see [Automatic Update of Ticket List][13]

### Occurrence

The improvement of the occurrence registration allows the requester or technician to be notified via email. In addition to the permission to include activity execution time and keep the information confidential registered, so that only authorized technicians can see it.

For further information, see [Register ticket occurrence][14]

### Simple - Agile Management at sight

Simple was created with the purpose of bringing the concept of agile management to the tool.
Independently or clustered in one of the Problem, Change and Release solutions, Simple allows you to reuse Sprints, share resources, send activities to other Sprints and manage at sight.

For further information, see [Simple][15]

### Customer's area

We provide a specific area to improve the user experience. In this area will be allowed the presentation of services, information and reports that come closest to the day-to-day use of the customer.

For further information, see [Experience Center][16]

### Business Intelligence

From the version 7.0.0.0, we have provided some quantitative reports of the main processes contained in CITSmart through our new BI platform.

For further information, see [Business Intelligence][17]

### Audit

We have reformed the system audit to increase the agility and reliability of the audit research feature.

For further information, see [System Audit][18]

### Password Security Policy

We have improved information security, implementing forms of password security for internal users.

For further information, see [Password Security Policy][19]

### Mobility 

We delivered a new application that, in a robust way, allow the field service of technicians who are momentarily without internet connection.

The mobility experience goes beyond signature features and notes.

For further information, see [Mobile Field Service][20]

Still in the context of mobility, and no less robust, we improved the Mobile SM application, which has among other uses, the ability to sign, approve and notes.

For further information, see [Mobile CITSmart Experience application manual][21]

### Neuro

From the version 1.2.3.0 of Neuro, it's possible to automatically create a CITSmart questionnaire from the Neuro business object register. The idea behind this innovation is to facilitate the extraction of responses from CITSmart questionnaires and to create reports in a simple way, with the help of the Smart Report.

### Flow

The package of flows delivered to the processes of Problem, Change and Release have been simplified, the products have been remodeled to adhere to the possibilities that the flow offers.

__If the customer doesn't want to use the new flows, the latest version 7.1.0 will continue to work perfectly.__


[1]:/en-us/citsmart-7/processes/tickets/use/register-ticket-related.html
[2]:/en-us/citsmart-7/processes/tickets/use/create-and-view-sub-request.html
[3]:/en-us/citsmart-7/processes/tickets/configuration/notification-delegated-email-ticket.html
[4]:/en-us/citsmart-7/processes/portfolio-and-catalog/configuration/send-email-reclassified-ticket.html
[5]:/en-us/citsmart-7/processes/change/overview.html
[6]:/en-us/citsmart-7/processes/problem/overview.html
[7]:/en-us/citsmart-7/processes/release/overview.html
[8]:/en-us/citsmart-7/processes/knowledge/use/review-reviews.html
[9]:/en-us/citsmart-7/processes/knowledge/configuration/configure-external-access-knowledge-portal.html
[10]:/en-us/citsmart-7/processes/configuration/overview.html
[11]:/en-us/citsmart-7/processes/tickets/use/create-escalation-rule.html
[12]:/en-us/citsmart-7/processes/tickets/use/approve-a-ticket.html
[13]:/en-us/citsmart-7/processes/tickets/use/desktop-of-service-desk.html
[14]:/en-us/citsmart-7/processes/tickets/use/register-ticket-occurrences.html
[15]:/en-us/citsmart-7/additional-features/project-management/simple-agile-management/simple-agile-management.html
[16]:/en-us/citsmart-7/processes/knowledge/use/create-experience-center.html
[17]:/en-us/citsmart-7/additional-features/smart-analytics/use-bi-solution.html
[18]:/en-us/citsmart-7/platform-administration/logs-and-auditing/system-audit.html
[19]:/en-us/citsmart-7/platform-administration/security/implement-password-security-rules.html
[20]:/en-us/citsmart-7/additional-features/mobile-and-field-service/apps/citsmart-field-service-manual.html
[21]:/en-us/citsmart-7/additional-features/mobile-and-field-service/apps/citsmart-app.html


