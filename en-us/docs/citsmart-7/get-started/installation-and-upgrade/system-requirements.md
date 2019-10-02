Title: System requirements

# System requirements


## Application Server

CITSmart runs on the Wildfly version 12 application server. The minimum system requirements required for the application server are:

| Resource | Value   |
|---------|---------|
| **Memory** | 8 GB   |
| **CPU**     | 4 CPU's |
| **Disk**   | 80 GB   |

## Relational Database Server

CITSmart is compatible with PostgreSQL, Oracle, and Microsoft SQL Server databases. If you already have an enterprise database management system, it can be used to host the CITSmart database. If you do not have and you want to install a new SGDB only for the application, we recommend using PostgreSQL 9.2 or later, with the following configurations:

| Resource | Value   |
|---------|---------|
| **Memory** | 4 GB   |
| **CPU**     | 2 CPU's |
| **Disk**   | 80 GB   |

## NoSQL Database Server

To install MongoDB, we recommend the following configuration:

| Resource | Value   |
|---------|---------|
| **Memory** | 4 GB   |
| **CPU**     | 2 CPU's |
| **Disk**   | 80 GB   |

## Indexing system

For installation of Apache SOLR, we recommend the following configurations:

| Resource | Value   |
|---------|---------|
| **Memory** | 4 GB   |
| **CPU**     | 2 CPU's |
| **Disk**   | 80 GB   |

!!! tip
     The **SOLR** and **MongoDB** services can be installed on the same server as the CITSmart application. We recommend for production environments that you separate the database server from the application server.

	 
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/22/2019 - João Pelles  
	
