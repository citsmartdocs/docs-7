Title: Hacer la instalación

# Hacer la instalación

## Instalación del Servidor de Aplicación Wildfly

1. Descomprimir el paquete JAVA JDK en el directorio /opt y crear un link
simbólico conforme mostrado en el ejemplo abajo. *(Caso ya tenga hecho la
instalación del ítem Servidor de Indexación Apache Solr (sesión Configuración de los
paquetes) el mismo servidor que el Wildfly se va a quedar, no será necesario la ejecución
de los comandos de instalación del Java JDK abajo)*.

    ```sh
    tar xzvf jdk-8u172-linux-x64.tar.gz -C /opt/
    ```

    ```sh
    ln -s /opt/jdk1.8.0_172 /opt/jdk
    ```

2. Ejecutar los comandos siguientes para configuración de los paquetes para CITSmart;

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

3. crear un usuario para administrar el Wildfly;

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

4. Configurar **PATH** para el JAVA_HOME y el JBOSS_HOME. Para
eso,  haga conforme el ejemplo siguiente.

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

5. Haga una prueba para validar se el Wildfly está iniciando correctamente hasta ese
punto. Para eso, ejecute los comandos siguientes.

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

6. Parar el Wildfly (Iniciado anteriormente) y configurar el standalone.conf en el
directorio \$JBOSS_HOME/bin, conforme presentado abajo.

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
### Configuração do Servidor de Aplicação Wildfly

Todas las configuraciones hechas en este documento se harán a través de jboss-cli. Para ello, inicie el Wildfly en standalone, conéctese a jboss-cli y ejecute los siguientes comandos.

```sh
su citsmart /opt/wildfly/bin/standalone.sh -s /bin/bash
```

```sh
/opt/wildfly/bin/jboss-cli.sh --connect
```

```sh
[standalone@localhost:9990 /]
```

### Configuración del System Properties

Para crear propiedades CITSmart, se debe ejecutar los siguientes comandos en la CLI o editar el XML.

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

### Configuración de los Datasources

Antes de crear los datasources, debemos adicionar al Wildfly el modulo JDBC del
PostgreSQL. Para eso, salga del modo jboss-cli y ejecute los comandos abajo.

1. Añadir el modulo del banco de datos como en el ejemplo abajo:

    ```sh
    mkdir -p /opt/wildfly/modules/system/layers/base/org/postgres/main
    ```

    ```sh
    tar xzvf postgresql-jdbc-driver.tar.gz -C /opt/wildfly/modules/system/layers/base/org/postgres/main
    ```

    ```sh
    chown citsmart:citsmart /opt/wildfly/modules/system/layers/base/org/postgres/ -R
    ```

2. Conectar en el jboss-cli nuevamente y ejecute el comando siguiente para adicionar el
módulo al standalone-full-ha.xml

    ```sh
    module add --name=org.postgres --resources=/opt/wildfly/modules/system/layers/base/org/postgres/main/postgresql-9.3-1103.jdbc41.jar --dependencies=javax.api,javax.transaction.api
    ```
    ```sh
    /subsystem=datasources/jdbc-driver=postgres:add(driver-name="postgres",driver-module-name="org.postgres",driver-xa-datasource-class-name=org.postgresql.xa.PGXADataSource
    ```

3. Hay **ocho entradas** de datasource para **citsmart_db**, siendo que
cuatro para Citsmart y cuatro para Citsmart Neuro. El usuario y contraseña
e **citsmartdbuser y exemplo123** creados respectivamente en el ítem *Servidor de Base de Datos
PostgreSQL*.

4. Para crear los datasources, ejecute los comandos CLI abajo:

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

5.  Antes de salir de jboss-cli ejecute el comando reload para aplicar los cambios y realizar una prueba de conexión con la base de datos.

    ```sh
    [standalone\@localhost:9990 /] :reload
    ```
    ```sh
    [standalone\@localhost:9990 /] /subsystem=datasources/data-source="/jdbc/citsmart":test-connection-in-pool { "outcome" =\> "success", "result" =\> [true] }
    ```

### Configurando los Subsytems


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

1. Para poder subir por encima de 10 Mb, incluir en el archivo subsystems la siguiente información:

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

2. Antes de salir del jboss-cli, ejecute el comando reload para aplicar los cambios.

    ```sh
    [standalone\@localhost:9990 /] :reload
    ```

## Crear archivo citsmart.cfg

1. En el archivo citsmart.cfg, el valor predeterminado es TRUE, es decir, si esta opción no existe en el archivo, el sistema utilizará el valor TRUE para esa propiedad. Definido como TRUE, activa el Thread que actualiza la tabla fatos de solicitudes de servicio en el inicio del sistema. Definido como FALSE, la actualización sólo se producirá después de la inclusión o modificación de la solicitud de servicio;

2. Debemos crear un archivo citsmart.cfg en /opt/wildfly/standalone/configuration/ con las informaciones siguientes:


    ```java
    START_MONITORA_INCIDENTES=FALSE
    JDBC_ALIAS_REPORTS=
    JDBC_ALIAS_BPM=
    JDBC_ALIAS_BPM_EVENTOS=
    START_VERIFICA_EVENTOS=FALSE
    QUANTIDADE_BACKUPLOGDADOS=1000
    START_MODE_RULES=FALSE
    START_MODE_RULES=FALSE
    LOAD_FACTSERVICEREQUESTRULES = TRUE
    ```


    !!! warning "ATENCIÓN"

         No olvides de cambiar el dueño de los archivos y directorios para el usuario CITSmart.

## Configuración del Quartz

El procesamiento Batch de CITSmart utiliza Quartz para la programación y el procesamiento de rutinas de sistema. Para configurarlo, siga el procedimiento:

1. Criar un archivo de nombre "quartz.properties" que contiene los datos siguientes, según su tipo de instalación (standalone o cluster);
2. Guardar este archivo en la carpeta de configuración del servidor de aplicaciones.

### Instalación Standalone (independiente de base de datos)

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

### Instalación Cluster

#### Base de Datos Postgres:

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

#### Base de Datos Microsoft SQL Server:

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

#### Base de Datos Oracle:

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

## Creación de directorios para instalación


!!! warning "ATENCIÓN"

    No olvides de cambiar el dueño del directorio /opt/citsmart .


1. Crear los directorios abajo para ser configurados en los 3 pasos de instalación web.

    **Para GED**:

    ```sh
    mkdir -p /opt/citsmart/ged
    ```
    **Para Base de Conocimiento**:

    ```sh
    mkdir /opt/citsmart/kb
    ```
    **Para Palavras homónimas**:

    ```sh
    mkdir /opt/citsmart/twinwords
    ```
    **Para Anexos de Base de Conhecimento**:

    ```sh
    mkdir /opt/citsmart/attachkb
    ```
    **Para Upload**:

    ```
	mkdir /opt/citsmart/upload
    ```


## Generación del certificado autofirmado SSL

Para el Wildfly se generará un certificado autofirmado. 
Si tiene un certificado, siga los siguientes pasos.

!!! info "DICAS"

    - Las contraseñas utilizadas en este manual son 123456, pro favor, poner una de su preferencia;

    - Los archivos de certificados manuales usan el sufijo abc, por favor, poner uno de su preferencia;

    - La contraseña predeterminada para cacerts es "changeit" y, por lo tanto, debe usarse para agregar el archivo cer;

    - Si usa diferentes contraseñas y nombres de archivos, cambie antes de ejecutar los comandos.

### Certificado autofirmado:

Creando nuevo alias con DNS (ejemplo itsm.citsmart.com):

```sh
/opt/jdk/bin/keytool -genkey -alias GRPv1 -keyalg RSA -keystore /opt/wildfly/standalone/configuration/GRPv1.keystore -ext san=dns:itsm.citsmart.com -validity 3650 -storepass 123456
```

Criando alias com IP do servidor do Jboss (exemplo 192.168.0.40):

```sh
/opt/jdk/bin/keytool -genkey -alias GRPv1 -keyalg RSA -keystore /opt/wildfly/standalone/configuration/GRPv1.keystore -ext san=ip:192.168.0.40 -validity 3650 -storepass 123456
```

Exportando certificado para extensão .cer:

```sh
/opt/jdk/bin/keytool -export -alias GRPv1 -keystore /opt/wildfly/standalone/configuration/GRPv1.keystore -validity 3650 -file /opt/wildfly/standalone/configuration/GRPv1.cer
```

### Certificado proprio:

Generar pkcs12 con base en su clave publica na sua chave publica (.crt) y privada (.key)
    
```sh
openssl pkcs12 -export -in abc.crt -inkey abc.key -out abc.p12
```    
    
Después de generar el pkcs12 (.p12) usted genera el archivo keystore (jks) que se agregará al wildfly.
    
```sh
keytool -importkeystore -srckeystore abc.p12 \
        -srcstoretype PKCS12 \
        -destkeystore abc.jks \
        -deststoretype JKS    
``` 

### Para ambos tipos de certificados:

Adicionando certificado en el cacerts del Java:

```sh
/opt/jdk/bin/keytool -keystore /opt/jdk/jre/lib/security/cacerts -importcert -alias GRPv1 -file /opt/wildfly/standalone/configuration/GRPv1.cer
```

**Recuerde de aplicar los permisos para el dueño del wildfly y java jdk**

```sh
chown citsmart:citsmart /opt/jdk1.8.0_172/ -R chown citsmart:citsmart /opt/wildfly-12.0.0.Final/ -R
```

Después de generar el certificado, conecte nuevamente en el jboss-cli y ejecute los comandos siguientes:

```sh
/subsystem=undertow/server=default-server/https-listener=https:read-attribute(name=security-realm)
/subsystem=elytron/key-store=citsmartKeyStore:add(path="abc.jks",relative-to=jboss.server.config.dir,credential-reference={clear-text="123456"},type=JKS)
/subsystem=elytron/key-manager=citsmartKeyManager:add(key-store=citsmartKeyStore,credential-reference={clear-text="123456"})
/subsystem=elytron/server-ssl-context=citsmartSSLContext:add(key-manager=citsmartKeyManager,protocols=["TLSv1.2"])
/core-service=management/security-realm=ApplicationRealm/server-identity=ssl:remove
/core-service=management/security-realm=ApplicationRealm/server-identity=ssl:add(keystore-path="abc.jks", keystore-password-credential-reference={clear-text="123456"}, keystore-relative-to="jboss.server.config.dir",alias="citsmartcloud")
```

Antes de salir del jboss-cli, ejecute el comando reload para aplicar los cambios.

```sh
[standalone\@localhost:9990 /] :reload
```

## Iniciando las soluciones siguiendo dependencias

1. Antes de salir del jboss-cli ejecute el comando reload para aplicar los cambios.

    **Servidor de Base de Datos PostgreSQL**:

    ```sh
    systemctl postgresql start
    ```

    **Servidor de Base de Datos MongoDB**

    ```sh
    /opt/mongodb-linux-x86_64-rhel70-3.4.15/bin/mongod --auth --port 27017
    ```

    **Servidor de Indexación Apache Solr**

    ```sh
    su solr /opt/solr/bin/solr start -s /bin/bash
    ```

    **Servidor de Aplicación Wildfly**

    ```sh
    su citsmart /opt/wildfly/bin/standalone.sh -s /bin/bash
    ```


## Implementación del CITSmart Enterprise


1. Enviar los archivos de implementación fornecidos para el servidor y los mueva para el directorio “deployments”.

    ```sh
    cp CitsmartITSM-Enterprise.war /opt/wildfly/standalone/deployments/
    ```

2. Hacer la implementación del Citsmart Neuro después de finalizar los pasos de la próxima sesión (Acceso al CITSmart Enterprise).


### Acesso al CITSmart Enterprise


1. Para acceder al CITSmart Enterprise, debemos acceder el IP o dirección (registrado en el DNS) y después el puerto y contexto.

    ```sh
    https://example.com:8443/citsmart
    ```

2. El contexto "citsmart" es el estándar de CITSmart Enterprise.

    Primer acceso: Entre con la URL > ```https://example.com:8443/citsmart```

3. Siga los 3 pasos de configuración y empiece a usar la solución CITSmart.

## Implementación del CITSmart Neuro

1. Enviar los archivos de implementación fornecidos para el servidor y los mueva para el directorio “deployments”.

    ```sh
    cp citsmart-neuro-web.war /opt/wildfly/standalone/deployments/
    ```

## Navegadores Soportados

Para el correcto funcionamiento del sistema, se deben utilizar las siguientes versiones mínimas de los principales navegadores:

- EDGE (versión mínima): Microsoft Edge 42.17134.0/ Microsoft EdgeHTML 17.17134;

- Google Chrome (versión mínima): versión 76.0.3809.132 (versión oficial) 64 bits;

- Mozila Firefox Quantum (versión mínima): 69.0 (64 bits)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/17/2019 – Anna Martins
