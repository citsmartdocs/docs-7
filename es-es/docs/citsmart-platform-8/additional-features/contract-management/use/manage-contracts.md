title: Administrar los contratos
Description: Gestionar los contratos ya registrados en el sistema.
# Administrar los contratos

La administración de los contratos se utiliza con el objetivo de gestionar los
contratos ya registrados en el sistema. Este proceso permite comprobar, agregar
y borrar servicios, además de disponer de vínculos para la creación de OS, de
factura y notificación.

Antes de empezar
--------------------

Es necesario el registro previo del grupo, contratos, servicios y modelo de
correo electrónico. También es imprescindible el registro del acuerdo de nivel
de servicio (general).

Para crear una orden de servicio, es necesario que el usuario tenga permiso para
abrir OS y registrar el servicio del tipo "Orden de servicio", vincular el
servicio al contrato, vincular el acuerdo de nivel de servicio del tipo "OS -
Resultados esperados "al servicio. De igual modo, es imperativo registrar las
actividades, con sus respectivos valores, siendo un costo total o calculado por
fórmula, del servicio del contrato. Todas estas acciones serán explicadas a lo
largo de este artículo..

Procedimiento para vincular un servicio al contrato
-------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo del contrato y seleccionar un contrato. A
    continuación, hacer clic en "Buscar";

3.  Hacer clic en la pestaña "Servicios del Contrato" y luego en el botón
    "Agregar Servicio al Contrato";

4.  Completar los campos necesarios. Para vincular un flujo de servicio, hacer
    clic en el icono "+" del flujo y seleccionar un flujo, después, hacer clic en
    "Guardar".

    !!! Abstract "ATENCIÓN"

        Si es necesario hacer uso de más de un flujo, es importante informar cuál
        es el principal.

5.  Después de completar los campos, hacer clic en "Guardar".

Procedimiento para vincular varios servicios al contrato
------------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Servicios del Contrato" y después en "Agregar
    Servicios al Contrato";

4.  Completar los campos necesarios. Para vincular un flujo de servicio, hacer
    clic en el icono "+" del flujo y seleccionar uno de ellos, después hacer clic
    en "Guardar".

    !!! Abstract "ATENCIÓN"

        Si es necesario hacer uso de más de un flujo, es importante informar cuál
        es el principal.

5.  Después de completar los campos, hacer clic en "Guardar".

Procedimiento para verificar los servicios del contrato
-----------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Se presentarán todos los servicios que están vinculados al contrato. Si
    desea buscar un servicio específico, introduzca su nombre en el campo
    de **Búsqueda Servicios del Contrato** y haga clic en "Búsqueda".

Procedimiento para editar las informaciones del vínculo de servicio al contrato
-----------------------------------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ello. Después, hacer
    clic en "Búsqueda";

3.  Hacer clic en "Servicios del Contrato", busque por un servicio y luego hacer
    clic en el icono "Editar el servicio" del servico para editar;

4.  Cambiar los datos conforme la necesidad y hacer clic en "Guardar".

Procedimiento para vincular SLA específico al servicio del contrato
-----------------------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ello. Después, hacer
    clic en "Buscar";

3.  Hacer clic en "Servicios del Contrato" y después en el icono "Acuerdos de Nivel de Servicio" del servicio.
    Hacer clic en "Crear acuerdo específico" para el servicio que se va
    presentar;

4.  Completar los campos necesarios con las siguientes recomendaciones:

       +   Si se informa el tipo de acuerdo como **Disponibilidad**, además de los
       campos generales, será necesario informar el índice de disponibilidad,
       es decir, definir el porcentaje de disponibilidad del servicio;

       +   Si se informa el tipo de acuerdo como **Fallas repetitivas**, además de
       los campos generales, será necesario informar la cantidad de glosas y el
       porcentaje de descuento. Recordar que es posible informar otros datos
       del acuerdo de servicio por fallas repetitivas al hacer clic en el
       icono "+";

       +   Si se informa el tipo de acuerdo como **OS - Resultados esperados**,
       además de los campos generales, será necesario informar los datos de
       resultados esperados y los niveles de calidad exigidos (resultados
       esperados, límites, glosa y límite de la glosa);

       +   Si se informa el tipo de acuerdo como **Tiempo (fases)**, además de los
       campos generales, será necesario definir los plazos de SLA (acuerdo de
       nivel de servicio), teniendo en cuenta la prioridad.

    !!! Abstract "ATENCIÓN"

        Después de "N" minutos configurados, y si no ha realizado ninguna acción
        en la solicitud del servicio, el sistema asignará Prioridad y escalará el
        Grupo que fueron configurados para ejecutar la solicitud del servicio.

    +   Si informa el tipo de acuerdo como **Información diversa capturada de otras fuentes**, será necesario informar los datos de         acuerdo de servicio (el valor límite, la unidad, la glosa y el límite de la glosa). Para copiar, editar o borrar el acuerdo de nivel     de servicio registrado, siga los pasos:

        +  Para editar o borrar un acuerdo de nivel de servicio que se ha agregado
           al servicio de contrato, simplemente hacer clic en el icono "Editar el servicio" al lado del
           acuerdo;

        +  Para copiar un acuerdo de nivel de servicio que se agregó al servicio
           del contrato, simplemente hacer clic en el icono "Copiar el Acuerdo a otro servicio" al lado del acordo;

5.  Hacer clic en "Guardar".

Procedimiento para vincular SLA Global al servicio del contrato
-------------------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hay dos formas de vincular el SLA global al Servicio del Contrato, siendo:

**Primera forma:**

1.  Hacer clic en la pestaña "Servicios del Contrato" y después en "Gestionar
    SLAs Globales";

2.  Seleccionar el acuerdo de nivel de servicio para vincular al Servicio del
    Contrato. Al seleccionar este acuerdo, se presentará una lista con los
    Servicios del Contrato;

3.  Seleccionar los servicios y hacer clic en "Guardar" para vincular el SLA con
    los servicios.

**Segunda forma:**

1.  Hacer clic en la pestaña "Servicios del Contrato" y después en el icono "Acuerdos de Nivel de Servicio" del
    servicio. Hacer clic en "Vincular Acuerdo" y completar los campos
    necesarios;

2.  Hacer clic en "Guardar";

3.  Después de hacer el vínculo del acuerdo de nivel de servicio al servicio,
    hacer clic en "Activar" para que se active el SLA.

Procedimiento para registrar actividades de servicio del contrato
---------------------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Servicios del Contrato" y después en el icono "Actividades del Servicio" de
    uno de los servicios;

4.  Hacer clic en "Agregar Nueva Actividad";

5.  Completar los campos necesario con las siguientes recomendaciones:

    !!! Abstract "ATENCIÓN"

        Al informar si desea contabilizar las solicitudes, recordar que la
        contabilización se hará de las solicitudes "cerradas", en el período de la
        OS (Orden de Servicio), del servicio del tipo solicitud/incidente.

    +  Si se informa el tipo de costo como **Costo Total**, además de los campos
    generales, será necesario indicar el costo total a la complejidad de la
    actividad;

    +  Si se informa el tipo de como **Fórmula**, además de los campos generales,
    será necesario seleccionar una fórmula. Después de elegir, completar los
    campos exhibidos (horas, complejidad y cantidad).

6.  Hacer clic en "Guardar".

Procedimiento para verificar el desempeño del contrato
----------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Servicio del Contrato" y después en "Desempeño del
    Contrato".

Procedimiento para borrar el vínculo de los servicios con el contrato
-------------------------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Servicios del Contrato", seleccionar un servicio
    para borrar. Después, apertar en "Remover Servicios del Contrato";

4.  Hacer clic en "OK" para confirmar.

Procedimiento para crear las órdenes de servicio
----------------------------------------------------

*Orden de Servicio es un documento que proporcionará el permiso de ejecución
relativo a algún servicio.*

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Órdenes de Servicio" y después en "Crear Orden de
    Servicio";

4.  Completar los campos necesarios.

    !!! Abstract "ATENCIÓN"

        Recordar que si el parámetro 243 está habilitado, se añadirá el campo
        Grupo de suscripciones.

        Después del completar los campos, se realizará el redondeo del costo
        total, después de la suma de los costos totales de cada actividad del
        servicio.

5.  Hacer clic en "Guardar Datos".

Procedimiento para verificar las informaciones de la orden de servicio
--------------------------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Órdenes de Servicio" y utilizar los botones en la
    barra (todas, en creación, solicitada, autorizada, aprobada, ejecutada,
    ejecutada y cancelada) para verificar las órdenes de servicio por situación.
    También puede buscar las órdenes de servicio por período;

4.  Al lado de cada registro de orden de servicio, se mostrarán iconos que
    permitirán la edición de OS, impresión de OS y RA (informe de actividad),
    generación de RA y ejecución de OS.

Procedimiento para editar el orden de servicio
--------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Órdenes de Servicio" y buscar por el orden de
    servicio;

4.  Hacer clic en el icono "Editar a OS" del OS para editar;

5.  Cambiar los datos según sea necesario y hacer clic en "Guardar".

Procedimiento para imprimir el orden de servicio
----------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Órdenes de Servicio" y buscar por el orden de
    servicio;

4.  Hacer clic en el icono "Imprimir a OS" para generar el informe del OS en PDF para la
    impresión;

5.  Hacer clic en el icono "Imprimir a OS" para generar el informe del OS en Excel para la
    impresión.

!!! Abstract "ATENCIÓN"

    El Informe de Actividad sólo puede generarse a partir de las órdenes de
    servicio con una situación "Aprobado"

Procedimiento para generar el informe de actividad (RA)
-----------------------------------------------------------

*El R.A (Informe de Actividades) sirve para comprobar que el servicio fue
entregado.*

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Órdenes de Servicio" y después en la pestaña
    Aprobadas;

4.  Hacer clic en el icono "Gerar RA" del OS aprobado y completar los campos necesarios;

5.  Hacer clic en "Guardar".

Procedimiento para ejecutar el orden de servicio
----------------------------------------------------

*Sólo se pueden ejecutar las Órdenes de Servicio que se generan en el informe de
actividades.*

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Órdenes de Servicio". Después de generar el
    informe de las OS, hacer clic en "En ejecución";

4.  Hacer clic en el icono "Expandir OS" del OS para expandir el area y presentar los
    informes de actividad del OS.

5.  Hacer clic en el icono "Ejecutar OS" de uno OS y cambiar su situación para Ejecutada y
    hacer clic en "Guardar datos".

6.  Después de ejecutar el OS, se generará una factura.

Procedimiento para crear factura
------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Facturas" y después en "Crear Factura";

4.  Completar los campos necesarios. Es posible vincular el OS a la factura al
    hacer clic en "Agregar OS", seleccionar el OS ya ejecutado y, después, hacer
    clic en "Asociado" para hacer la adición;

5.  Hacer clic en "Guardar".

Procedimiento para verificar las facturas
---------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Facturas" y utilizar los botones en la barra
    (todas, en creación, solicitada, autorizada, aguardando aprobación y
    aprobadas) para verificar las facturas por situación. También puede buscar
    las facturas por período;

4.  Al lado de cada registro de Orden de Servicio, se mostrarán iconos que van
    posibilitar la edición de la factura (en creación), impresión de la factura
    tanto en formato PDF como en formato Excel y apunte de la situación para
    factura.

Procedimiento para editar las facturas
------------------------------------------

*Sólo las facturas que están "en creación" pueden ser editadas.*

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Facturas" y después en el icono "Editar factura" de la fatura para
    editar. Cambiar los datos según la necesidad y hacer clic en "Guardar".

Procedimiento para imprimir la factura
------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Factura" y buscar por una factura;

4.  Hacer clic en el icono "Imprimir factura" para generar el informe de la factura en PDF para
    impresión;

5.  Hacer clic en el icono "Imprimir factura" para generar el informe de la factura en Excel para
    impresión.

Procedimiento para apuntar la situación de la factura
---------------------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Factura" y buscar por una factura;

4.  Hacer clic en el icono "Apuntar la situación de la factura" de la factura para apuntar una situación.

5.  Cambiar la situación y hacer clic en "Actualizar Situación de la Factura".

Procedimiento para agregar notificación
-------------------------------------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Administración de Contratos;

2.  Hacer clic en el campo contrato y seleccionar uno de ellos. Después, hacer
    clic en "Buscar";

3.  Hacer clic en la pestaña "Notificaciones" y después en "Agregar
    Notificación";

4.  Completar los campos necesarios. Recordar que es posible agregar un usuario
    o grupo al hacer clic en el icono  y buscar y vincular uno elemento;

5.  Hacer clic en "Guardar".


Relacionado
----------------------------------------------
[Acuerdo de Nivel de Servicio](/es-es/citsmart-7/processes/service-level/use/service-level-agreement.html)

[Registrar grupo](/es-es/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Registrar contrato](/es-es/citsmart-7/processes/portfolio-and-catalog/configuration/register-contract.html)

[Definir modelo de e-mail](/es-es/citsmart-7/platform-administration/email-settings/email-templates-configure-email-template.html)

[Registrar servicio](/es-es/citsmart-7/processes/portfolio-and-catalog/use/register-a-service.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROTLt6Tt7uegzqwpXHX5nA2)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 – Anna Martins

