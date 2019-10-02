
title: Implementar CITSmart Inventory

# Implementar CITSmart Inventory

CITSmart Inventory es un componente de la plataforma CITSmart que permite recopilar, registrar y administrar información de activos de TI. Permite gestionar el ciclo de vida de los elementos de configuración de su organización desde el proceso de Gestión de Configuración.

![Arquitectura CITSmart EVM y INV](images/cloud-arch-inv-evm.png)

Antes de empezar
-------------

El CITSmart Inventory trabaja en conjunto con el [Monitor de Eventos CITSmart - EVM][1] y como un colector de datos (ej.: paquetes XML) el EVM sirve como repositorios para esta información. Por lo tanto, para activar el inventario, primero debe configurar el EVM.  


## Procedimiento


1. [Instalar][2] el servidor de aplicación Wildfly;
2. Descargar el paquete WAR del componente Inventory;
3. Descomprimir los archivos;  
4. Copiar el paquete a la carpeta de implementación del servidor de aplicaciones Wildfly (ej.: /deployments);  
5. Configurar las [Propriedades del Sistema][3] con los datos de la instancia CITSmart.

## Lo que hacer después

Para probar el Inventory, [configurar][4] las conexiones en la instancia CITSmart.

## Relacionado

[Implementar CITSmart Event Monitor][5]

[Gestión de Configuración y Activos][6]


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>06/25/2019

[1]:/es-es/citsmart-7/additional-features/add-ons/event-monitor.html
[2]:/es-es/citsmart-7/get-started/installation-and-upgrade/perform-installation.html
[3]:/es-es/citsmart-7/get-started/installation-and-upgrade/perform-installation.html#configuracion-del-system-properties
[4]:/es-es/citsmart-7/processes/event/configuration/set-inventory-connection.html
[5]:/es-es/citsmart-7/additional-features/add-ons/event-monitor.html
[6]:/es-es/citsmart-7/processes/configuration/overview.html
