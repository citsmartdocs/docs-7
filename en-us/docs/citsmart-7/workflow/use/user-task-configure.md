title: Configure user activity in the workflow
Description: This document is intended to configure the activity within the workflow, called user task. 
# Configure user activity in the workflow 

When designing a workflow, it is possible to insert several elements, among them, the User Activity. This document is intended to guide the configuration of this element in the workflow.

Before getting started
----------------------
To use the "User Activity" element, it's necessary to have, at least, a registered workflow in the tool, with the event elements: "start" and "end".


!!! Abstract "NOTE"

    Within the *Interface* tab, choosing the "Neuro Form" Interaction Type: have 2 distinct Neuro 
    forms configured for the creation form to be displayed next to the monitoring form. 
    It is also necessary to create the Ticket Template for each of the forms.

Procedure
------------

1.	Access the main menu Workflow > Flow Design;
2.	Click on "New”;
3.	Click on the Diagram tab and then on Activity;
4.	Click on the User Task element and drag it to the workflow creation panel;
5.	The following element configuration tabs will be opened:

**Identification**

*	Name: name of the user task;

*	Description: detail the user task;

*	Type of instance:

    *	A single instance: it can only have a single non-executed instance of the task in the workflow;
    
    *	More than one instance controlled by the workflow: it can have multiple instances not executed from the task;
    
    *	Create an instance for each user: in the assignment, if there is a semicolon in the users, a task will be created for each user;

*	Identifier: it is a unique acronym for the task and it is used to code Rhino and for Neuro forms;

*	Counts SLA: it sets "Yes" or "No" ( the "Suspend SLA" status will appear in the ticket management interface);

*	Execution percentage: informative field about the percentage of this task in the entire workflow;

*	Is it an approval task?: set "Yes" or "No”;

**Assignment**

*	Recipient type: select whether it will be for a specific group or user

*	Assignment Type: define whether the assignment will be execution or monitoring

*	Group/User: select the group/user

*	Or Expression: search for an expression already registered

**User actions**

*	Select the registration action: it searches for the action already registered (e.g.:, approval action, that is, an expression for this purpose);

**Input action**

*	Build expression: it directly defines an expression
*	Select registration action: it searches for an action already registered

**Output action**

*	Build expression: it directly defines an expression

*	Select registration action: it searches for an action already registered

**Interface**

*	Interaction type: it is the way in which a Questionnaire or a Neuro Form will be applied in the ticket management interface, in a given workflow status. The configuration of items that will be visible can be defined in the portfolio, or configured directly in the User Activity element (of the workflow):

    *	Defined in portfolio: it is possible for a ticket template (questionnaire or form) to appear punctually in a workflow status, using what has been configured in the service attribute "Activity" (request/incident) - fields: “CREATION Template” and “Monitoring Template”. This option is advantageous when you have generic workflows used by several services.

    *	Standard form: default from system 

    *	Neuro Form: it has an identifier to call for the workflow triggered by this form

*	Template (Standard/Neuro): it allows to link the ticket template.

    !!! Abstract "ATTENTION"

        If there is no linking of a service request template in the interface tab, the system will subtend 
        and apply the settings of a standard form, enabling configuration item, change, problem and request 
        related to the ticket.
    
*	Allows to direct to group: enables the activation/deactivation of the "Direct to group" option in the registration of a ticket;

*	Allows to change the status: it makes visible/invisible the ticket attendance options (Registered/In Progress; Solved and Canceled);

*	Enables email notification: it makes the email notification options visible/invisible;

*	Allows delegate attendance: it enables the activation/deactivation of the "Delegate" option, in order to be visible in the options menu of the ticket management;

*	Allows change screen data: allows to edit questionnaires on the ticket management screen.

!!! Abstract "RULE"    
    
    The rules configured in the workflow will have priority over the service request template markings, as this is a 
    complement to the workflow.
    
**Knowledge Base**

   *  Link knowledge base: choose the knowledge you want to link to the user task.

!!! Abstract "ATTENTION"

    The main purpose of linking this knowledge is to allow the attendant of a request/incident to have easy access to it. 
    As soon as the workflow arrives at the activity of the flow linked to a knowledge, the button "Knowledge" is shown in 
    the upper right corner of the Request/Incident screen, to give read access to the content, for that, such knowledge is 
    usually written in the form of a step by step.
    
    
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/22/2019 – Anna Martins
