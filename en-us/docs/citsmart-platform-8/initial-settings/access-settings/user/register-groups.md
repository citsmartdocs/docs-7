title: Creating group
Description: This functionality registers the groups and links with users, profile, contracts and notification e-mails.

# Creating group

A group is a set of one or more employees with the same related objectives and its functions.

The two most common usages for the groups created are:

1.	Security/secrecy management of access to various types of registries (e.g.: knowledge base folders, service portfolios, etc.).

2.	Automatic notification scheduling based on some specific event/situation;


This functionality registers the groups and links with users, profile, contracts and notification e-mails.

This feature provides a variety of actions, such as including, changing, and deleting a group.

## Before getting started

To register a group, it's necessary to previously register the employee profile
access.

## Procedure

1.  Access the functionality Group through the main menu Access and Permission
    \> Group;

2.  Click on "New";

3.  Complete all mandatory fields;

    - **Basic Informations**

    |Field|Description|
    |-|-|
    |Name *	|[Name of Group]|
    |Acronym *	|[NG]|
    |Group ID|[01] - Automatically created|
    |Leader|[Name of Leader] - Used to identify the group manager|
    |Profile Access *	|[Profile] - Inherited access profile|
    |Service Desk Group|[Yes/No] - If the group makes attendance (= YES), otherwise, the group will not appear in the group list for ticket direction/delegation|
    |Chat Requester|[Yes/No] - If members of the group can open tickets via chat|
    |Change Advisory Board|[Yes/No] - If the group is part of a CAB (Change Management)|
    |Suspension/Reactivation |Parameter to allow tickets to be suspended/reactivated regardless of workflow permissions (reactivate/suspend)|
    |Mandatory email notifications (Opening, Progress and Closing)|If enabled, it makes the sending of email - coming from the various actions of the flows - mandatory (not configurable by the attendant). When it is disabled, the attendant can configure the options of email sending.|
    |Description |Details to help identify the group|

    - **Contracts:** Agreements that the group will have access (to register a service, attend and others).

    - **Permissions on workflows**

    |Actions```*```| Description|
	  |-|-|
	  |Create|Permission to register ticket/activity|
	  |Execute|Permission to execute ticket/activity|
    |Delegate|Permissino to delegate ticket/activity|
	  |Suspend|Permission to suspend ticket/activity|
    |Reactivate|Permission to reactivate ticket/activity|
    |Change SLA|Permission to change the SLA of a ticket/activity|
	  |Reopen|Permission to reopen ticket/activity|
    |Cancel|Permission to cancel ticket/activity|
    |Reclassify|Permission to reclassify ticket/activity|

    ```*```Select only the permissions specific to the context of the action.

    - **Employees (System users):** members of the group.
    - **E-mail:** email addresses that will receive notifications originating from a workflow. This option is very useful when it is necessary to make a person "informed" of the group's interactions without participating in the group.

4.  Define the necessary configurations;
5.  Click on "Save".


!!! Abstract "RULE"

    The group exclusion depends on there being no portfolios, employees and
    contracts linked to it.    

Related
-----------

[Register employee](/en-us/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Create profile access](/en-us/citsmart-7/initial-settings/access-settings/profile/create-profile-access.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROVt1SUUxco2tWF8E99_eva)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/10/2019 – Larissa Lourenço
