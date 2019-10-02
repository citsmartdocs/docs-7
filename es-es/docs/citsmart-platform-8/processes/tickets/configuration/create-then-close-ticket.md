title: Cómo crear y, a continuación, cerrar un ticket
Description: Configurar para que ocurra la creación y cierre del ticket al mismo tiempo.
# Cómo crear y, a continuación, cerrar un ticket


Para las actividades que no necesitan SLA, donde el asistente deseas sólo
formalizar la solicitud y ejecución de la actividad, es posible configurar para
que ocurra la creación y cierre del ticket al mismo tiempo.

Procedimiento
-----------------

1.  Definir el flujo de creación y cierre del ticket:

    -   **1º Modo - Importar el flujo**: es posible importar el flujo con los script ya registrados. Basta
        descargar el adjunto "Fluxo JSON" y acceder a la funcionalidad del flujo
        (Sistema \> Mantenimiento de Flujos), haga clic en "Nuevo", después haga
        clic en "Importar" y seleccionar la opción "JSON". Descargas el archivo
        adjunto y haga clic en "Importar". Después, para verificar el script,
        haga clic en la pestaña "Diagrama" y en el icono de tarea, y después,
        haga clic en la pestaña "Acción de entrada".

    -   **2º Modo - Copiar el guión**: para copiar sólo el script, copiar el contenido del adjunto "Script" y
        acceda la funcionalidad de flujo (Sistema \> Mantenimiento de Flujos),
        haga clic en "Nuveo" y llena los campos necesarios. Después, haga clic
        en la pestaña "Diagrama", diseñar el flujo de creación y cierre de una
        tarea, seleccionar y hacer clic en esa tarea (pequeña caja gris al lado
        de la tarea) en la pestaña "Acción de entrada" . Es necesario copiar el
        RhinoScript en el constructor de expresiones, hacer clic en "Construir
        expresiones" y seleccionar la expresión de registro.

!!! Abstract "ATENCIÓN"

    No se han implementado controles para información de captura pues el
    tiempo de atención y cierre del ticket es muy corto, si es necesario hacer
    lo mismo, será necesario implementar el registro de las informaciones en las
    tablas de captura.


Adjunto
------
[Download-Flujo JSON][1]

[Download-script][2]


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROl8PJLi-kszYhGzr17uvz-)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 – Anna Martins


[1]:/es-es/citsmart-7/processes/tickets/images/fluxo-JSON.json
[2]:/es-es/citsmart-7/processes/tickets/images/script.zip
