title: Create time of attendance
Description: Provides a variety of actions, such as including, changing, and deleting the time of attendance of type Global (applicable to all services), Client (applicable to the contract services) and Incident/Request/Procedure (applicable to a specific service).
# Create time of attendance

This feature provides a variety of actions, such as including, changing, and 
deleting the time of attendance of type *Global* (applicable to all services), 
*Client* (applicable to the contract services) and *Incident/Request/Procedure* 
(applicable to a specific service).

Before getting started
--------------------------

To register a time of attendance, it's necessary to previously register the
service portfolio.

Procedure
-------------

1.  Access the functionality Time of Attendance through the main menu Processes
    \> Service Level Management \> Attendance Time;

2.  Set the type of attendance time and click on the corresponding tab;

3.  Complete all mandatory field in **Basic Data**;

    !!! Abstract "IMPORTANT"

        Indicate in the attribute "Impact/Urgency Change", if it'll be allowed the 
        change of Impact and/or Urgency.
        
    !!! Abstract "ATTENTION"
    
        If the attendance time does not allow the change of impact and urgency, the 
        system automatically replaces what is sent via WebService to the impact, 
        urgency, priority and time of attendance defined in this register.

4.  In **Time of Attendance per Priority**, set the service time of attendance,
    taking into consideration the priority. The priority is used to identify the
    time required to an action to be taken. The priority goes from 1 to 5, being
    1 the highest priority and 5 the lowest. Select the priority to define the
    time:

    - **Capture**: set the time of capture of the service request, according to
      the priority selected;

    - **Resolution**: set the time of service resolution according to the priority
      selected.

5.  Before complete the fields in **Automation**, it should be properly
    parametrized, it must be properly parameterized, so it is necessary to
    execute the steps in the knowledge Creation escalation rule, except for
    parameter 190 that must be equal to 'N' in this context;

6.  Before the N minutes (informed in the time of action) and in case it doesn't
    have performed any action in the service request linked to this time of
    attendance, the system will attribute the priority and will escalate the
    execution group to the service request;

7.  In the fields of **Incident/Request/Procedure**, it will be selected the
    services to apply the configurations, taking into consideration the type of
    attendance time selected;

8.  Click on "Save".


Related
-------

[Register a service](/en-us/citsmart-7/processes/portfolio-and-catalog/use/register-a-service.html)

[Configure service attributes](/en-us/citsmart-7/processes/portfolio-and-catalog/use/configure-services-attributes.html)

[Create the portfolio](/en-us/citsmart-7/processes/portfolio-and-catalog/use/create-the-portfolio.html)

[Configure parametrization – ticket](/en-us/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)

[Create escalation rule](/en-us/citsmart-7/processes/tickets/use/create-escalation-rule.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RMDKjZH8augISpB17EQqrrc)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/04/2019 - Anna Martins
