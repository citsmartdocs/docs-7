Title: Software e Download

# Software e Download

## Pacotes

!!! info "IMPORTANTE"

    A instalação do CITSmart Enterprise requer sistema operacional GNU/Linux com kernel igual ou superior ao 3.10.

    Recomenda-se Red Hat, CentOS, Debian ou Ubuntu.

Para execução do CITSmart Enterprise, baixar os pacotes necessários conforme
o procedimento relativo ao produto.

### Servidor de Aplicação Wildfly

!!! note "NOTA"

    No manual será utilizado PostgreSQL.
    Pode-se baixar o pacote para Oracle ou MSSQL e fazer as alterações
    igualmente descritas para PostgreSQL.

1. O download do Java JDK8u172 diretamente do repositório oficial
jdk-8u172-linux-x64.tar.gz  
2. Download do pacote diretamente do repositório oficial através do link
abaixo:<http://download.jboss.org/wildfly/12.0.0.Final/wildfly-12.0.0.Final.tar.gz>

    ![Java Download](images/java-download.png)

     Figura 1 - Tabela Java

3. Download do módulo jbdc para o postgresql:

https://jdbc.postgresql.org/download/postgresql-9.3-1103.jdbc41.jar

### Servidor de Banco de Dados MongoDB

!!! note "NOTA"

       No manual será utilizado a distribuição GNU/Linux CentOS Linux release
       7.5.1804. Baixar e MongoDB conforme sua distribuição. A versão do MongoDB deve ser 3.4.

Para localizar o download conforme sua
distribuição: <https://www.mongodb.com/download-center#community>

Para o download do MongoDB para CentOS 7.5:
https://fastdl.mongodb.org/linux/mongodb-linux-x86_64-rhel70-3.4.15.tgz

### Servidor de Banco de Dados PostgreSQL/Oracle/MSSQL


!!! note "NOTA"

    No manual será utilizado PostgreSQL com download do repositório oficial.

O CITSmart Enterprise é compatível com a versão 9.3 do PostgreSQL ou superiores, exceto a versão 11, e o download será feito no
   momento da configuração dos pacotes.

   Recomenda-se que instalações de Oracle ou MSSQL sejam efetuados conforme
   informações e melhores práticas de cada fabricante:

   *Oracle:* <https://docs.oracle.com/cd/E11882_01/server.112/e10897/toc.htm>

   *MSSQL:* <https://docs.microsoft.com/en-us/sql/database-engine/install-windows/install-sql-server>.

### Servidor de Indexação Apache Solr

A versão homologada do Apache Solr é a 6.4.2.

:arrow_down: Este pacote (Solr 6.4.2) e os arquivos de configuração (Knowledge Base Confs) podem ser baixados na área de relacionamento com o parceiro, no item *Installation Components*.

### Download dos arquivos assets para o CITSmart

:arrow_down: Este pacote (Assets) pode ser baixado na área de relacionamento com o parceiro, no item *Installation Components*.


## Configuração dos Pacotes

!!! note "NOTA"

    Será utilizado o diretório /opt para instalação de todos os pacotes para o
    CITSmart Enterprise.

    O GNU/Linux com instalação mínima deve estar configurado nas 4 máquinas.

    Nesse exemplo é utilizado CentOS Linux release 7.5.1804. Caso deseje utilizar
    outra distribuição alterar os comandos conforme o gerenciamento de pacotes.

Com os downloads finalizados dar início a instalação da solução CITSmart Enterprise.


### Servidor de Banco de Dados MongoDB

1. Após baixar o MongoDB da versão 3.4.15 para sua correta distribuição, deve-se
  efetuar a descompressão para o diretório /opt

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

2. Deve-se criar um diretório para a base e iniciar o MongoDB. Note que ele irá subir com permissões irrestritas de acesso.

3. Com o MongoDB iniciado, abrir outro terminal, acessar o diretório bin do MongoDB e criar a base CITSmart definindo o usuário e senha.

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

4. O retorno *“Successfully added user”* deve ser observado.

5. Digitar **exit** para sair do console do MongoDB.

6. Retornar ao terminal anterior e finalize o processo do mongodb com um CTRL+C.


### PostgreSQL Database Server


!!! warning "ATENÇÃO"

    Para esse manual será utilizada a versão 9.5 do PostgreSQL.
    Pode instalar o PostgreSQL seguindo o manual oficial do PostgreSQL através do link:
    https://www.postgresql.org/download/linux/redhat/

1. Após instalar o PostgreSQL precisa-se criar a bases de dados, usuário e senha;

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

2. Observar o retorno dos comandos analisando a correta execução;

3. Configurar o **/var/lib/pgsql/9.5/data/pg_hba.conf** para permitir
a conexão do Wildfly para a database e usuário do citsmart. No final do arquivo
alterar as linhas:

    Padrão: host all all 127.0.0.1/32 md5   
    Alterado: host citsmart_db citsmartdbuser IP_Wildfly/32 md5* |

4. Hora de abrir o listening no arquivo **/var/lib/pgsql/9.5/data/postgresql.conf**

    Padrão está comentado:

    ``` sh
    listen_addresses = 'localhost'
	```
	Alterado:

    ``` sh
    listen_addresses = ‘0.0.0.0'
    ```


5. Após as configurações, dar um restart no postgresql.

``` sh
systemctl restart postgresql-9.5.service
```



### Servidor de Indexação Apache Solr

1. Instalar os pacotes unzip e lsof.

2. Descomprimir o JAVA e Solr para /opt/

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

3. Criar um usuário para execução do Solr com shell falso e com permissão no
diretório do Solr para ele e inicie.

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

4. Descomprimir o arquivo para configurações da base de conhecimento e executar a
criação da collection.

    ``` sh
    unzip -x base_conhecimento_configs.zip -d /opt/solr-6.4.2/
    ```

    ```sh
    su - solr -s /bin/bash
    ```

    ``` sh
    bin/solr create -c base_conhecimento -d base_conhecimento_configs -s 2 -rf 2
    ```


5. Observar que o retorno do comando deve ser algo como no exemplo abaixo.

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
    <b>Updated:</b>09/11/2019 – Larissa Lourenço
