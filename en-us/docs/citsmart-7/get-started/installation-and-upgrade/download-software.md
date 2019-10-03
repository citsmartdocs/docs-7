Title: Software and Download

# Software and Download

## Packages

!!! info "IMPORTANT"

    The CITSmart Enterprise installation requires an operating system GNU/Linux with kernel equal or higher than 3.10.
    We recommend Red Hat, CentOS, Debian or Ubuntu.

To execute the CITSmart Enterprise, we'll download the necessary package, as the procedure about the product.

### Wildfly Application Server

!!! note "NOTE"

    In this knowledge we'll use PostgreSQL.
    You can download the package of Oracle or MSSQL and make the changes as described for the PostgreSQL.

1. Download the package directly of the official repository through the link: http://download.jboss.org/wildfly/12.0.0.Final/wildfly-12.0.0.Final.tar.gz
2. Download directly the Java JDK8u172 of the official repository jdk-8u172-linux-x64.tar.gz:

      ![Java Download](images/java-download.png)

      Figure 1 - Java download list

3. Download the jdbc module for the postgresql.

https://jdbc.postgresql.org/download/postgresql-9.3-1103.jdbc41.jar

### MongoDB Database Server

!!! note "NOTE"

    In the manual we'll use the distribution GNU/Linux CentOS Linux release 7.5.1804.
    Download the MongoDB as its distribution. The version of MongoDB should be 3.4.

To find the download as its distribution:
https://www.mongodb.com/download-center#community

To download the MongoDB for CentOS 7.5:
https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-rhel70-3.4.15.tgz

### PostgreSQL/Oracle/MSSQL Database Server

!!! note "NOTE"

    In the knowledge, we'll use the PostgreSQL with download of official repository.

The CITSmart Enterprise is consistent with PostgreSQL 9.3 or higher, except version 11, and the download will be done when configure the packages.

It's recommended that the Oracle or MSSQL Installation to be done as the information and best practices of each manufacturer:

   *Oracle:* https://docs.oracle.com/cd/E11882_01/server.112/e10897/toc.htm

   *MSSQL:* https://docs.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server

### Apache Solr Indexing Server

The version homologate of the Apache Solr is 6.4.2.

:arrow_down: This package (Solr 6.4.2) and the configuration files (Knowledge Base Confs) can be downloaded in the partner relationship area, in the item *Installation Components*.

### Download of assets files to CITSmart

:arrow_down: This package (Assets) can be downloaded in the partner relationship area, in the item *Installation Components*.

## Package Configuration

!!! note "NOTE"

    We'll use the directory /opt to install all packages to CITSmart Enterprise.

    GNU/Linux with minimum installation should be configured in the 4 machines.

    In this example, we'll use CentOS Linux release 7.5.1804. If you want to use
    other distribution, change the commands as in the package management.

After all the necessary download, we can start the installation of the solution CITSmart Enterprise.

### MongoDB Database Server

1. After download the MongoDB version 3.4.15, for its correct distribution, it's necessary the decompression to the directory /opt

    ``` sh
    tar xvzf mongodb-linux-x86_64-rhel70-3.4.15.tgz -C /opt/
    ```

    ``` sh
    mkdir -p /data /db
    ```

    ``` sh
    cd /opt/mongodb-linux-x86_64-rhel70-3.4.15/bin/
    ```

    ``` sh
    ./mongod
    ```

        <message of unrestricted access>

2. We should create a directory to the base and start the MongoDB. Note that it will upload with access unrestricted permission;

3. With MongoDB started, open another terminal, access the bin directory of MongoDB and create the CITSmart base, setting its user and password;

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

4. It will appear the message "Successfully added user";

5. Type **exit** to leave the MongoDB console;

6. Return to the previous terminal and finish the mongodb process with CTRL+C.


### PostgreSQL Database Server

!!! warning "ATTENTION"

    To this knowledge we'll use the version 9.5 of the PostgreSQL.
    We can install PostgreSQL with the steps in this official manual:
    https://www.postgresql.org/download/linux/redhat/

1. After install the PostgreSQL we can create the database, user and password;

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

2. Note the command return analyzing the correct execution;
3. Now we'll configure the **/var/lib/pgsql/9.5/data/pg_hba.conf**
to allow the Wildfly connection to the database and user of citsmart.
At the end of the file change the lines:

    Default: host all all 127.0.0.1/32 md5  
    Changed: host citsmart_db citsmartdbuser IP_Wildfly/32 md5*

4. Time to open the listening in the file **/var/lib/pgsql/9.5/data/postgresql.conf**;

    Default is commented:

    ``` sh
    listen_addresses = 'localhost'
    ```
    Changed:

    ``` sh
    listen_addresses = ‘0.0.0.0'
    ```

5. After the configuration, restart in the postgresql;

``` sh
systemctl restart postgresql-9.5.service
```

### Apache Solr Indexing Server

1. Install the packages unzip and Isof;

2. Decompress the JAVA and Solr to the /opt;

    ``` sh
    yum install unzip lsof
    ```

	```sh
    tar xzvf jdk-8u172-linux-x64.tar.gz -C /opt/
	```

	```sh
    ln -s /opt/jdk1.7.0_172 /opt/jdk
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

3. Create a user to execute the Solr with fake shell and permission
in the directory Solr, then, start it;

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

4. Decompress the file to the knowledge base configuration and execute the collection creation;

    ``` sh
    unzip -x base_conhecimento_configs.zip -d /opt/solr-6.4.2/
	```

    ```sh
    su - solr -s /bin/bash
    ```

    ``` sh
    bin/solr create -c base_conhecimento -d base_conhecimento_configs -s 2 -rf 2
    ```

5. Note that the command return should be something like the example bellow:

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
    <b>Updated:</b>01/30/2019 - João Pelles  
