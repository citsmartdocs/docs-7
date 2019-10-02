title: Configurar Audit 0.4.0
Description: El objetivo de este documento es proporcionar el asesoramiento técnico de instalación y configuraciones para el uso de la funcionalidad de Auditoría (Audit), versión 0.4.0 (itsm-audit-0.4.0) del CITSmart Workflow 8.
# Configurar Audit 0.4.0

El objetivo de este documento es proporcionar el asesoramiento técnico de instalación y configuraciones para el uso de la funcionalidad de Auditoría (Audit), versión 0.4.0 (itsm-audit-0.4.0) del CITSmart Workflow 8.

Antes de empezar 
-----------------

Vea las principales novedades de la versión 0.4.0

 - No es necesario tener un AcitiveMQ externo activo;
 
 - No es necesario tener un servicio ejecutando el .jar de la auditoría;
 
 - Audit ahora es un .war y se ejecuta dentro de Wildfly junto al ITSM en la carpeta "\deployments";
 
Procedimiento
--------------

1. Agregar las siguientes líneas al standalone del wildfly en el subsistema del activemq:

    ```java
    <jms-queue name="ITSM.READ_DATA_AUDIT" entries="queue/ITSM.READ_DATA_AUDIT java:jboss/exported/jms/queue/queue/ITSM.READ_DATA_AUDIT"/>
    <jms-queue name="ITSM.READ_LICENSE_AUDIT" entries="queue/ITSM.READ_LICENSE_AUDIT java:jboss/exported/jms/queue/queue/ITSM.READ_LICENSE_AUDIT"/>
    <jms-queue name="ITSM.READ_ACCESS_AUDIT" entries="queue/ITSM.READ_ACCESS_AUDIT java:jboss/exported/jms/queue/queue/ITSM.READ_ACCESS_AUDIT"/>
    <jms-queue name="ITSM.READ_BACKUP_AUDIT" entries="queue/ITSM.READ_BACKUP_AUDIT java:jboss/exported/jms/queue/queue/ITSM.READ_BACKUP_AUDIT"/>
    ```

2. Agregar las siguientes líneas al standalone del wildfly en las system-properties (igual se utiliza en EVM e Inventory):  

    ```java
    <property name="mongodb.host" value="localhost"/>
    <property name="mongodb.port" value="27017"/>
    <property name="mongodb.user" value="mongodb"/>
    <property name="mongodb.password" value="mongodb"/>
    <property name="mongodb.dabase.audit" value="itsm-audit"/>
    ```
     
    !!! Abstract "OBSERVACIÓN "
    
        Configurar la conexión del banco mongo con host, port, user, pass y database (Probablemente ya existente, EVM e Inventory 
        utilizan estas configuraciones). Es necesario que el usuario (Mongo) insertado tenga los debidos permisos para lectura y 
        escritura en el banco informado.  
 
3. En CITSmart, configure el parámetro 425 que indica la dirección URL del Audit (Ej.: http://localhost:8080/itsm-audit);

4. Agregar el WAR del Audit en la carpeta de implementación (o a través de la consola del Wildfly) y empezar el Wildfly junto con 
CITSmart;

5. Después de estos pasos y configuraciones, la auditoría ya debe estar en ejecución.

Relacionado
-------------

[Realizar auditoría en el sistema](/es-es/citsmart-7/platform-administration/logs-and-auditing/system-audit.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>05/31/2019 – Larissa Lourenço
