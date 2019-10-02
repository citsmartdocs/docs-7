title: Configure Audit 0.4.0
Description: The purpose of this document is to provide the technical guidance for installation and configurations for the use of the Audit functionality, version 0.4.0 (itsm-audit-0.4.0) of CITSmart Workflow 8.
# Configure Audit 0.4.0

The purpose of this document is to provide the technical guidance for installation and configurations for the use of the Audit functionality, version 0.4.0 (itsm-audit-0.4.0) of CITSmart Workflow 8.

Before getting started 
-----------------

See the main news of version 0.4.0

 - It is not necessary to have an external active AcitiveMQ;
 
 - It is not necessary to have a service running the audit .jar;
 
 - Audit is now a .war and runs inside Wildfly next to ITSM in the "\deployments" folder;
 
Procedure
--------------

1. Add the following lines to the wildfly standalone in the activemq subsystem:

    ```java
    <jms-queue name="ITSM.READ_DATA_AUDIT" entries="queue/ITSM.READ_DATA_AUDIT java:jboss/exported/jms/queue/queue/ITSM.READ_DATA_AUDIT"/>
    <jms-queue name="ITSM.READ_LICENSE_AUDIT" entries="queue/ITSM.READ_LICENSE_AUDIT java:jboss/exported/jms/queue/queue/ITSM.READ_LICENSE_AUDIT"/>
    <jms-queue name="ITSM.READ_ACCESS_AUDIT" entries="queue/ITSM.READ_ACCESS_AUDIT java:jboss/exported/jms/queue/queue/ITSM.READ_ACCESS_AUDIT"/>
    <jms-queue name="ITSM.READ_BACKUP_AUDIT" entries="queue/ITSM.READ_BACKUP_AUDIT java:jboss/exported/jms/queue/queue/ITSM.READ_BACKUP_AUDIT"/>
    ```

2. Add the following lines to the wildfly standalone in system-properties (as it is used in EVM and Inventory):  

    ```java
    <property name="mongodb.host" value="localhost"/>
    <property name="mongodb.port" value="27017"/>
    <property name="mongodb.user" value="mongodb"/>
    <property name="mongodb.password" value="mongodb"/>
    <property name="mongodb.dabase.audit" value="itsm-audit"/>
    ```
     
    !!! Abstract "NOTE"
        
        Configure the mongo base connection with host, port, user, pass, and database (Probably already existed, EVM and Inventory use 
        these settings). It is necessary that the user (Mongo) inserted has the necessary permissions to read and write in the informed 
        base.  
 
3. In CITSmart, configure parameter 425 by entering the Audit URL (E.g.: http://localhost:8080/itsm-audit);

4. Add Audit WAR to the deployments folder (or via Wildfly Console) and start the Wildfly along with CITSmart;

5. After these steps and settings, the audit should already be running.

Related
-------------

[Audit system](/en-us/citsmart-7/platform-administration/logs-and-auditing/system-audit.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>05/31/2019 – Larissa Lourenço
