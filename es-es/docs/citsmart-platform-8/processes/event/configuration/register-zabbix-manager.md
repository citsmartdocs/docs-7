title: Registrar gerente Zabbix
Description: Registrar y mantener los gerentes responsables por lo monitoreo de los elementos de configuración, cuyo estado se va buscar en el Zabbix.
# Registrar gerente Zabbix


Zabbix es una herramienta para monitorear red, servidor y servicios, diseñado
para monitorear la disponibilidad, experiencia del usuario y calidad de los
servicios.

El objetivo de esta funcionalidad es registrar y mantener los gerentes
responsables por lo monitoreo de los elementos de configuración, cuyo estado se
va buscar en el Zabbix. Él permite al usuario relacionar los elementos de
configuración a sus disparadores y a las acciones que es necesario hacer en la
ocurrencia de eventos.

Esta funcionalidad ofrece diversas acciones, como, incluir, cambiar y borrar un
gerente Zabbix.

Antes de empezar
--------------------

Para registrar el gerente Zabbix, es necesario tener registrado la conexión del
CITSmart Event Monitor, horario, categoría de ocurrencia, accion automática y la
conexión del CITSmart Inventory.

Procedimiento
-----------------

1.  Acceder al menú principal Procesos \> Gestión de Evento \> Monitor Zabbix \>
    Gerente Zabbix;

2.  Completar los campos disponibles en cada area;

3.  En el área Ítem de Configuración Padre, es posible registrar el IC en el
    CITSmart con los datos del Host seleccionado. Hacer clic en "Crear EC". Es
    importante recordar que este registro sólo puede ser realizado si no hay un
    EC con la misma identificación del Host:

    -   Informar los datos del elemento de configuración hijo;

    -   Hacer relación entre el servicio Host y el elemento de configuración hijo.
        Cada servicio del host debe estar relacionado con su elemento de configuración hijo.

4.  Hacer clic en "Guardar".


Relacionado
----------

[Registrar categoría de ocurrencia](/es-es/citsmart-7/processes/event/configuration/register-occurence-category.html)

[Registrar Conexión Event Monitor](/es-es/citsmart-7/processes/event/configuration/register-event-monitor-connection.html)

[Registrar horario](/es-es/citsmart-7/processes/event/configuration/register-time.html)

[Configurar conexión Inventory](/es-es/citsmart-7/processes/event/configuration/set-inventory-connection.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/24/2019 – Anna Martins
