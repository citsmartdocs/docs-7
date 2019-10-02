
title: Implementar o Event Monitor
Description: Módulo que pretende ser un intermediario entre CITSmart y soluciones de los clientes.

# Implementar o Event Monitor

Event Monitor - EVM - es un módulo que pretende ser un intermediario entre CITSmart y soluciones de los clientes (por ejemplo, Nagios, CITSmart Inventory), sirviendo como un repositorio de informaciones de eventos, generado por herramientas de monitoreo o proceso de inventario.

Para activarlo en una instancia del CITSmart, es necesario descargar el paquete WAR y ejecutar la implementación en el servidor de aplicaciones Wildfly, que puede ser el mismo que el CITSmart. Es importante observar que el EVM debe estar disponible en un puerto diferente de la aplicación CITSmart. Además, notamos que el EVM no posee su propia interfaz, porque la gestión es hecha a través de la aplicación CITSmart.

Procedimiento
----------

1. Descargar el paquete war del component EVM;
2. Descomprimir los archivos;
3. Copiar el paquete a la carpeta de implementación del servidor de la aplicación Wildfly;
4. Configurar [Propriedades del Sistema][1] con los datos de acceso del Mongo y de la instancia del CITSmart;

Lo que hacer después
---------

Para probar el EVM, [configurar][2] las conexiones en la instancia del CITSmart.

[1]:/es-es/citsmart-7/get-started/installation-and-upgrade/perform-installation.html
[2]:/es-es/citsmart-7/processes/event/configuration/register-event-monitor-connection.html
