title:  System audit
Description: It allows to manage possible risks to the system
# System audit

This functionality allows to manage the possible risks to the system, when auditing all the executions made in the system in form of logs.
Some changes were made to the audit (itsm-audit-0.4.0), changes that are only at the configuration level.

Before getting started 
-----------------

Configure the functionality "Audit" in your instance.    

Procedure
------------

***Process to configure the Audit***

*Configuration to create a backup of the audits.*

First, it's essential to configure the specific parameters of the functionality.

1.  Access the main menu Parametrization \> Audit Parametrization;

2.  Inform in the field "Directory" the folder where it'll be kept all *logs* of
    the audits made;

3.  In the "Frequency in days" field, it's possible to adjust a backup routine of
    the audit logs, by choosing the periodicity of the backup in days.

    !!! Abstract "NOTE"

        The choice of frequency should be from 1 (one) day to the execution of the backup.  

4.  The possibility of determining a specific period (start and end date) for the
    generation of system audit logs is made available.

    !!! Abstract "IMPORTANT"

        It's offered three types of system audit: audit of system data, system access
        and system licenses .

***System data audit***

*It presentes the history of all change, inclusion, and deletion of data in the
system.*

1.  Access the main menu System \> Audit trail \> System logs;

2.  It'll be presented the audit logs of every move performed in the program,
    showing the date and time of the updates, the IP address, the executor
    name of the update, the name of the table, the type of operation made in 
    the system. Clicking on the data button, it'll show what was actually updated in the program.

    !!! Abstract "NOTE"  

        The "Operations" field presents the type of action made in the system 
        in thesis. It's defined by symbols, and their meanings are:  
        
        -   The letter "C" stands for "Change" in the system data;  
        
        -   The letter "I" stands for "Insertion" of new data into the system;  

        -   The letter "D" stands for "Deletion" of system data.  

3.  It's also released the search of a *log* through filters available in the screen.

***System access audit***

*It presentes the history of access in the system (login and logout).*

1.  Access the main menu System \>
    Audit trail \> Access audit;

2.  It'll present the users that made login and logout in the system, alos
    registering the date and hour of each of theses activities;

    !!! Abstract "NOTE"  
        
        If the system expires, it will not be possible to capture the system logout,
        so only the login information of the access session will be registered.  

3.  There are filters to help in the search of an access.

***System license audit***

*Inform the licenses used to validate the system.*

1.  Access the main menu System \>
    Audit trail \> Audit license;

2.  It presents the license data acquired and used to execute the system;

3.  It's possible to search for a license and its deadline by the filters
    in the main screen.
    
Related
---------

[Configure Audit 0.4.0](/en-us/citsmart-7/platform-administration/logs-and-auditing/audit040-configure.html)
    
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/15/2019 – Larissa Lourenço
