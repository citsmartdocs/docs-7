Title: Requerimientos del Sistema

# Requerimientos del Sistema


## Servidor de la Aplicación

CITSmart se ejecuta en el servidor de aplicaciones Wildfly versión 12. Los requerimientos mínimos del sistema requeridos para el servidor de aplicaciones son:

| Recurso | Valor  |
|---------|---------|
| **Memoria** | 8 GB   |
| **CPU**     | 4 CPU's |
| **Disco**   | 80 GB   |

## Servidor de Base de Datos Relacional

CITSmart es compatible con bases de datos PostgreSQL, Oracle y Microsoft SQL Server. Si ya tiene un sistema de gestión de bases de datos corporativas, se puede utilizar para alojar la base de datos de CITSmart. Si no posee y desea instalar un nuevo SGDB sólo para la aplicación, recomendamos el uso de PostgreSQL 9.2 o posterior, con las siguientes configuraciones:

| Recurso | Valor   |
|---------|---------|
| **Memoria** | 4 GB   |
| **CPU**     | 2 CPU's |
| **Disco**   | 80 GB   |

##  Servidor de Base de Datos NoSQL

Para instalar el MongoDB, se recomienda seguir la siguiente configuración:

| Recurso | Valor   |
|---------|---------|
| **Memoria** | 4 GB   |
| **CPU**     | 2 CPU's |
| **Disco**   | 80 GB   |

## Sistema de indexación

Para instalar el Apache SOLR, se recomienda seguir la siguiente configuración:

| Recurso | Valor   |
|---------|---------|
| **Memoria** | 4 GB   |
| **CPU**     | 2 CPU's |
| **Disco**   | 80 GB   |

!!! tip
    Los servicios **SOLR** y **MongoDB** se pueden instalar en el mismo servidor que la aplicación CITSmart. Recomendamos para entornos de producción que separe el servidor de base de datos del servidor de aplicaciones.
   
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/17/2019 – Anna Martins

