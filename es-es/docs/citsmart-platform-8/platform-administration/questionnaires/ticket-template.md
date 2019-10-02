title:  Registrar plantilla de ticket 
Description: Tiene el objetivo de habilitar algunas funcionalidades en la pantalla de solicitud de servicio (ticket).
# Registrar plantilla de ticket

Esta funcionalidad tiene el objetivo de habilitar algunas funcionalidades en la pantalla de solicitud de servicio (ticket).
Esta funcionalidad ofrece acciones diversas, tales como, incluir, cambiar y borrar plantilla de ticket.

Antes de empezar
----------------

La plantilla de ticket del tipo Cuestionario requiere el registro de un
cuestionario previamente.

La plantilla de ticket del tipo Neuro requiere el registro previo de un
formulario del tipo **Neuro** previamente.

Procedimiento
-------------

1.  Acceder al menú principal Sistema \> Plantilla de Ticket;

2.  Hacer clic en "Nuevo";

3.  El Tipo de Plantilla seleccionado establecerá los campos para completar:

    -   **JSP**:esta funcionalidad permite personalizar la pantalla de servicios con
    referencia, principalmente, en la gestión de compras y viajes. Dentro del
    tipo JSP hay sub-tipos previamente registrados. La utilidad de este tipo de
    plantilla sólo se observa en las versiones anteriores a 7.2.3.9. Esta clase
    de plantilla deberá ser manipulada por analista que tenga conocimiento de
    programación JAVA;

    -   **Cuestionario**: incluso si deshabilitada la opción de "Habilitar editar
    cuestionario", esta edición será posible cuando ocurra el registro del
    ticket. Hay dos funciones de aprobación que se pueden configurar, en la
    pantalla de la plantilla de solicitud de servicio o en el mantenimiento del
    flujo. Por regla general, para el sistema, sólo las configuraciones
    realizadas en la pantalla de flujo tendrán validez. La función de aprobación
    existente en la pantalla de plantilla de solicitud de servicio, sólo tendrá
    validez si está vinculada al registro de un formulario JSP en los modelos
    más antiguos del sistema. Los campos de habilitación, a pesar de
    seleccionados por defecto, tendrán su visualización no disponible en el
    momento de creación de ticket, esta visualización ocurrirá con la
    efectividad del registro. En el momento de registro del ticket que tenga un
    formulario del tipo estándar, estarán disponibles en el botón “Menú”, en la
    esquina superior izquierda, sólo las características: EC del Solicitante,
    Adjuntos, Agenda, Liberación, Proyecto, Conocimiento y Lectura de correos
    electrónicos. Todas las funcionalidades de habilitación, que se presentan
    tanto en la pantalla de plantilla de solicitud de servicio, como en la de
    mantenimiento de flujo, sólo tendrán validez las marcas configuradas en la
    pantalla de flujo, pues la primera mencionada es un complemento de la
    segunda. Si la plantilla de solicitud de servicio está vinculada sólo a las
    actividades del portafolio, el sistema va a subentender que el formulario es
    estándar, por lo que no va a cumplir las normativas (habilitación o no de la
    funcionalidad) de la plantilla. Para la regla de reclasificación, donde la
    plantilla de servicio del tipo Cuestionario o Neuro tiene que ser presentado
    para la respuesta del usuario, es necesario que la plantilla o formulario
    esté vinculado a la plantilla de solicitud de servicio concomitantemente con
    la pantalla de mantenimiento del flujo y la actividad del portafolio;

    -   **Neuro**: al seleccionar esta opción, el campo de vinculación de formulario
    Neuro y la página Neuro están disponibles. También puede elegir la
    **versión** del formulario haciendo clic en el botón *Versión específica del
    formulario*. Las reglas del template del tipo Cuestionario son válidas para
    la plantilla del tipo Neuro.

Relacionado
-----------

[Crear flujo de trabajo](/es-es/citsmart-7/workflow/use/create-flow.html)

[Registrar cuestionario](/es-es/citsmart-7/platform-administration/questionnaires/questionaires-management/register-questionnaire.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Larissa Lourenço

