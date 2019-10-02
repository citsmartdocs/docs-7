title:  Reclasificar ticket 
Description: Después de crear un ticket, es posible reclasificar su información 
# Reclasificar ticket

Después de crear un ticket, es posible reclasificar su información. Esta acción desencadena un e-mail para el solicitante informando sobre el cambio.
No se permite delegar el ticket a un empleado si la situación es Resuelta.

Antes de empezar
----------------

Para reclasificar un ticket, el usuario necesitas pertenecer al grupo ejecutor,
en la pantalla de grupo, vincular el Flujo a la opción de "Cambiar SLA", además
de tener permiso para "crear" en el flujo de actividad destino, eso cuando la
reclasificación incluye el cambio de actividad, y si es un escenario de flujos
diferentes.

Procedimiento
-------------

1.  Acceder a la funcionalidad por el menú principal Procesos \> Gestión de
    Requerimiento e Incidente \> Ticket;

2.  Seleccionar o buscar el ticket;

3.  Haga clic en el ticket, seleccionar el botón “Más Opciones” y elegir la
    opción "Reclasificar";

4.  Haga los cambios.

!!! Abstract "ATENCIÓN"

    Al reclasificar un ticket es necesario el llenado del campo **Justificación
    de la reclasificación** para que quede registrado para todas las personas
    involucradas en el proceso, las actualizaciones en cuanto a cambios
    relacionados al mismo.


!!! Abstract "REGLA"

    Si cambio es en la descripción del ticket, se mostrará en el correo
    electrónico de notificación (en destaque) el cambio en la descripción.
    Recordar que este correo electrónico de notificación sólo se enviará si ha
    habilitado el envío del mismo en el parámetro "231 - Habilitar el envío de
    correo electrónico cuando se edita un incidente (S o N - Default:
    S)". La reclasificación incluye una delegación implícita para el Grupo
    o el Asunto de destino, en versiones anteriores, el usuario tenía que:
    reclasificar, capturar la actividad y delegar a otro grupo.

Lo que hacer después
--------------------

Verificar en la pagina de tickets relacionados si tuvo la reclasificación.

Relacionado
-----------

[Registrar grupo](/es-es/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Crear flujo de trabajo](/es-es/citsmart-7/workflow/use/create-flow.html)

[Configurar permiso de acceso de la gestión de solicitudes/incidentes](/es-es/citsmart-7/processes/tickets/configuration/access-ticket-management.html)

[Configurar parametrización - ticket](/es-es/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROfIFL9F-3s-gomHNzudBEy)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 – Larissa Lourenço
