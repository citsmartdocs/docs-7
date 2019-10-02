Title: Requisitos do Sistema

# Requisitos do Sistema


## Servidor de Aplicação

O CITSmart é executado no servidor de aplicativos Wildfly versão 12. Os requisitos mínimos do sistema requeridos para o servidor de aplicativos são:

| Recurso | Valor  |
|---------|---------|
| **Memória** | 8 GB   |
| **CPU**     | 4 CPU's |
| **Disco**   | 80 GB   |

## Servidor de Banco de Dados Relacional

O CITSmart é compatível com bancos de dados PostgreSQL, Oracle e Microsoft SQL Server. Se você já tiver um sistema de gerenciamento de banco de dados corporativo, ele poderá ser usado para hospedar o banco de dados do CITSmart. Se você não possui e deseja instalar um novo SGDB apenas para o aplicativo, recomendamos o uso do PostgreSQL 9.2 ou posterior, com as seguintes configurações:

| Recurso | Valor   |
|---------|---------|
| **Memória** | 4 GB   |
| **CPU**     | 2 CPU's |
| **Disco**   | 80 GB   |

##  Servidor de Banco de Dados NoSQL

Para instalar MongoDB, é recomendado seguir a seguinte configuração:

| Recurso | Valor   |
|---------|---------|
| **Memória** | 4 GB   |
| **CPU**     | 2 CPU's |
| **Disco**   | 80 GB   |

## Sistema de indexação

Para instalar Apache SOLR, é recomendado seguir a seguinte configuração:

| Recurso | Valor   |
|---------|---------|
| **Memória** | 4 GB   |
| **CPU**     | 2 CPU's |
| **Disco**   | 80 GB   |

!!! tip

    Os serviços **SOLR** e **MongoDB** podem ser instalados no mesmo servidor que o aplicativo CITSmart. Recomenda-se para ambientes de produção a separação do servidor de banco de dados do servidor de aplicativos.
   
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/17/2019 – Anna Martins

