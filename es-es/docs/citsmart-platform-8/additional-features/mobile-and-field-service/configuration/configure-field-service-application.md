title: Configurar instancia para utilizar la aplicación CITSmart GO
Description: La aplicación CITSmart GO permite atender en modo offline - en las que el operador no tiene internet.
# Configurar instancia para utilizar la aplicación CITSmart GO

La aplicación CITSmart GO permite atender en modo offline - en las que el
operador no tiene internet. Una vez que la aplicación se conecta a Internet,
enviará automáticamente la información al ambiente en producción. Es importante
recordar que la delegación de la solicitud a un empleado debe ser hecha
manualmente por un responsable.

Los asistentes visualizará sólo las solicitudes que se los delegaron.

Antes de empezar
--------------------

1.  Instalar la aplicación CITSmart GO;

2.  En el ambiente - instancia del CITSmart - , configurar las siguientes
    funcionalidades:

    -   Webservice: indicar en el ítem "permisos" los grupos de atención que podrán
      ver los tickets;

    -   Unidad: obtener las coordenadas de la unidad registrada.

Procedimiento
-----------------

***Webservice***

1.  Acceder al menú menu principal Sistema \> Web Service \> Operación del Web
    Service;

2.  En la pestaña **Consulta de Operaciones**, buscar por cada uno de los
    webservices abajo, y después, en cada uno de ellos, hacer clic en "Añadir
    grupo" e incluir el grupo que los atendentes están vinculados:

    -   request_add_attachments

    -   request_updateRequestList

    -   request_userLocation

    -   request_saveRequest

    -   request_uploadAttachment

    -   request_getByUser
    
    -   request_saveRequestNote
    
    -   request_updateRequestNoteList
    
    -   request_updateRequestListGroups
    
    -   request_uploadSignature
    
    -   parameter_query

3.  Hacer clic en "Guardar" después de configurar los grupos en cada webservice.

***Unidad***

1.  Acceder al menú principal Registros Generales \> Gestión de Personal \>
    Unidad:

2.  Buscar por la unidad en la pestaña Búsqueda de Unidades para seleccionar la
    unidad:

3.  En la pestaña Registro de Unidad, con la unidad ya seleccionada, hacer clic
    en "Obtener Coordenadas"

4.  Hacer clic en "Guardar".

Lo que hacer después
----------

Inicie sesión en la aplicación CITSmart GO ya instalada, insertando la dirección
URL, el usuario y la contraseña del ambiente. Comprobar los tickets y hacer la
atención.


Relacionado
-----------

[Manual de utilización del CITSmart GO](/es-es/citsmart-7/additional-features/mobile-and-field-service/apps/citsmart-field-service-manual.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 – Anna Martins
