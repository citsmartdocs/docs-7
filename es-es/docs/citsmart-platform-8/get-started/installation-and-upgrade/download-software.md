Title: Software y Descarga

# Software y Descarga

## Paquetes

!!! info "IMPORTANTE"

    La instalación de CITSmart Enterprise requiere el sistema operativo GNU/Linux con kernel igual o superior al 3.10.

    Recomendamos Red Hat, CentOS, Debian o Ubuntu.


Para ejecución del CITSmart Enterprise, descargaremos los paquetes necesarios conforme
el procedimiento relativo al producto.

### Servidor de la Aplicación Wildfly

!!! note "NOTA"

    En el manual utilizaremos el PostgreSQL.
    Usted puede descargar el paquete para Oracle o MSSQL y hacer los cambios
    igualmente descritos para el PostgreSQL.

1. Descargar el Java JDK8u172 directamente del repositorio oficial jdk-8u172-linux-x64.tar.gz  
2. Descargar los paquetes directamente del repositorio oficial a través del link siguiente: <http://download.jboss.org/wildfly/12.0.0.Final/wildfly-12.0.0.Final.tar.gz>

    ![Java Download](images/java-download.png)

     Figura 1 - Tabla Java

3. Descargar el módulo jdbc para el postgresql:

https://jdbc.postgresql.org/download/postgresql-9.3-1103.jdbc41.jar

### Servidor de la Base de Datos MongoDB

!!! note "NOTA"

      En el manual utilizaremos la distribución GNU/Linux CentOS Linux release
      7.5.1804. Descargue el MongoDB conforme su distribución. La versión del MongoDB debe ser 3.4.

Para localizar la descarga conforme su distribución: <https://www.mongodb.com/download-center#community>

Para la descargar el MongoDB para CentOS 7.5: https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-rhel70-3.4.15.tgz

### Servidor de Base de Datos PostgreSQL/Oracle/MSSQL


!!! note "NOTA"

    En el manual utilizaremos PostgreSQL con descarga del repositorio oficial.

   CITSmart Enterprise es compatible con el PostgreSQL 9.3 o superior, excepto la versión 11, y la descarga será hecha 
   en el momento de configuración de los paquetes.

Se recomienda que la instalación de Oracle o MSSQL sean hechas conforme las informaciones y mejores prácticas de cada fabricante:

   *Oracle:* <https://docs.oracle.com/cd/E11882_01/server.112/e10897/toc.htm>

   *MSSQL:* <https://docs.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server>.

### Servidor de Indexación Apache Solr

La versión homologadaa del Apache Solr es la 6.4.2.

:arrow_down: Este paquete (Solr 6.4.2) y los archivos de configuración (Knowledge Base Confs) se pueden descargar desde el área de relación del socio, en el item *Installation Components*.

### Descarga de los archivos assets para CITSmart

:arrow_down: Este paquete (Assets) se puede descargar desde el área de relación del socio, en el item *Installation Components*.


## Configuración de los Paquetes

!!! note "NOTA"

    Utilizaremos el directorio /opt para la instalación de todos los paquetes para
    CITSmart Enterprise.

    El GNU/Linux con instalación mínima debe estar configurado en las 4 máquinas.

    En este ejemplo, utilizaremos CentOS Linux release 7.5.1804. Se deseas utilizar
    otra distribución, cambiar los comandos conforme la gestión de paquetes.

Después de finalizar las descargas, podremos iniciar la instalación de la solución CITSmart Enterprise.


### Servidor de Base de Datos MongoDB


1. Después de la descarga del MongoDB de la versión 3.4.15, para su correcta distribución, se debe
  hacer la descompresión para el directori /opt

    ``` sh
    tar xvzf mongodb-linux-x86_64-rhel70-3.4.15.tgz -C /opt/*
    ```

    ``` sh
    mkdir -p /data/db
    ```

    ``` sh
	cd /opt/mongodb-linux-x86_64-rhel70-3.4.15/bin/
    ```

    ``` sh
	./mongod
    ```

	<message of unrestricted access \>

2. Debemos crear un directorio para la base e iniciar el MongoDB. Asegúrese que él va subir con permisiones sin restricciones de acceso.

3. Con el MongoDB iniciado, abra otro terminal, acceda el directorio bin del MongoDB y cree la base citsmart definiendo su usuario y contraseña.

    ``` sh
    cd /opt/mongodb-linux-x86_64-ubuntu1604-3.4.5/bin/
    ```

    ``` sh
    ./mongo
    ```

    <message of unrestricted access>

    ```sh
    use admin
    db.createUser({
    user: "admin",
    pwd: "yourpassword",
    roles:[
    { role: "root", db: "admin" },
    { role: "dbOwner", db: "citsmart" }
    ]
    })
    ```
4. Se debe observar el retorno *“Successfully added user”*.  

5. Digite **exit** para salir de la consola del MongoDB.  

6. Retorne al terminal anterior y finalice el proceso del mongodb con CTRL+C.  


### PostgreSQL Database Server


!!! warning "ATENCIÓN"

    Para este documento vamos a usar la versión 9.5 del PostgreSQL. Podemos instalar el PostgreSQL siguiendo los pasos del manual           oficial: https://www.postgresql.org/download/linux/redhat/


1. Posteriormente la instalación del PostgreSQL precisamos crear la base de datos, usuario y contraseña;

    ``` sh
    systemctl start postgresql
    ```

    ``` sh
    su – postgres
    ```

    ``` sh
    psql
    ```

    ```sh
    create user citsmartdbuser with password 'exemple123';
    ```

    <message CREATE ROLE>

    ``` sh
    create database citsmart_db with owner citsmartdbuser encoding 'UTF8' tablespace pg_default;
    ```

    <mensagem CREATE DATABASE>

    ``` sh
    alter role citsmartdbuser superuser;
    ```

    <mensagem ALTER ROLE>

    ``` sh
    \q
    ```

    ``` sh
    exit
    ```

2. Observe el retorno de los comandos analizando la correcta ejecución.

3. Ahora iremos configurar el **/var/lib/pgsql/9.5/data/pg_hba.conf** para permitir
la conexión del Wildfly para la base de datos y usuario del CITSmart. Al final del archivo,
cambiar las líneas:

    Estándar: host all all 127.0.0.1/32 md5   
    Cambiado: host citsmart_db citsmartdbuser IP_Wildfly/32 md5* |

4. Hora de la apertura del listening en el archivo /var/lib/pgsql/9.5/data/postgresql.conf

    Estándar es comentado:

    ``` sh
    listen_addresses = 'localhost'
	```
	Cambiado:

    ``` sh
    listen_addresses = ‘0.0.0.0'
    ```

5. Después de las configuraciones, haga restart en el postgresql.

``` sh
systemctl restart postgresql-9.5.service
```


### Servidor de Indexación Apache Solr

1. Instalar los paquetes unzip y lsof.

2. Descomprimir el JAVA y Solr para /opt/

    ``` sh
    yum install unzip lsof
    ```

	```sh
    tar xzvf jdk-8u172-linux-x64.tar.gz -C /opt/
	```

	```sh
    ln -s /opt/jdk1.8.0_172 /opt/jdk
	```

	```sh
    unzip solr-6.4.2.zip -d /opt/
	```

	```sh
    ln -s /opt/solr-6.4.2 /opt/solr
    ```

    ``` sh
    vim /etc/profile
    ```
    export JAVA_HOME="/opt/jdk"
    export PATH="$JAVA_HOME/bin:$PATH"

    ``` sh
    :wq
    ```

    ``` sh
    source /etc/profile
    ```

3. Cree un usuario para ejecución del Solr con shell falso y con permisión en el
directorio del Solr para el e inicie.

    ``` sh
    groupadd -r solr
	```

	```sh
    useradd -r -g solr -d /opt/solr -s /sbin/nologin solr
	```

	```sh
    chown -R solr:solr /opt/solr-6.4.2/
	```

	```sh
    su - solr -s /bin/bash
	```

	```sh
    bin/solr start
    ```    

4. Descomprima el archivo para configuraciones de la base de conocimiento y ejecute la creación de collection.

    ``` sh
    unzip -x base_conhecimento_configs.zip -d /opt/solr-6.4.2/
    ```

    ```sh
    su - solr -s /bin/bash
    ```

    ``` sh
    bin/solr create -c base_conhecimento -d base_conhecimento_configs -s 2 -rf 2
    ```

5. Observa que el retorno del comando debe ser algo como en el ejemplo siguiente.


Copying configuration to new core instance directory:

```sh
/opt/solr/server/solr/base_conhecimento
```

Creating new core 'base_conhecimento' using command:

```sh
http://localhost:8983/solr/admin/cores?action=CREATE&name=base_conhecimento&instanceDir=base_conhecimento
```
```java
{
"responseHeader":{
"status":0,
"QTime":3223},
"core":"base_conhecimento"}

```



!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/30/2019 – Joao Pelles
