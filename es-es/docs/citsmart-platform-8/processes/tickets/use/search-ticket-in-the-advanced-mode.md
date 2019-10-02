title:  Buscar ticket en modo avanzado 
Description: Permite refinar la búsqueda por tickets a través de filtros. 
# Buscar ticket en modo avanzado

La funcionalidad permite refinar la búsqueda por tickets a través de filtros.

Antes de empezar
----------------

Para realizar la búsqueda avanzada de los tickets, es necesario el registro
previo del mismo, y poseer llamados abiertos, en cualquier situación y
configurar los siguientes parámetros: 40, 41, 261, 260 (con el valor default
1-Lista sin restricción), 343 (con el valor default 1-Lista sin restricción) el
valor por defecto: "S") y el parámetro 378 (si el usuario indica el valor igual
a 0, el sistema siempre se descargará en segundo plano. Si el usuario deja el
campo en blanco, el sistema limita la descarga en segundo plano a cinco mil
registros. Si el usuario coloca valor superior o inferior a cinco mil registros,
el sistema considera el valor informado por el usuario).

Procedimiento
-------------

1.  Acceder a la funcionalidad por el menú principal Procesos \> Gestión de
    Requerimiento e Incidente \> Ticket;

2.  Haga clic en el botón de menú situado en la esquina superior izquierda de la
    pantalla y después el elemento de "Búsqueda Avanzada";

3.  Llenar los filtros con la información que quieras. Recordando que la
    eficacia de la investigación depende del segmento de algunas reglas de
    permiso por el filtro, tales como: ejecución, delegación, monitoreo,
    visualización, grupo de usuarios, vinculo con el contrato, unidades y
    empleados conectados. Por lo tanto, si el parámetro 61 está habilitado, sólo
    estarán disponibles las unidades vinculadas al contrato al que tiene vínculo
    con los grupos en que pertenece;

4.  Haga clic en "Búsqueda";

5.  Elegir uno de los formatos de archivo (PDF, XLS y CSV) para generar el
    informe. Después de elegir el formato, el sistema verificará el parámetro
    261 y, encontrando registro mayor que la cantidad permitida, aparecerá el
    siguiente mensaje:

    -   "La cantidad de registros encontrados supera la cantidad máxima
        permitida de visualización. Por favor, restablecer los filtros de
        búsqueda";

6.  Sin embargo, si la cantidad de registro devuelta de la búsqueda es menor que
    el limitado en el parámetro 261, entonces el sistema verifica la
    configuración del parámetro 378;

7.  Se comprueba la cantidad de registros para generar el informe en segundo
    plano, si la cantidad es mayor que la cantidad parametrizada, el sistema
    muestra el siguiente mensaje:

    -   "Se está procesando el informe. Una notificación se le enviará cuando
        esté listo"

8.  Si el archivo a ser generado es muy extenso, el sistema disparará una
    notificación en la pantalla principal, informando que su descarga está
    finalizada. Al finalizar, haga clic en el botón "Visualizar" para acceder al
    informe a través del enlace disponible.

Relacionado
-----------

[Crear ticket](/es-es/citsmart-7/processes/tickets/use/create-ticket.html)

[Configurar parametrización - ticket](/es-es/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)

[Configurar parametrización - sistema](/es-es/citsmart-7/platform-administration/parameters-list/configure-parametrization-system.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROfIFL9F-3s-gomHNzudBEy)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 – Larissa Lourenço
