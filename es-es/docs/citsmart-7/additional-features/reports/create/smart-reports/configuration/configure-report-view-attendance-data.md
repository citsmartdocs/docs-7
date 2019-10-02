title: Configurar informe para ver datos de la atención
Description: Demostrar cómo configurar los Smart Reports para utilizarlos en la gestión de la atención (Ticket management).
# Configurar informe para ver datos de la atención


Este documento tiene el propósito de demostrar cómo configurar los Smart Reports
para utilizarlos en la gestión de la atención (Ticket management).

Informes por Ticket/Atención
--------------------------------

*Este informe tiene por objetivo demostrar en un período de tiempo, los tickets
atendidos y el tiempo gastado en cada ticket, así como auxiliar en la
identificación de expiración del tiempo.*

### Procedimiento

1.  Acceder al menú principal Informes \> Informes Smart \> Generador de
    Informes Smart;

2.  Descargar el archivo adjunto "TicketAtención";

3.  Hacer clic en "Importar" y seleccionar el archivo que se descargó;

4.  Seleccionar el informe "RelatorioPorTicketAtendimento" de la lista de
    funcionalidad y hacer clic en "Editar";

5.  Elegir el módulo de título "N/A" y definir los grupos que van a tener
    permiso de ver el informe creado.

### Uso

1.  Acceder al menú principal Informes \> Informes Smart \> Informes Smart;

2.  Hacer clic en Incidentes/Solicitudes y seleccionar el elemento
    "RelatórioPorTicketAtendimento";

3.  Definir los filtros con um período (con las fechas de início y cierre de los
    tickets);

4.  Se presentará una lista con los siguientes datos: Solicitud de servicio,
    tipo, servicio, actividad, estado, solicitante, fecha y hora de la
    solicitud, fecha límite de tiempo, SLA, tiempo de atención (es la suma de
    las entradas de las horas registradas en las ocurrencias del ticket) y fecha
    y hora del cierre (si existe) además de un informe sintético referente al
    contrato elegido;

    -   Se puede hacer clic en el número de solicitud del servicio para mostrar
        más detalles sobre el técnico y las horas gastadas por el mismo para
        atender el ticket.

5.  Esta disponible también ver estos Informes en el dashboard, si así lo
    configura al personalizar el mismo Smart Decisions.

!!! Abstract "ATENCIÓN"

    Existe en la pestaña "Relacionados" en la esquina superior izquierda de la
    pantalla, un conocimiento que instruye sobre la creación personalizada de
    dashboards.

Informe por Técnico y Tiempo Gastado
----------------------------------------

*Este informe tiene por objetivo identificar el tiempo de ociosidad por cada
técnico, una vez que presenta la suma de la cantidad de ticket que cada técnico
ejecutó y la suma de los tiempos ejecutados por cada técnico.*

### Procedimiento

1.  Acceder al menú principal Informes \> Informes Smart \> Generador de
    Informes Smart;

2.  Descargar el archivo adjunto "TecnicoTiempo";

3.  Hacer clic en "Importar" y seleccionar el archivo que se descargó. Haga clic
    en "Editar" y cambiar el nombre del informe con el título "Ticket - Tiempo
    empleado por técnico";

4.  Seleccionar el inorme renombrado y hacer clic en "Editar";

5.  Elegir el módulo del título "N/A" y definir los grupos que van a tener
    permiso de ver el informe creado.

### Uso

1.  Acceder al menú principal Informes \> Informes Smart \> Informes Smart;

2.  Hacer clic en "Incidentes/Solicitudes" y seleccionar el elemento "Ticket -
    Tempo gasto por técnico";

3.  Se presentará una lista con los siguientes datos: Técnico, ticket y tiempo
    gastado.

4.  Esta disponible también ver estos Informes en el dashboard, si así lo
    configura al personalizar el mismo Smart Decisions.

!!! Abstract "ATENCIÓN"

    Existe en la pestaña "Relacionados" en la esquina superior izquierda de la
    pantalla, un conocimiento que instruye sobre la creación personalizada de
    dashboards.




Relacionado
-------

[Personalizar el panel gerencial (Smart Decision)](/es-es/citsmart-7/additional-features/reports/create/dashboard-customize-management-panel-smart-decision.html)

Adjunto
------
[Download-Tecnico tiempo][1]

[Download-Ticket atención][2]



!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Anna Martins


[1]:/es-es/citsmart-7/additional-features/reports/create/smart-reports/configuration/images/tecnico-tempo.citreport

[2]:/es-es/citsmart-7/additional-features/reports/create/smart-reports/configuration/images/ticket-atendimento.citreport
