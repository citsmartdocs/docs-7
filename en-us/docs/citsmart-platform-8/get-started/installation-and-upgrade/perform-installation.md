Title: Perform installation

# Perform installation

## Wildfly Installation Server

1. We should decompress the JAVA JDK package in the directory /opt and create a symbolic link as presented in the example below. (If you have already done the installation described in the "Create the citsmart.cfg file" in the same server that the Wildfly will be, it'll not be necessary the command execution of the JAVA JDK installation below).

    ```sh
    tar xzvf jdk-8u172-linux-x64.tar.gz -C /opt/
    ```

    ```sh
    ln -s /opt/jdk1.8.0_172 /opt/jdk
    ```

2. Execute the commands below to configure the CITSmart package.

    ```sh
    tar xzvf wildfly-12.0.0.Final.tar.gz -C /opt/
    ```

    ```sh
    ln -s /opt/wildfly-12.0.0.Final /opt/wildfly
    ```

    ```sh
    cp /etc/skel/.bash_profile /opt/wildfly/
    ```

    ```sh
    tar xzvf assets.tar.gz -C /opt/wildfly/
    ```

    ```sh
    mkdir /opt/wildfly/reports
    ```


3. Create an user to administrate the Wildfly:

    ```sh
    groupadd -r citsmart
    ```

    ```sh
    useradd -r -g citsmart -d /opt/wildfly -s /sbin/nologin citsmart
    ```

    ```sh
    chown citsmart:citsmart /opt/wildfly-12.0.0.Final/ -R
    ```

    ```sh
    chown citsmart:citsmart /opt/jdk1.8.0_172/ -R
    ```

4. Configure the **PATH** for the JAVA_HOME and JBOSS_HOME. For that, do as in the example below:

    ```sh
    vim /opt/wildfly/.bash_profile
    ```
    ```sh
    export JAVA_HOME="/opt/jdk"
    ```
    ```sh
    export JBOSS_HOME="/opt/wildfly"
    ```
    ```sh
    export PATH="$JAVA_HOME/bin:$JBOSS_HOME/bin:$PATH"
    ```

5. Make a test to validate if the Wildfly is starting correctly till this point. For that, execute the commands below:

    ```sh
    su - citsmart -s /bin/bash
    ```

    ```sh
    java -version
    ```
    ```html
    java version "1.8.0_172"
    Java(TM) SE Runtime Environment (build 1.8.0_172-b11)
    Java HotSpot(TM) 64-Bit Server VM (build 25.172-b11, mixed mode)
    ```
    ```sh
    bin/standalone.sh
    ```

6. Stop the Wildfly (previously started) and configure the standalone.conf in the directory $JBOSS_HOME/bin, as presented below:

    ```sh
    mv standalone.conf standalone.dist
    ```

    ```sh
    vim standalone.conf
    ```

    ```java
    if [ "x$JBOSS_MODULES_SYSTEM_PKGS" = "x" ]; then
    JBOSS_MODULES_SYSTEM_PKGS="org.jboss.byteman"
    fi  
    if [ "x$JAVA_OPTS" = "x" ]; then
    JAVA_OPTS="$JAVA_OPTS -Xms5200m"
    JAVA_OPTS="$JAVA_OPTS -Xmx5200m"
    JAVA_OPTS="$JAVA_OPTS -XX:MinHeapFreeRatio=40"
    JAVA_OPTS="$JAVA_OPTS -XX:MaxHeapFreeRatio=80"
    JAVA_OPTS="$JAVA_OPTS -XX:NewRatio=8"
    JAVA_OPTS="$JAVA_OPTS -XX:SurvivorRatio=32"
    JAVA_OPTS="$JAVA_OPTS -XX:+UseG1GC"
    JAVA_OPTS="$JAVA_OPTS -XX:G1HeapRegionSize=4"
    JAVA_OPTS="$JAVA_OPTS -XX:InitiatingHeapOccupancyPercent=50"
    JAVA_OPTS="$JAVA_OPTS -Djava.net.preferIPv4Stack=true"
    JAVA_OPTS="$JAVA_OPTS -Dorg.jboss.resolver.warning=true"
    JAVA_OPTS="$JAVA_OPTS -Duser.timezone="America/Sao_Paulo""
    JAVA_OPTS="$JAVA_OPTS -Djboss.modules.system.pkgs=$JBOSS_MODULES_SYSTEM_PKGS"
    JAVA_OPTS="$JAVA_OPTS -Djava.awt.headless=true"
    JAVA_OPTS="$JAVA_OPTS -Djboss.server.default.config=standalone-full-ha.xml"
    JAVA_OPTS="$JAVA_OPTS -Djboss.bind.address=0.0.0.0"
    JAVA_OPTS="$JAVA_OPTS -Djboss.bind.address.management=0.0.0.0"
    else
    echo "JAVA_OPTS already set in environment; overriding default settings with values: $JAVA_OPTS"
    fi
    ```

    ```sh
    chown citsmart:citsmart /opt/wildfly/bin/standalone.conf
    ```

### Wildfly Application Configuration Server

All configurations done in this document will be done through jboss-cli. For that, start the Wildfly in standalone, connect with jboss-cli and execute the following commands.

```sh
su citsmart /opt/wildfly/bin/standalone.sh -s /bin/bash
```

```sh
/opt/wildfly/bin/jboss-cli.sh --connect
```

```sh
[standalone@localhost:9990 /]
```

### Configure system properties

To create CITSmart properties, it is necessary to execute the following commands
in the CLI or edit the XML.

#### CLI

```java
/system-property=mongodb.host:add(value="citmongo")
/system-property=mongodb.port:add(value="27017")
/system-property=mongodb.user:add(value="admin")
/system-property=mongodb.password:add(value="admin")
/system-property=citsmart.protocol:add(value="http")
/system-property=citsmart.host:add(value="my.citsmart.com")
/system-property=citsmart.port:add(value="8080")
/system-property=citsmart.context:add(value="citsmart")
/system-property=citsmart.login:add(value="citsmart.local\\\consultor")
/system-property=citsmart.password:add(value="senhaConsultor")
/system-property=citsmart.inventory.id:add(value="citsmartinventory")
/system-property=citsmart.evm.id:add(value="citsmartevm")
/system-property=citsmart.evm.enable:add(value=true)
/system-property=citsmart.inventory.enable:add(value=true)
/system-property=rhino.scripts.directory:add(value="")
/system-property=jboss.as.management.blocking.timeout:add(value="600")
/system-property=citsmart.port.updateparameters:add(value="9000")
/system-property=citsmart.inventory.pagelength:add(value="100")
/system-property=org.quartz.properties:add(value="$\{jboss.server.config.dir\}/quartz.properties")
/system-property=snmp.oid.repository.directory:add(value="/opt/templates")
```

#### XML

```java
<system-properties>
    <property name="mongodb.host" value="citmongo"/>
    <property name="mongodb.port" value="27017"/>
    <property name="mongodb.user" value="admin"/>
    <property name="mongodb.password" value="admin"/>
    <property name="citsmart.protocol" value="http"/>
    <property name="citsmart.host" value="my.citsmartcloud.com"/>
    <property name="citsmart.port" value="8080"/>
    <property name="citsmart.context" value="citsmart"/>
    <property name="citsmart.login" value="citsmart.local\\\consultor"/>
    <property name="citsmart.password" value="senhaConsultor"/>
    <property name="citsmart.inventory.id" value="citsmartinventory"/>
    <property name="citsmart.evm.id" value="citsmartevm"/>
    <property name="citsmart.evm.enable" value="false"/>
    <property name="citsmart.inventory.enable" value="false"/>
    <property name="rhino.scripts.directory" value=""/>
    <property name="jboss.as.management.blocking.timeout" value="600"/>
    <property name="citsmart.port.updateparameters" value="9000"/>
    <property name="citsmart.inventory.pagelength" value="100"/>
    <property name="org.quartz.properties" value="${jboss.server.config.dir}/quartz.properties"/>
    <property name="snmp.oid.repository.directory" value="/opt/templates"/>
</system-properties>
```

### Datasources configuration

Before creating the datasources, we have to add to the Wildfly the module JDBC of PostgreSQL. For that, exit the mode jboss-cli and execute the commands below.

1. Add the database module as in the example below:

    ```sh
    mkdir -p /opt/wildfly/modules/system/layers/base/org/postgres/main
    ```

    ```sh
    tar xzvf postgresql-jdbc-driver.tar.gz -C /opt/wildfly/modules/system/layers/base/org/postgres/main
    ```

    ```sh
    chown citsmart:citsmart /opt/wildfly/modules/system/layers/base/org/postgres/ -R
    ```

2. Connect the jboss-cli once again and execute the command below to add the module to the standalone-full-ha.xml   

    ```sh
    module add --name=org.postgres --resources=/opt/wildfly/modules/system/layers/base/org/postgres/main/postgresql-9.3-1103.jdbc41.jar --dependencies=javax.api,javax.transaction.api
    ```
    ```sh
    /subsystem=datasources/jdbc-driver=postgres:add(driver-name="postgres",driver-module-name="org.postgres",driver-xa-datasource-class-name=org.postgresql.xa.PGXADataSource
    ```

3. There are **eight inputs** of datasource for the **citsmart_db**, being four for CITSmart and four for CITSmart Neuro. The user and password is **citsmartdbuser and exemplo123** respectively created in the section *PostgreSQL Database Server*.

4. To create datasources, execute the CLI commands below:

    Datasource citsmart:

    ```sh
    /subsystem=datasources/data-source="/jdbc/citsmart":add(jndi-name="java:/jdbc/citsmart",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.citsmart.com:5432/citsmart_db",user-name="citsmartdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
    /subsystem=datasources/data-source="/jdbc/citsmart":write-attribute(name=min-pool-size,value=10)
    /subsystem=datasources/data-source="/jdbc/citsmart":write-attribute(name=max-pool-size,value=300)
    /subsystem=datasources/data-source="/jdbc/citsmart":write-attribute(name=pool-prefill,value=true)
    /subsystem=datasources/data-source="/jdbc/citsmart":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
    /subsystem=datasources/data-source="/jdbc/citsmart":write-attribute(name=blocking-timeout-wait-millis,value=60000)
    /subsystem=datasources/data-source="/jdbc/citsmart":write-attribute(name=idle-timeout-minutes,value=5)
    ```

    Datasource citsmartFlow:

    ```sh
    /subsystem=datasources/data-source="/jdbc/citsmartFluxo":add(jndi-name="java:/jdbc/citsmartFluxo",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.citsmart.com:5432/citsmart_db",user-name="citsmartdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
    /subsystem=datasources/data-source="/jdbc/citsmartFluxo":write-attribute(name=min-pool-size,value=10)
    /subsystem=datasources/data-source="/jdbc/citsmartFluxo":write-attribute(name=max-pool-size,value=300)
    /subsystem=datasources/data-source="/jdbc/citsmartFluxo":write-attribute(name=pool-prefill,value=true)
    /subsystem=datasources/data-source="/jdbc/citsmartFluxo":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
    /subsystem=datasources/data-source="/jdbc/citsmartFluxo":write-attribute(name=blocking-timeout-wait-millis,value=60000)
    /subsystem=datasources/data-source="/jdbc/citsmartFluxo":write-attribute(name=idle-timeout-minutes,value=5)
    ```

    Datasourece citsmart_reports

    ```sh
    /subsystem=datasources/data-source="/jdbc/citsmart_reports":add(jndi-name="java:/jdbc/citsmart_reports",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.citsmart.com:5432/citsmart_db",user-name="citsmartdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
    /subsystem=datasources/data-source="/jdbc/citsmart_reports":write-attribute(name=min-pool-size,value=10)
    /subsystem=datasources/data-source="/jdbc/citsmart_reports":write-attribute(name=max-pool-size,value=300)
    /subsystem=datasources/data-source="/jdbc/citsmart_reports":write-attribute(name=pool-prefill,value=true)
    /subsystem=datasources/data-source="/jdbc/citsmart_reports":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
    /subsystem=datasources/data-source="/jdbc/citsmart_reports":write-attribute(name=blocking-timeout-wait-millis,value=60000)
    /subsystem=datasources/data-source="/jdbc/citsmart_reports":write-attribute(name=idle-timeout-minutes,value=5)
    ```

    Datasource citsmartBpmEventos

    ```sh
    /subsystem=datasources/data-source="/jdbc/citsmartBpmEventos":add(jndi-name="java:/jdbc/citsmartBpmEventos",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.citsmart.com:5432/citsmart_db",user-name="citsmartdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
    /subsystem=datasources/data-source="/jdbc/citsmartBpmEventos":write-attribute(name=min-pool-size,value=10)
    /subsystem=datasources/data-source="/jdbc/citsmartBpmEventos":write-attribute(name=max-pool-size,value=300)
    /subsystem=datasources/data-source="/jdbc/citsmartBpmEventos":write-attribute(name=pool-prefill,value=true)
    /subsystem=datasources/data-source="/jdbc/citsmartBpmEventos":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
    /subsystem=datasources/data-source="/jdbc/citsmartBpmEventos":write-attribute(name=blocking-timeout-wait-millis,value=60000)
    /subsystem=datasources/data-source="/jdbc/citsmartBpmEventos":write-attribute(name=idle-timeout-minutes,value=5
    ```

    Datasource citsmart-neuro

    ```sh
    /subsystem=datasources/data-source="/env/jdbc/citsmart-neuro":add(jndi-name="java:/env/jdbc/citsmart-neuro",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.citsmart.com:5432/citsmart_db",user-name="citsmartdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=min-pool-size,value=10)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=max-pool-size,value=300)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=pool-prefill,value=true)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=blocking-timeout-wait-millis,value=60000)
    ```

    Datasource citsmart-neuro-app1

    ```sh
    /subsystem=datasources/data-source="/env/jdbc/citsmart-neuro-app1":add(jndi-name="java:/env/jdbc/citsmart-neuro-app1",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.citsmart.com:5432/citsmart_db",user-name="citsmartdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=min-pool-size,value=10)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=max-pool-size,value=300)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=pool-prefill,value=true)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=blocking-timeout-wait-millis,value=60000)
    ```

    Datasource citsmart-neuro-app2

    ```sh
    /subsystem=datasources/data-source="/env/jdbc/citsmart-neuro-app2":add(jndi-name="java:/env/jdbc/citsmart-neuro-app2",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.citsmart.com:5432/citsmart_db",user-name="citsmartdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=min-pool-size,value=10)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=max-pool-size,value=300)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=pool-prefill,value=true)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=blocking-timeout-wait-millis,value=60000)
    ```

    Datasource citsmart-neuro-app3

    ```sh
    /subsystem=datasources/data-source="/env/jdbc/citsmart-neuro-app3":add(jndi-name="java:/env/jdbc/citsmart-neuro-app3",driver-name="postgres",connection-url="jdbc:postgresql://pgdata.citsmart.com:5432/citsmart_db",user-name="citsmartdbuser",password="exemplo123",driver-class="org.postgresql.Driver", enabled=true, use-java-context=true)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=min-pool-size,value=10)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=max-pool-size,value=300)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=pool-prefill,value=true)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=flush-strategy,value=FailingConnectionOnly)
    /subsystem=datasources/data-source="/env\/jdbc\/citsmart-neuro":write-attribute(name=blocking-timeout-wait-millis,value=60000)
    ```

5. Before exit the jboss-cli, execute the command reload to apply the changes. Then, make a connection text with database;

    ```sh
    [standalone\@localhost:9990 /] :reload
    ```
    ```sh
    [standalone\@localhost:9990 /] /subsystem=datasources/data-source="/jdbc/citsmart":test-connection-in-pool { "outcome" =\> "success", "result" =\> [true] }
    ```

### Configure subsytems

```sh
/subsystem=logging/root-logger=ROOT:write-attribute(name=level,value=INFO)
/subsystem=logging/console-handler=CONSOLE:write-attribute(name=level,value=INFO)
/subsystem=undertow/server=default-server/http-listener=default:write-attribute(name=max-post-size,value="5000485760")
/subsystem=undertow/server=default-server/http-listener=default:write-attribute(name=max-parameters,value="3000")
/subsystem=undertow/server=default-server/http-listener=default:write-attribute(name=max-header-size,value="65535")
/subsystem=undertow/server=default-server/https-listener=https:write-attribute(name=max-post-size,value="5000485760")
/subsystem=undertow/server=default-server/https-listener=https:write-attribute(name=max-header-size,value="65535")
/subsystem=undertow/server=default-server/https-listener=https:write-attribute(name=max-parameters,value="3000")
/subsystem=undertow/configuration=filter/rewrite=citsmart:add(target="/citsmart")
/subsystem=undertow/server=default-server/host=default-host/filter-ref=citsmart:add(predicate="regex('\^/?\$') and equals(/citsmart)")
/subsystem=undertow/server=default-server/host=default-host/setting=access-log:add
/subsystem=undertow/server=default-server/host=default-host/setting=access-log:write-attribute(name=pattern, value="%h %l %u [%t] \\"%r\\" %s %b \\"%{i,Referer}\\" \\"%{i,User-Agent}\\"")
/subsystem=messaging-activemq/server=default/jms-queue=filaDocumentoQueue:add(entries=["queue/filaDocumento","java:jboss/exported/jms/queue/filaDocumento"])
/subsystem=messaging-activemq/server=default/jms-topic=filaDocumentoTopic:add(entries=["topic/filaDocumento","java:jboss/exported/jms/topic/filaDocumento"])
/subsystem=messaging-activemq/server=default/jms-queue=neuroInputQueue:add(entries=["queue/neuroInputQueue","java:jboss/exported/jms/queue/queue/neuroInputQueue"])
/subsystem=messaging-activemq/server=default/jms-queue=neuroOutputQueue:add(entries=["queue/neuroOutputQueue","java:jboss/exported/jms/queue/queue/neuroOutputQueue"])
/subsystem=deployment-scanner/scanner=default:write-attribute(name=deployment-timeout,value=6000000)
```

1. To enable uploading above 10 Mb, include in the subsystems file the following information:

    ```java
    <subsystem xmlns="urn:jboss:domain:undertow:5.0">
            <buffer-cache name="default"/>
            <server name="default-server">
                <http-listener name="default" socket-binding="http" max-post-size="5000485760" max-header-size="65535" max-parameters="3000" redirect-socket="https" enable-http2="true"/>
                <https-listener name="https" socket-binding="https" max-post-size="5000485760" max-header-size="65535" max-parameters="3000" security-realm="ApplicationRealm" enable-http2="true"/>

            ...
            </server>
    ...
    </subsystem>
    ```

2. Before leaving jboss-cli run the reload command to apply the changes.

    ```sh
    [standalone\@localhost:9990 /] :reload
    ```


## Create citsmart.cfg file

1. In the citsmart.cfg file, the default value is TRUE, that is, if this option does not exist in the file the system will take the value TRUE for this property. Set to TRUE it activates the Thread that updates the fact table of service requests at system startup. Set to FALSE the update will happen only after the inclusion or change of the service request;

2. We should create a file citsmart.cfg in /opt/wildfly/standalone/configuration/ with the information below:

    ```java
    START_MONITORA_INCIDENTES=FALSE
    JDBC_ALIAS_REPORTS=
    JDBC_ALIAS_BPM=
    JDBC_ALIAS_BPM_EVENTOS=
    START_VERIFICA_EVENTOS=FALSE
    QUANTIDADE_BACKUPLOGDADOS=1000
    START_MODE_RULES=FALSE
    START_MODE_RULES=FALSE
    LOAD_FACTSERVICEREQUESTRULES=TRUE
    INICIAR_PROCESSAMENTOS_BATCH=TRUE
    ```

    !!! warning "ATTENTION"

        Do not forget to change the owner of the files and directories to the CITSmart's user.

## Quartz Configuration

CITSmart Batch processing uses Quartz for scheduling and processing system routines. To set it up, follow the procedure:

1. Create a file named "quartz.properties" containing the data below, depending on your type of installation (standalone or cluster);
2. Save this file to the application server's "configuration" folder.

### Standalone Installation (database-independent):

```java
#===============================================================
#Configure Main Scheduler Properties
#===============================================================
org.quartz.scheduler.instanceName = CitSmartMonitor
org.quartz.scheduler.instanceId = AUTO
#===============================================================
#Configure ThreadPool
#===============================================================
org.quartz.threadPool.threadCount =  5
org.quartz.threadPool.threadPriority = 5
org.quartz.threadPool.class = org.quartz.simpl.SimpleThreadPool
#===============================================================
#Configure JobStore
#===============================================================
org.quartz.jobStore.class = org.quartz.simpl.RAMJobStore
```

### Cluster Installation

#### Postgres Database

```java
#============================================================================
# Configure Main Scheduler Properties
#============================================================================
org.quartz.scheduler.instanceName = CitSmartMonitor
org.quartz.scheduler.instanceId = AUTO
#============================================================================
# Configure ThreadPool
#============================================================================
org.quartz.threadPool.class = org.quartz.simpl.SimpleThreadPool
org.quartz.threadPool.threadCount = 25
org.quartz.threadPool.threadPriority = 5
#============================================================================
# Configure JobStore
#============================================================================
org.quartz.jobStore.misfireThreshold = 60000
org.quartz.jobStore.class = org.quartz.impl.jdbcjobstore.JobStoreTX
org.quartz.jobStore.driverDelegateClass = org.quartz.impl.jdbcjobstore.PostgreSQLDelegate
org.quartz.jobStore.useProperties = true
org.quartz.jobStore.dataSource = citsmart
org.quartz.jobStore.tablePrefix = QRTZ_
org.quartz.jobStore.isClustered = true
org.quartz.jobStore.clusterCheckinInterval = 20000
org.quartz.dataSource.citsmart.jndiURL= java:/jdbc/citsmart
```

#### Microsoft SQL Server Database

```java
#============================================================================
# Configure Main Scheduler Properties
#============================================================================
org.quartz.scheduler.instanceName = CitSmartMonitor
org.quartz.scheduler.instanceId = AUTO
#============================================================================
# Configure ThreadPool
#============================================================================
org.quartz.threadPool.class = org.quartz.simpl.SimpleThreadPool
org.quartz.threadPool.threadCount = 25
org.quartz.threadPool.threadPriority = 5
#============================================================================
# Configure JobStore
#============================================================================
org.quartz.jobStore.misfireThreshold = 60000
org.quartz.jobStore.class = org.quartz.impl.jdbcjobstore.JobStoreTX
org.quartz.jobStore.driverDelegateClass = org.quartz.impl.jdbcjobstore.MSSQLDelegate
org.quartz.jobStore.useProperties = true
org.quartz.jobStore.dataSource = citsmart
org.quartz.jobStore.tablePrefix = QRTZ_
org.quartz.jobStore.isClustered = true
org.quartz.jobStore.clusterCheckinInterval = 20000
org.quartz.dataSource.citsmart.jndiURL= java:/jdbc/citsmart
```

#### Oracle Database:

```java
#============================================================================
# Configure Main Scheduler Properties
#============================================================================
org.quartz.scheduler.instanceName = CitSmartMonitor
org.quartz.scheduler.instanceId = AUTO
#============================================================================
# Configure ThreadPool
#============================================================================
org.quartz.threadPool.class = org.quartz.simpl.SimpleThreadPool
org.quartz.threadPool.threadCount = 25
org.quartz.threadPool.threadPriority = 5
#============================================================================
# Configure JobStore
#============================================================================
org.quartz.jobStore.misfireThreshold = 60000
org.quartz.jobStore.class = org.quartz.impl.jdbcjobstore.JobStoreTX
org.quartz.jobStore.driverDelegateClass = org.quartz.impl.jdbcjobstore.oracle.OracleDelegate
org.quartz.jobStore.useProperties = true
org.quartz.jobStore.dataSource = citsmart
org.quartz.jobStore.tablePrefix = QRTZ_
org.quartz.jobStore.isClustered = true
org.quartz.jobStore.clusterCheckinInterval = 20000
org.quartz.dataSource.citsmart.jndiURL= java:/jdbc/citsmart
```

## Create directories to installation

!!! warning "ATTENTION"

    Don't forget to change the owner of directory /opt/citsmart .

1. Create the directories below to be configured in the 3 (three) steps of web installation.

    **For GED:**

    ```sh
    mkdir -p /opt/citsmart/ged
    ```

    **For Knowledge Base:**

    ```sh
    mkdir /opt/citsmart/kb
    ```

    **For Synonyms:**

    ```sh
    mkdir /opt/citsmart/twinwords
    ```

    **For Attachments of Knowledge Base:**

    ```sh
    mkdir /opt/citsmart/attachkb
    ```

    **For Upload:**

    ```
	mkdir /opt/citsmart/upload
    ```

## Generate certificate SSL Self-Signed

For the Wildfly it will be created a self-signed certificate. If you have a certificate, follow the next steps.

!!! info "TIPS"

    - The passwords used in this manual are 123456, please, enter one of your preference;

    - The manual certificate files use the suffix abc, please, put in your preference;

    - The default password for cacerts is "changeit" and should be used to add the cer file;

    - If you use different passwords and file names, change before executing the commands.

### Self-signed certificate:

Creating new alias with DNS (example itsm.citsmart.com):

```sh
/opt/jdk/bin/keytool -genkey -alias GRPv1 -keyalg RSA -keystore /opt/wildfly/standalone/configuration/GRPv1.keystore -ext san=dns:itsm.citsmart.com -validity 3650 -storepass 123456
```

Creating alias with IP of Jboss server (example 192.168.0.40):

```sh
/opt/jdk/bin/keytool -genkey -alias GRPv1 -keyalg RSA -keystore /opt/wildfly/standalone/configuration/GRPv1.keystore -ext san=ip:192.168.0.40 -validity 3650 -storepass 123456
```

Exporting certificate to extension .cer:

```sh
/opt/jdk/bin/keytool -export -alias GRPv1 -keystore /opt/wildfly/standalone/configuration/GRPv1.keystore -validity 3650 -file /opt/wildfly/standalone/configuration/GRPv1.cer
```

### Proper certificate:

Create pkcs12 based on its public key (.crt) and private (.key)

```sh
openssl pkcs12 -export -in abc.crt -inkey abc.key -out abc.p12
```    
    
After creating the pkcs12 (.p12) you create the file keystore (jks) that will be added to the wildfly.
    
```sh
keytool -importkeystore -srckeystore abc.p12 \
        -srcstoretype PKCS12 \
        -destkeystore abc.jks \
        -deststoretype JKS    
``` 

### For both type of certificates:

Adding certificate in the cacerts of Java:

```sh
/opt/jdk/bin/keytool -keystore /opt/jdk/jre/lib/security/cacerts -importcert -alias GRPv1 -file /opt/wildfly/standalone/configuration/GRPv1.cer
```

**Remember to apply the permissions to the wildfly and java jdk owner**

```sh
chown citsmart:citsmart /opt/jdk1.8.0_172/ -R chown citsmart:citsmart /opt/wildfly-12.0.0.Final/ -R
```

After generate the certificate, connect once again in the jboss-cli and execute the commands below:

```sh
/subsystem=undertow/server=default-server/https-listener=https:read-attribute(name=security-realm)
/subsystem=elytron/key-store=citsmartKeyStore:add(path="GRPv1.keystore",relative-to=jboss.server.config.dir,credential-reference={clear-text="123456"},type=JKS)
/subsystem=elytron/key-manager=citsmartKeyManager:add(key-store=citsmartKeyStore,credential-reference={clear-text="123456"})
/subsystem=elytron/server-ssl-context=citsmartSSLContext:add(key-manager=citsmartKeyManager,protocols=["TLSv1.2"])
/core-service=management/security-realm=ApplicationRealm/server-identity=ssl:remove
/core-service=management/security-realm=ApplicationRealm/server-identity=ssl:add(keystore-path="GRPv1.keystore", keystore-password-credential-reference={clear-text="123456"}, keystore-relative-to="jboss.server.config.dir",alias="GRPv1")
```

Before exit the jboss-cli, execute the command reload to apply the changes.

```sh
[standalone@localhost:9990 /] :reload
```

## Starting solutions following dependecies

1. Before leaving jboss-cli run the reload command to apply the changes.

    **PostgreSQL Database Server**

    ```sh
    systemctl postgresql start
    ```

    **MongoDB Database Server**

    ```sh
    /opt/mongodb-linux-x86_64-rhel70-3.4.15/bin/mongod --auth --port 27017
    ```

    **Apache Solr Indexing Server**

    ```sh
    su solr /opt/solr/bin/solr start -s /bin/bash
    ```

    **Wildfly Application Server**

    ```sh
    su citsmart /opt/wildfly/bin/standalone.sh -s /bin/bash
    ```

## CITSmart Enterprise Deployment

1. Send the files of deployment provided to the server and move them to the directory "deployments";

    ```sh
    cp CitsmartITSM-Enterprise.war /opt/wildfly/standalone/deployments/
    ```

2. Do the CITSmart Neuro deployment after finish the steps in section "CITSmart Neuro Deployment".

### Access CITSmart Enterprise

1. To access the CITSmart Enterprise, we should access the IP or DNS with the port and context:

    ```sh
    https://example.com:8443/citsmart
    ```

2. The CITSmart context is standard to the CITSmart Enterprise.

    First Access: Enter the URL > ```https://example.com:8443/citsmart```.

3. Now, follow the steps in the manual of 3 steps and start to use the solution CITSmart.

## CITSmart Neuro Deployment

1. Send the files of deployment provided to the server and move them to the directory "deployments".

    ```sh
    cp citsmart-neuro-web.war /opt/wildfly/standalone/deployments/
    ```
    
## Browsers supported

For the proper functioning of the system, the following minimum versions of browsers should be used:

- EDGE (minimum version): Microsoft Edge 42.17134.0/ Microsoft EdgeHTML 17.17134;

- Google Chrome (minimum version): version 76.0.3809.132 (official version) 64 bits;

- Mozila Firefox Quantum (minimum version): 69.0 (64 bits)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/22/2019 - Docummentation Team
