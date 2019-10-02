title:  Crear y ver sub-ticket 
Description: Puede crear sub-ticket a través de la solicitud original y verla después de crearla.
# Crear y ver sub-ticket

La funcionalidad permite registrar un ticket con actividades relacionadas al ticket original.

Antes de empezar
----------------

Es necesario el registro previo del colaborador, contrato y unidad. También es
necesario vincular el grupo al contrato, la unidad al contrato y el contrato al
servicio.

Registrar el portafolio con los servicios y las actividades de solicitud e
incidente. Definir el tiempo de atención de las actividades de solicitud e
incidente.

Vincular las actividades de solicitud e incidente al contrato del servicio.
Configurar el parámetro 385 con el valor 'S'.

Procedimiento
-------------

1.  Acceda a la funcionalidad por el menú principal Procesos \> Gestión de
    Ticket \> Ticket;

2.  Haga clic en el ticket deseado y seleccione la alternativa "Crear sub-ticket por copia" en el menú de opciones;

3.  Llenar los campos necesarios y hacer clic en el botón "Guardar y mantener la
    tarea actual". El sub-ticket será dirigido al grupo ejecutor
    definido en el registro del vínculo de la actividad, el mismo será dirigido
    al grupo ejecutor definido en el parámetro 9;

4.  Recuerde que el sistema enviará correos electrónicos de notificación acerca
    de la creación, escalonamiento, captura, cierre y demás cambios de los
    tickets relacionados para el grupo ejecutor del ticket principal.

5.  Para buscar los tickets relacionados, es necesario marcar el filtro "Mostrar relacionadas" 
    en el área de búsqueda en la pantalla principal de la funcionalidad.

        
!!! Abstract "ATENCIÓN"

    La sub-ticket tiene un flujo propio, por lo que no se cierra junto con 
    el cierre del ticket de origen. Deberá, por lo tanto, ser ejecutada y cerrada de 
    forma autónoma.  
    
!!! Abstract "ATENCIÓN"

    La sub-ticket puede ser reabierta en cualquier momento, independientemente del 
    estado de la solicitud padre (si está reabierta o cerrada).

Relacionado
-----------

[Crear ticket](/es-es/citsmart-7/processes/tickets/use/create-ticket.html)

[Registrar grupo](/es-es/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Registrar colaborador](/es-es/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Registrar unidad](/es-es/citsmart-7/platform-administration/region-and-language/register-unit.html)

[Configurar permiso de acceso de la gestión de solicitudes/incidentes](/es-es/citsmart-7/processes/tickets/configuration/access-ticket-management.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROfIFL9F-3s-gomHNzudBEy)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 - Larissa Lourenço  


