Title: Preguntas frecuentes - FAQ

# Preguntas frecuentes - FAQ

## Processos

### Gestión de Tickets

!!! Question "¿Es posible adjuntar documentos a incidentes, solicitudes, problemas y cambios?"   

    Tanto una Solicitud como un Incidente pueden tener documentos adjuntos en su apertura y en su atención, para Problemas y Cambios podrán ser anexados documentos a cada fase de la solución y también, si es necesario, en cada una de las etadas definidas en la solución del problema o cambio.
    Los documentos pueden ser de cualquier tipo (extensión) y su tamaño máximo puede ser definido por el administrador en el parámetro del sistema 278 (el default es 1GB).
    
!!! Question "¿Es posible clasificar la Solicitud/Incidente (Ticket)?"

    Tanto una Solicitud como un Incidente pueden ser categorizados en la etapa de [registro de las actividades en un servicio](https://docs-7.citsmart.com/es-es/citsmart-7/processes/portfolio-and-catalog/use/register-service-activity.html), las categorías se pueden crear en la misma pantalla de registro, en la hora del enlace de la categoría o en las funcionalidades específicas para [Crear categoría de servicio](https://docs-7.citsmart.com/es-es/citsmart-7/processes/portfolio-and-catalog/configuration/create-service-category.html).

!!! Question "¿Cómo acceder a la solicitud de servicio a partir de la notificación de correo electrónico?"
    
    Para acceder a la solicitud de servicio desde la notificación de correo electrónico, proceda de la siguiente manera:
   
    1. Asegúrese de que está conectado al sistema.
    2. Abra la notificación de correo electrónico referente a la solicitud de servicio;
    3. La notificación tendrá el número de solicitud con un hipervínculo, simplemente haga clic en el número, que luego será redirigido a la pantalla de Gestión de servicios presentando la información de la solicitud.

!!! Question "¿Cómo definir un grupo padrón para el atendimiento del primer nivel de la solicitud de servicio?"
   
    Para definir el grupo predeterminado para la atención de primer nivel, proceda de acuerdo con las siguientes instrucciones:
   
    1. Acceda a la funcionalidad de registro de grupo mediante la navegación en el menú principal Acceso y Permiso > Grupo. Se mostrará la pantalla de registro de grupo, mostrando los contratos;
    2. Realizar el registro del grupo de 1º nivel, si no está registrado, y proceder con el llenado de los campos;
    3. Si el grupo de primer nivel ya está registrado en el sistema, realice la búsqueda del grupo y obtenga su número de identificación (ID);
    4. Después de obtener el ID del grupo de primer nivel, acceda a la funcionalidad de Parámetros de CITSmart a través de la navegación en el menú principal. Parametrización > Parámetros CITSmart.
    5. Se mostrará la pantalla Parámetros de CITSmart, haga clic en la pestaña Búsqueda de parámetros de CITSmart
    6. Realice la búsqueda del parámetro "9 - ID Grupo Nível 1"
    7. Seleccione el mismo.
    8. Se mostrará la pantalla de registro del parámetro con el contenido referente al registro seleccionado, en el campo valor, introduzca el número de identificación (ID) del grupo de primer nivel
    9. Haga clic en el botón Grabar para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría.
    
    REGLA: después de la configuración del parámetro, al realizar el registro de una Solicitud de Servicio/Incidente, si no ha informado al grupo para atención del servicio, será escalado el grupo, el cual fue definido en el parámetro para atención de 1º nivel.

!!! Question "¿Cómo configurar las notificaciones de correo electrónico de solicitud de servicios?"
    
    Al registrar una solicitud de servicio, realizar otras acciones y cerrar la misma, el solicitante será notificado.
    
	Para que esta notificación sea enviada es necesario realizar los siguientes procedimientos:
    
    1- Acceda a los Servicios del Contrato relativos al servicio de negocio Gestión de Portafolio > Portafolio de Servicios > Servicio de Negócio > Contrato > Servicios y servicio técnico Gestión de Portafolio > Portafolio de Servicios > Servicio de Negócio > Servicio de Apoyo/Técnico > Contrato > Servicios e informe o modelo de e-mail en los campos:
        
	- "Modelo de correo electrónico Apertura Solicitud/Incidente"
	
        - "Modelo de E-mail en la finalización de Incidentes/Solicitudes"
	
        - "Modelo de E-mail en las demás acciones de Solicitudes/Incidentes" 
        
    REGLA: si notifica los modelos de correo electrónico, no se enviarán las notificaciones.

    2- Acceda a la funcionalidad de Registro de Grupo mediante la navegación en el menú principal Registros Gererales > Gestión de Personal > Grupo;    
    
    3- Se mostrará la pantalla de registro de grupo. Si el grupo ya está registrado en el sistema, realice la búsqueda del grupo;
    
    4- Seleccione el mismo;
    
    5- Se mostrará la pantalla de registro del grupo determinado, defina si las notificaciones de correo electrónico (apertura, progreso y cierre) referentes a las solicitudes, serán de envío obligatorio;
    
    REGLA: si ha determinado que las notificaciones serán obligatorias, al registrar una solicitud de servicio, en la pantalla de Registro de Solicitud de Servicio/Incidente, estas opciones ya estarán seleccionadas, no permitiendo su alteración. Pero si ha determinado que las notificaciones no serán obligatorias, al registrar una solicitud de servicio, estas opciones pueden ser definidas por el responsable del registro de la solicitud.
    
    6- En la pantalla de Registro de Solicitud de Servicio/Incidente, al registrar una solicitud de servicio se establecerá la regla referente a la notificación por e-mail, definida en el registro de grupo.
    
    REGLA: al registrar una solicitud de servicio, se enviará la notificación sólo al grupo ejecutor, el cual es responsable de la atención de la solicitud. Cuando se realiza la ejecución de las demás acciones y cierre de la solicitud de servicio, las notificaciones serán encaminadas solamente al solicitante.

!!! Question "¿Cómo habilitar la regla de escalabilidad de las solicitudes de servicio?"
    
    La regla de escalado de solicitud de servicio está habilitada en la pantalla de Parámetro de CITSmart. Para habilitar esta regla, proceda de la siguiente manera:

    1. En el archivo citsmart.cfg colocar la rutina START_MONITORA_INCIDENTES = TRUE ;
    2. Acceda a la funcionalidad de Parámetros de CITSmart a través de la navegación en el menú principal Sistema > Parámetros CITSmart;
    3. Se mostrará la pantalla de Parámetros de CITSmart, haga clic en la pestaña de Búsqueda de Parámetros de CITSmart;
    4. Busque y cambie el parámetro 190 - ¿ Activa el funcionamiento de las reglas de programación? (Ej.: S o N - Default: 'N') que indica el valor "S" para habilitar escalado de solicitud de servicio;
    5. Busque y cambie el parámetro 31 - Enviar e-mail flujos de ejecución de solicitudes/incidentes (Ej: S o N) informando el valor "S";
    6. Busque y cambie el parámetro 297 - Desactiva el envío de correos electrónicos del sistema (Valores: "S" o "N" Default: "N") informando el valor "N";
    7. También haga los debidos cambios en los siguientes parámetros, según las necesidades y escenario de la instalación: 
    
     - 195: Id plantilla de correo electrónico para envío de solicitud de notificación con un plazo de batir (Ej .: 1);
    
     - 197: Login usuario recibirá reglas de correo electrónico respecto a la solicitud de servicios de programación que expira (Ej.: Consultor);
    
     - 113: Modelo ID de correo electrónico de escalada automática;
    
     - 10: SMTP ENVÍO - Ogiren notificaciones por correo electrónico de las solicitudes de servicio;
    
     - 33: URL para acceder al sistema.
    
    8. Haga clic en el botón Grabar para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría.

!!! Question "¿Cuál es el Impacto del filtro "Grupo Solucionador" en el comportamiento de las encuestas de solicitudes de servicios e incidentes?"
    
    Cuando el filtro "grupo solucionador" está activo, se mostrará sólo las solicitudes cerradas, una vez que al seleccionar este filtro, se entiende que hay la necesidad de presentar el grupo que de hecho solucionó una solicitud, no presentando grupos responsables de tareas ( de acuerdo con el flujo vinculado al servicio de la solicitud) ejecutadas después de que se haya solucionado la solicitud.

    Veamos un ejemplo genérico:
    
    - El servicio A tiene un flujo de calidad vinculado. Después de solucionarse una solicitud referente al servicio A y avanzar el flujo, el grupo responsable será el de calidad y éste terminará el ciclo de vida de la solicitud en cuestión, pero este grupo no es el grupo que solucionó esta solicitud, sólo aprobó la solución y, ha finalizado la solicitud, por lo que no se presentará en el informe generado por la pantalla de búsqueda de solicitudes e incidentes cuando el filtro "Grupo de soluciones" esté marcado con un grupo específico.
    
    - Sin embargo, cuando el filtro "Grupo Solucionador" no está activo, el grupo presentado en el informe o en la encuesta será el grupo correspondiente a la tarea actual de la solicitud, es decir, si la solicitud está cerrada y tiene un flujo de calidad, de calidad como el grupo actual responsable del cierre del ciclo de vida de esta solicitud. Y si la solicitud está en marcha, se presentará el grupo actual responsable de la ejecución de esta solicitud.

!!! Question "¿Por qué la numeración de la solicitud de servicio no siempre seguirá un orden secuencial riguroso/perfecto en la pantalla de solicitud de servicio o en algunos Informes?"
    
    Tanto la pantalla de Solicitud de Servicios como en algunos informes (tales como "Calidad de Atención - SLA"), la ordenación del número de solicitudes sigue un orden secuencial creciente, excepto cuando:
    
    1. Los informes agrupan los datos por algún criterio especial (por ejemplo, por el plazo de SLA, que es lo que sucede en el caso del informe "Calidad de Atención - SLA");
    2. Cuando el recurso denominado Sequence Block es impactado por un factor externo, esto ocurre si:
    - Hay una parada de la aplicación para la actualización de la versión, o el mantenimiento del entorno y posterior retorno.
    - El entorno se agrupa.

!!! Question "¿Por qué el sistema presenta mensaje de fecha inválida al auditar el ticket?"
    
    En la interfaz de la Gestión de Tickets, específicamente en el elemento "Auditoría", al intentar configurar la auditoría de un ticket abierto (definir las fechas de inicio y fin en el filtro), el siguiente error puede ocurrir: el sistema presentará el mensaje de "Fecha Inválida ". Esto porque la funcionalidad necesita que el idioma definido en el sistema y en el explorador utilizado sean idénticos.  
    Si este requisito no se observa, y se produce esta diferencia en los idiomas, al auditar los tickets, el sistema presentará un mensaje imposibilitando obtener el informe pretendido. Es necesario, por lo tanto, igualar el idioma del sistema y del navegador.  

### Gestión de Portafolio y Catálogo

!!! Question "¿Cómo hago el diseño de activos que componen mi servicio?"
   
    Se hace el diseño de activos que componen el servicio utilizando la herramienta de Diseño de Mapa de Servicio que proporciona diseños eficientes y eficaces para la gestión del servicio durante su ciclo de vida, demostrando los ítems de configuración relacionados.

    Para realizar este diseño, proceda de acuerdo con las siguientes instrucciones (ver conocimiento [Configurar atributos del servicio](/es-es/citsmart-7/processes/portfolio-and-catalog/use/configure-services-attributes.html) ):
    
    1. Acceda a la funcionalidad de diseño de mapa del servicio referente al servicio de negocio Gerência de Portafolio y Catálogo > Gestión de Portafolio y Catálogo > Menu Apoyo > Avanzar Portafolio > Catálogo de Servicios > Avanzar Servicio > Mapa de Servicios;
    2. Se presentará la pantalla para el diseño de los activos que componen el servicio de negocio;
    3. Realice el diseño.

!!! Question "¿Cómo vincular colaboradores (usuarios) a un grupo?"
    
    Hay dos formas de vincular a los colaboradores (usuarios) a los grupos.

    A PARTIR DEL REGISTRO DE GRUPO
	
    1. Acceda a la funcionalidad de Registro de Grupo a través de la navegación en el menú principal. Posicione el puntero en la opción Acceso y Permiso y haga clic en la opción Grupo (ver [Registrar grupo](/es-es/citsmart-7/initial-settings/access-settings/user/register-groups.html) );
    2. Se mostrará la pantalla de Registro de Grupo. Si el grupo ya está registrado en el sistema, realice la búsqueda del grupo y seleccione el mismo. Hecho esto, se mostrará la pantalla de registro del determinado grupo;
    3. Haga clic en el icono de agregar del campo Colaboradores, se mostrará la pantalla para búsqueda de colaboradores;
    4. Realice la búsqueda del colaborador que desea vincular al grupo y seleccione el mismo. Después de eso, el colaborador será vinculado al grupo;
    5. Después del vínculo, haga clic en el botón Grabar para realizar la operación, en este caso la fecha, hora y usuario se almacenar automáticamente para una futura auditoría.
    
    A PARTIR DO CADASTRO DE USUARIO
    
    1. Acceda a la funcionalidad de Registro de Usuario a través de la navegación en el menú principal. Sitúe el puntero en la opción Registros Generales, Administración de Personal y haga clic en la opción Usuario (ver [Registrar usuario](/es-es/citsmart-7/initial-settings/access-settings/user/users.html));
    2. Se mostrará la pantalla de Registro de Usuario. Si el usuario ya está registrado en el sistema, realice la búsqueda del usuario y seleccione el mismo. Hecho esto, se mostrará la pantalla de registro del usuario determinado;
    3. Haga clic en el icono Agregar del campo Grupo. Se mostrará la pantalla para la búsqueda de grupos;
    4. Realice la búsqueda del grupo deseado y seleccione la misma. Después de eso, el usuario será vinculado al grupo;
    5. Después del vínculo, haga clic en el botón "Grabar" para realizar la operación, en este caso la fecha, hora y usuario se almacenar automáticamente para una futura auditoría.

!!! Question "¿Cómo relacionar el grupo al contrato?"
    
    Para relacionar grupo al contrato, proceda conforme a las orientaciones abajo:
    
    1. Acceda a la funcionalidad de Parámetros de CITSmart a través de la navegación en el menú principal. Coloque el puntero en la opción Parametrización y haga clic en la opción Parámetros CITSmart. Se mostrará la pantalla de Parámetros de CITSmart, haga clic en la pestaña de consulta de parámetros de CITSmart. Hecho esto, se mostrará la pantalla para la búsqueda de parámetros;
    2. Realiza la búsqueda del parámetro "41 - ¿Hace que el control de vínculo de colaboradores a los contratos (S/N)?" y seleccione. Después de eso, aparecerá la pantalla de registro del parámetro con el contenido referente al registro seleccionado;
    3. En el campo valor, introduzca el valor "S" para que se muestren los contratos en la pantalla de registro de grupo. Hecho esto, haga clic en el botón Grabar para efectuar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría;
    4. Después de configurar el parámetro, acceda a la funcionalidad de registro de grupo a través de la navegación en el menú principal Registros generales > Gestión de Personal > Grupo. Se mostrará la pantalla de registro de grupo, mostrando los contratos (ver [Registrar grupo](/es-es/citsmart-7/initial-settings/access-settings/user/register-groups.html));
    5. Si el grupo que desea vincular al contrato ya está registrado en el sistema, realice la búsqueda del grupo y seleccione el mismo;
    6. Hecho esto, se mostrará la pantalla de registro del determinado grupo;
    7. Seleccione los contratos a los que se vinculará el grupo.

!!! Question "¿Cómo relacionar la unidad al contrato?"
    
    Para relacionar unidad al contrato, proceda de acuerdo con las siguientes directrices:
    
    1. Acceda a la funcionalidad de Parámetros de CITSmart a través de la navegación en el menú principal opción Parametrización > Parámetros CITSmart. Después de eso, aparecerá la pantalla de Parámetros de CITSmart, haga clic en la pestaña de búsqueda de parámetros de CITSmart. Hecho esto, se mostrará la pantalla para la búsqueda de parámetros;
    2. Realice la búsqueda del parámetro "61 - Vincula contratos a unidad" y seleccione el mismo. Después de eso, aparecerá la pantalla de registro del parámetro con el contenido referente al registro seleccionado;
    3. En el campo valor, introduzca el valor "S" para que se muestren los contratos en la pantalla de registro de unidad. Hecho esto, haga clic en el botón Grabar para efectuar la operación;
    4. Después de configurar el parámetro, acceda a la funcionalidad de registro de unidad a través de la navegación en el menú principal Registros Generales > Gestión de personal > Unidad. Se mostrará la pantalla de registro de unidad, mostrando los contratos;
    5. Si la unidad que desea vincular al contrato ya está registrada en el sistema, realice la búsqueda de la unidad y seleccione la misma. Hecho esto, se mostrará la pantalla de registro de la determinada unidad;
    6. Seleccione los contratos, a los que se vinculará la unidad;
    7. Haga clic en el botón Grabar para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría.

### Gestión de Conocimiento

!!! Question "¿Cómo son clasificados según el ranking los documentos en el momento de la consulta de SOLR en la base de conocimientos?"

    Para rankear (colocar) los documentos en el momento de la búsqueda, el Solr genera una puntuación (score) para cada documento.

    Así, el documento que posee la mayor puntuación, es presentado en primer lugar y los demás, con menor puntuación, en secuencia.

    Para calcular la puntuación de los documentos, Solr utiliza un algoritmo default, donde se comprueba la frecuencia del término (term frequency) investigado. Pero, es posible cambiar la puntuación con la utilización de los impulsores (boosts).

    Los impulsores del Solr pueden ser utilizados en dos momentos, en el momento de la indexación o consulta, siendo más común su uso en la búsqueda.

    Algunos impulsores que pueden cambiar el cálculo de la puntuación, en el momento de la búsqueda, son:
    
    -  term^num:donde el "num" es la importancia del término búscado, por ejemplo: incid ^ 2;

    -  y también puede ser utilizado los impulsores de campo y las funciones del dismax y edismax para impulsar la búsqueda.
    
    En el ITSM no se utiliza ningún impulsor, hasta el momento, sólo se utiliza el cálculo default de puntuación del Solr, y al final de la investigación se realiza la ordenación por la puntuación por la cantidad de veces que el conocimiento fue votado/gustado.

    Los impulsores están abiertos para el uso, pero para utilizarlos es necesario un análisis mejor de la importancia de los campos y de los documentos añadidos al Solr, por la base de conocimiento.

!!! Question "¿Cómo configurar el recurso SOLR?"
    
    CONFIGURACIÓN DEL PARÁMETRO
    
    1. Para configurar el parámetro vaya a la pantalla Parametrización > Gestión de Conocimiento;
    2. Busque el parámetro “URL del servidor de SOLR (Ej: http://localhost:8983/solr/collection_name)” ;
    3. Después de indicar la dirección URL del servidor Solr, un ejemplo de URL sería el siguiente: http://localhost:8983/solr/base_conocimiento .

    INDEXACIÓN DE LOS CONOCIMIENTOS EXISTENTES
	
    1. Para indexar los conocimientos vaya en Sistema > Configuraciones > Gestión de conocimiento (Indexación);
    2. Si tiene conocimientos indexados, haga clic en "Eliminar la indexación de base de conocimientos";
    3. Luego haga clic en "Indexar base de conocimiento";
    4. Si se produce algún error, haga clic en "Actualizar el servidor de índices";
    5. Después de hacer clic de nuevo en "Indexar base de conocimiento";
    6. Si se produce algún error, póngase en contacto con el soporte de ITSM.

!!! Question "¿Cuál es el significado de cada privacidad que un conocimiento puede tener en la base de conocimientos?"
    
    - Público: todos los usuarios con acceso en el Portal del Conocimiento poseen acceso, independientemente de si tienen acceso a la carpeta del conocimiento.
    - Confidencial: sólo el autor y el aprobador pueden visualizar el conocimiento.
    - Interno: sólo las personas con permiso en la carpeta del conocimiento pueden visualizar.

!!! Question "¿Es posible la versión de un conocimiento en la gestión del conocimiento?"

    Para ver un conocimiento, abra uno en la interfaz de gestión del conocimiento, haga clic en editar, en la pantalla de información del conocimiento, después haga clic en "Versionar". Es posible también "Archivar la versión anterior" del conocimiento.

### Gestión de Problema

!!! Question "¿Es posible adjuntar documentos a incidentes, solicitudes, problemas y cambios?"   

    Tanto una Solicitud como un Incidente pueden tener documentos adjuntos en su apertura y en su atención, para Problemas y Cambios podrán ser anexados documentos a cada fase de la solución y también, si es necesario, en cada una de las etadas definidas en la solución del problema o cambio.
    Los documentos pueden ser de cualquier tipo (extensión) y su tamaño máximo puede ser definido por el administrador en el parámetro del sistema 278 (el default es 1GB).

!!! Question "¿Cómo habilitar la regla de escalonamiento del módulo de problemas?"
    
    Para habilitar esta regla, proceda de la siguiente manera:
    
    1. Acceda a la funcionalidad de Parámetros de CITSmart a través de la navegación en el menú principal Parametrización > Parámetros CITSmart;
    2. Se mostrará la pantalla de Parámetros de CITSmart, haga clic en la pestaña de Búsqueda de Parámetros de CITSmart;
    3. Se mostrará la pantalla para la búsqueda de parámetros, realice la búsqueda del parámetro"194 - ¿Habilitar el escalonamiento de problema definido en las reglas de escalonamiento?". (Ej.: S o N - Default 'N')" y seleccione el mismo;
    4. Se mostrará la pantalla de registro del parámetro con el contenido referente al registro seleccionado, en el campo valor, informe el valor "S" para activar escalonamiento de cambios;
    5. Haga clic en el botón "Grabar" para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría.

### Gestão de Mudança

!!! Question "¿Es posible evaluar el impacto de los cambios para poder aprobar el registro de cambios?"

    El proceso de riesgos en el cambio comienza en el diseño del portafolio de cambio, donde se indica el "**Tipo de Análisis de Impacto y Riesgo**, que puede ser simplificada o completa. El siguiente paso es, en el registro del cambio, informar los datos del riesgo en la barra lateral izquierda, en el elemento de análisis de riesgo que será mostrado con la indicación definida en el portafolio de cambio:
    
    "**Simplificada**" para una análisis Simplificada en el elemento.
    
    "**Completa**" para un análisis de riesgo completo con definición de Objetivos, Análisis de Impacto y Evaluación de Riesgos.

!!! Question "¿Es posible adjuntar documentos a incidentes, solicitudes, problemas y cambios?"   

    Tanto una Solicitud como un Incidente pueden tener documentos adjuntos en su apertura y en su atención, para Problemas y Cambios podrán ser anexados documentos a cada fase de la solución y también, si es necesario, en cada una de las etadas definidas en la solución del problema o cambio.
    Los documentos pueden ser de cualquier tipo (extensión) y su tamaño máximo puede ser definido por el administrador en el parámetro del sistema 278 (el default es 1GB).

!!! Question "¿Cómo actualizar un Elemento de Configuración directamente por la Solicitud de Cambio?"

    Cuando una RFC pretende realizar la actualización de un EC, es posible cambiar los datos del EC directamente por la pantalla de gestión de cambios. Para ello:
    
    1.  Acceder a la Gestión de Cambio (Procesos > Gestión de Cambio > Cambio); 
    2. Seleccionar la RFC y hacer clic en ella, después hacer clic en "Abrir";
    3. En la interfaz de gestión, hacer clic en el elemento "EC relacionados";
    4. En el elemento acciones, hacer clic en el icono "Cambiar";
    5. Cambiar el EC con la nueva información;
    6. Hacer clic en "Guardar".

!!! Question "¿Cómo definir la obligatoriedad del vinculo del cambio de EC?"
    
    La obligatoriedad del vínculo del cambio con el IC se define en la pantalla de Parámetro del CITSmart. Para definir esta obligatoriedad, proceda conforme a las siguientes directrices:

    1. Acceda a la funcionalidad de Parámetros del CITSmart a través de la navegación en el menú principal Parametrización > Parámetros CITSmart;
    2. Se mostrará la pantalla de Parámetros del CITSmart, haga clic en la pestaña de búsqueda de parámetros del CITSmart;
    3. Se mostrará la pantalla para la búsqueda de parámetros. Realiza la búsqueda del parámetro "85 - ¿Verificar enlace del Cambio relacionado al IC?";
    4. Seleccione el mismo;
    5. Se mostrará la pantalla de registro del parámetro con el contenido referente al registro seleccionado, en el campo valor, informe el valor "S";
    6. Haga clic en el botón "Grabar" para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría;
    7. Después de la configuración del parámetro, cuando se registre un ítem de configuración, será obligatorio el vínculo del cambio.

!!! Question "¿Cómo habilitar la regla de escalabilidad del módulo de cambios?"
    
    La regla de escalado de cambios está habilitada en la pantalla de Parámetro de CITSmart.

    Para habilitar esta regla, proceda de la siguiente manera:

    1. Acceda a la funcionalidad de Parámetros de CITSmart a través de la navegación en el menú principal Parametrización > Parámetros CITSmart;
    2. Se mostrará la pantalla de Parámetros de CITSmart, haga clic en la pestaña de Búsqueda de Parámetros de CITSmart;
    3. Se mostrará la pantalla para la búsqueda de parámetros, realice la búsqueda del parámetro"193 - ¿Permite programar los cambios en las reglas de escalamiento definidos? (Ej: S o N - Default 'N')" y seleccione el mismo;
    4. Se mostrará la pantalla de registro del parámetro con el contenido referente al registro seleccionado, en el campo valor, informe el valor "S" para activar escalonamiento de cambios;
    5. Haga clic en el botón Grabar para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría.

### Gestión de Configuración y Activos

!!! Question "¿Se puede asignar la responsabilidad de un elemento de configuración a un usuario/grupo?" 

    Sí. Es posible asignar al responsable de un EC editando las opciones del mismo (Procesos > Gestión de Configuración > CMDB > Buscar > Editar > Tipo de Responsable > Responsable). Tenga en cuenta que la actualización de un EC puede estar vinculada a la Gestión de Cambio, siendo necesario vincular el ID de una RFC.

!!! Question "¿Cómo actualizar un Elemento de Configuración directamente por la Solicitud de Cambio?"

    Cuando una RFC pretende realizar la actualización de un EC, es posible cambiar los datos del EC directamente por la pantalla de gestión de cambios. Para ello:
    
    1. Acceder a la Gestión de Cambio (Procesos > Gestión de Cambio > Cambio);
    
    2. Seleccionar la RFC y hacer clic en ella, después hacer clic en "Abrir";
    
    3. En la interfaz de gestión, hacer clic en el elemento "EC relacionados"; 
    
    4. En el elemento acciones, hacer clic en el icono "Cambiar";
    
    5. Cambiar el EC con la nueva información;
    
    6. Hacer clic en "Guardar".

!!! Question "¿Cómo configurar el nombre de las fases del ciclo de vida de los EC (Elementos de configuración)?"
    
    La configuración de los nombres de las fases del ciclo de vida del IC se puede realizar desde la pantalla de Configuración del GCAS y desde la pantalla de Parámetros del CITSmart. Para realizar esta configuración, proceda de la siguiente manera:
  
    CONFIGURACIÓN A PARTIR DE LA PANTALLA DE CONFIGURACIÓN DEL GCA
    
    1. Acceda a la funcionalidad de configuración del GCAS mediante la navegación en el menú principal Procesos ITIL > Gestión de Configuración > Configuración del GCAS. Hecho esto, aparecerá la pantalla de configuración de los parámetros (atributos) de gestión de configuración y activos de servicio;
    2. Introduzca los valores de los parámetros (atributos):
    
     - Nombre del Grupo de ICs en la fase Desarrollo (Ej.: ICs en desarrollo)
    
     - Nombre del Grupo de ICs en la fase Producción (Ej: ICs en Producción)
    
     - Nombre del Grupo de ICs en la fase Producción (Ej: ICs en Homologación).
    
    3. Haga clic en el botón Grabar para realizar la operación, donde la fecha, hora y usuario se guardarán automáticamente para una futura auditoría.
    4. Después de la configuración de los parámetros referentes al nombre de las fases del ciclo de vida del IC, en la pantalla de Gestión de ítems de configuración se muestra la descripción de las fases del ciclo de vida del IC, tal como se especifica en el valor del parámetro.
    
	CONFIGURACIÓN A PARTIR DE LA PANTALLA DE PARÁMETROS DEL CITSMART
    
    1. Acceda a la funcionalidad de Parámetros del CITSmart a través de la navegación en el menú principal Parametrización > Parámetros CITSmart.
    2. Después de eso, aparecerá la pantalla de Parámetros de CITSmart, haga clic en la pestaña de búsqueda de parámetros de CITSmart. Se mostrará la pantalla para la búsqueda de parámetros;
    3. Realiza la búsqueda del parámetro "92 - Nombre del Grupo de ICs en la fase Desarrollo (Ej: ICs en Desarrollo)";
    4. Seleccione el mismo. Después de eso, aparecerá la pantalla de registro del parámetro con el contenido referente al registro seleccionado;
    5. En el campo valor, introduzca el nombre del grupo de IC de la fase de desarrollo;
    6. Haga clic en el botón Grabar para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría;
    7. Realiza la búsqueda del parámetro "93 - Nombre del Grupo de ICs en la fase Producción (Ej: ICs en Producción)";
    8. Seleccione el mismo. Después de eso, aparecerá la pantalla de registro del parámetro con el contenido referente al registro seleccionado;
    9. En el campo valor, introduzca el nombre del grupo de IC de la fase de producción;
    10. Haga clic en el botón Grabar para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría;
    11. Realiza la búsqueda del parámetro "94 - Nombre del Grupo IC en la fase Homologación (Ej: ICs en Homologación)";
    12. Seleccione el mismo. Después de eso, aparecerá la pantalla de registro del parámetro con el contenido referente al registro seleccionado;
    13. En el campo valor, introduzca el nombre del grupo de IC de la fase de homologación;
    14. Haga clic en el botón Grabar para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría.

!!! Question "¿Cómo definir la obligatoriedad del vinculo del cambio de EC?"
    
    La obligatoriedad del vínculo del cambio con el IC se define en la pantalla de Parámetro del CITSmart. Para definir esta obligatoriedad, proceda conforme a las siguientes directrices:

    1. Acceda a la funcionalidad de Parámetros del CITSmart a través de la navegación en el menú principal Parametrización > Parámetros CITSmart;
    2. Se mostrará la pantalla de Parámetros del CITSmart, haga clic en la pestaña de búsqueda de parámetros del CITSmart;
    3. Se mostrará la pantalla para la búsqueda de parámetros. Realiza la búsqueda del parámetro "85 - ¿Verificar enlace del Cambio relacionado al IC?";
    4. Seleccione el mismo;
    5. Se mostrará la pantalla de registro del parámetro con el contenido referente al registro seleccionado, en el campo valor, informe el valor "S";
    6. Haga clic en el botón "Grabar" para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría;
    7. Después de la configuración del parámetro, cuando se registre un ítem de configuración, será obligatorio el vínculo del cambio.

!!! Question "¿Para cuál destinatario se hará el envío de notificaciones de EC?"
    
    Las notificaciones de IC se enviarán al destinatario definido en la pantalla de Parámetro de CITSmart.

    Para definir el destinatario, proceda de la siguiente manera:
    
    1. Acceda a la funcionalidad de Parámetros de CITSmart a través de la navegación en el menú principal Parametrización > Parámetros CITSmart.
    2. Se mostrará la pantalla de Parámetros de CITSmart, haga clic en la pestaña de búsqueda de parámetros de CITSmart;
    3. Se mostrará la pantalla para la búsqueda de parámetros;
    4. Realiza la búsqueda del parámetro "90 - Envío de correos electrónicos de notificación IC (1-Grupo, 2-Propietario, 3-Todos)";
    5. Seleccione el mismo;
    6. Se mostrará la pantalla de registro del parámetro con el contenido referente al registro seleccionado, en el campo valor, introduzca el número de identificación del destinatario (1 - Grupo, 2 - Propietario o 3 - Todos);
    7. Haga clic en el botón "Grabar" para realizar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría;
    8. Después de la configuración del parámetro, se realizará el envío de e-mails de notificaciones de IC para el destinatario (grupo, propietario o todos), según se especifica en el valor del parámetro.
    
!!! Question "¿Cuál es el significado de cada estado del inventario de EC?"
    
    - Inventariado - El inventario logró leer la información del IC y se cerró con éxito;
    - Ignorado -En la pantalla de citsmart / pages / evmInventoryConfiguración / evmInventoryConfiguracao.load tenemos una opción para ignorar las máquinas a inventariadas, esta marcación aparece cuando esto ocurre;
    - Inaccesible - Cuando el servidor encuentra el IC, pero no puede traer la información;
    - No inventariado - Cuando no encuentra el IC en la red, pero tiene conocimiento de que ya existió;
    - En ejecución - Durante la lectura del inventario, el IC queda en ese estado.

### Gestión de Eventos

!!! Question "¿Cómo puede la Gestión de Eventos convertirse en una herramienta de monitoreo de negocios?"
    
    ESQUEMA DE WEBSERVICE PARA SISTEMAS LEGADOS (MONITOREO DE NEGOCIOS)
    Es posible conectar el componente EVM con cualquier software, incluso un diferente de los que el módulo de Gestión de eventos normalmente se integra (Nagios, Zabbix e Inventory), siempre y cuando los datos enviados (vía webservice) sigan un padrón preestablecido.

    Una vez que los datos se envían al CITSmart Event Monitor, se pueden crear reglas (por ejemplo, con el EPL de espera) para que determinados eventos se disparen de acuerdo con alguna condición observada en los datos.

    Ejemplo "Hoja/Nómina de pago":
    
    - Digamos que es una regla de una empresa no contratar a más de 5 empleados por sector.
    - El programa de nóminas podría enviar los datos mínimos de cada contratación por departamento (definido en el plan presupuestario de la empresa), de modo que cuando el número de contracción por departamento supera el límite preestablecido, un evento de "exceso de contratación " Podría ser disparado.


## Administración de la Plataforma

!!! Question "¿Cómo configurar la autenticación del Nagios vía LDAP?"
    
    La configuración de autenticación de Nagios a través de LDAP pasa por:
    
    1. Cambie el archivo thruk.conf de la siguiente manera:
    ```sh
    vim /etc/apache2/conf-available/thruk.conf
	```
    <Location /thruk/>
    Options ExecCGI FollowSymLinks
    AuthName "LDAP Authentication"
    AuthType Basic
    AuthBasicProvider ldap
    AuthLDAPURL ldap://auth01.citsmartcloud.com/dc=citsmart,dc=com?uid?sub?(objectClass=*)
    Require ldap-group ou=people,o=citsmartco,dc=citsmart,dc=com
    Require valid-user
    
    2. Ejecutar:
    ```sh
    /etc/init.d/apache2 restart
	```
    ```sh
    /etc/init.d/thruk restart
	```
	```sh
    /etc/init.d/nagios reload
	```
!!! Question "¿Cómo configurar la respuesta automática de encuestas de satisfacción?"
    
    El mecanismo de respuesta automática, que responderá automáticamente a las encuestas de satisfacción de las solicitudes de servicio, se produce cuando la encuesta de satisfacción no es respondida por el usuario, dentro de un plazo definido por el administrador del sistema.

    Para realizar la configuración de las respuestas automáticas, proceda de acuerdo a las siguientes instrucciones:

    1. Configure los siguientes parámetros del sistema que definen el comportamiento del motor de respuesta automática:
    Parámetro 139: Define el plazo máximo, en días, que el usuario tiene para responder la encuesta de satisfacción, antes de que ésta sea respondida automáticamente por el sistema;
    Parámetro 152: Nota default que se asigna a las encuestas de satisfacción que se responden automáticamente. Opciones: OPTIMO, BUENO, REGULAR Y MALO;
    Parámetro 151: Activa o desactiva las respuestas automáticas en el sistema. S para activar y N para desactivar.
    2. Acceda a la funcionalidad de procesamiento por lotes (Sistema > Procesamiento Batch).
    3. Se mostrará la pantalla de registro de procesamiento por lotes, complete los siguientes campos con la respectiva información:
    Descripción: informe la descripción que identificará este proceso. Por ejemplo: "Respuesta automática encuesta de satisfacción";
    Situación: la situación define si este proceso estará activo o inactivo. Cuando se encuentre inhabilitado las solicitudes dejarán de ser respondidas;
    Tipo: seleccionar el tipo "Clase Java";
    Programación: define cuando esta rutina se ejecutará, corresponde al administrador del sistema definir cuál es la mejor hora y frecuencia para la ejecución;
    Contenido: informe el texto: br.com.centralit.citcorpore.quartz.job.AvaliarSolicitacoesNoRespuestas;
    4. Haga clic en el botón Grabar para realizar el registro.
    
	REGLA: a partir del momento de la grabación, en el horario y día programado, las solicitudes no respondidas (con plazo superior al definido en el parámetro 139) serán automáticamente respondidas (con el valor definido en el parámetro 152), si el parámetro 151 está con valor ' S'.

!!! Question "¿Cómo habilitar la rutina de lectura automática de mensajes de correo electrónico?"

    Al enviar un e-mail al soporte del CITSmart se lee la lectura del correo electrónico automático, si el e-mail es referente a una solicitud, se verificará el título del e-mail, si contiene la palabra 'Solicitud' y el "el número de la solicitud, en caso de contener, se almacenará el correo electrónico como ocurrencia en la solicitud referente.

    Para que esta rutina de lectura de correos electrónicos funcione perfectamente, es necesario realizar los siguientes procedimientos:
    
     1.  Instalar la versión de java 7, si tiene versión inferior la rutina no
        funcionará;
     2.  Acceda a la funcionalidad de Parámetros de Citsmart a través de la
    navegación en el menú principal Parametrización > Parámetros
    Citsmart;
    3.  Se mostrará la pantalla de Parámetros de Citsmart, haga clic en la
    pestaña de Búsqueda de Parámetros de Citsmart;
     4.  Se mostrará la pantalla para la búsqueda de parámetros, realice la búsqueda
    del parámetro "23 - SMTP LECTURA - Servidor de entrada de e-mails del
    Service Desk" y seleccionelo;
    5.  Se mostrará la pantalla de registro del parámetro con el contenido referente
    al registro seleccionado, en el campo valor, informe al servidor de entrada
    de correo electrónico (ej .: orion.egrupo.com.br)
    6.  Haga clic en el botón "Grabar" para realizar la operación, en este caso la
    fecha, hora y usuario serán almacenados automáticamente para una futura
    auditoría;
    7.  Realice la búsqueda del parámetro "24 - SMTP LECTURA - Usuario de buzón de
    entrada de mensajes de Service Desk" y seleccionelo;
    8.  Se mostrará la pantalla de registro del parámetro con el contenido referente
    al registro seleccionado, en el campo valor, informe el correo electrónico o
    login de la cuenta de correo electrónico (por ejemplo, soporte.citsmart)
    9.  Haga clic en el botón "Grabar" para realizar la operación, en este caso la
    fecha, hora y usuario serán almacenados automáticamente para una futura
    auditoría.
    10. Realice la búsqueda del parámetro "25 - SMTP LECTURA - Contraseña de buzón
    de entrada de mensajes de Service Desk" y seleccionelo;
    11. Se mostrará la pantalla de registro del parámetro con el contenido referente
    al registro seleccionado, en el campo valor, la contraseña de la cuenta de
    correo electrónico;
    12. Haga clic en el botón *Grabar* para realizar la operación, en este caso la
    fecha, hora y usuario serán almacenados automáticamente para una futura
    auditoría;
    13. Realice la búsqueda del parámetro "26 - SMTP LECTURA - Proveedor del
    servidor de correo del Centro de Servicio (imaps, pops, imap, pop, etc)" y
    seleccionelo;
    14. Se mostrará la pantalla de registro del parámetro con el contenido referente
    al registro seleccionado, en el campo valor, informe el protocolo que será
    utilizado para lectura de e-mails (ej. Imap o pop) y haga clic en el botón
    Grabar para efectuar la operación, En este caso la fecha, hora y usuario se
    almacenan automáticamente para una futura auditoría.
    15. Realice la búsqueda del parámetro "27 - SMTP LECTURA - Puerto del servidor
    de correo electrónico del Service Desk" y seleccionelo.
    16. Se mostrará la pantalla de registro del parámetro con el contenido referente
    al registro seleccionado, en el campo valor, informe el puerto que se
    utilizará para acceder al servidor de correos electrónicos (587 para
    servidor pop o 995 para servidor imap);
    17. Haga clic en el botón *Grabar* para realizar la operación, en este caso la
    fecha, hora y usuario serán almacenados automáticamente para una futura
    auditoría.
    18. Realice la búsqueda del parámetro "28 - SMTP LECTURA - Carpeta de la
    bandeja de entrada de correos electrónicos del Service Desk" y
    seleccionelo.
    19. Se mostrará la pantalla de registro del parámetro con el contenido referente
    al registro seleccionado, en el campo valor, introduzca la carpeta de la
    bandeja de entrada de la cuenta de correo electrónico;
    20. Haga clic en el botón *Grabar* para realizar la operación, en este caso la
    fecha, hora y usuario serán almacenados automáticamente para una futura
    auditoría.
    21. Realice la búsqueda del parámetro "200 - ¿Habilitar rutina para leer los
    nuevos mensajes de correo electrónico de forma automática (por ejemplo, S o
    N - Default 'N') y seleccione el mismo;
    22. Se mostrará la pantalla de registro del parámetro con el contenido referente
    al registro seleccionado, en el campo valor, introduzca el valor "S" para
    activar la rutina de lectura de e-mail automáticamente;
    23. Haga clic en el botón *Grabar* para realizar la operación, en este caso la
    fecha, hora y usuario serán almacenados automáticamente para una futura
    auditoría.


!!! Question "¿Cómo habilitar el Portal del Servicios (Smart Portal)?"
    
    Para que los usuarios tengan acceso al Portal o al Portal Smart, se debe habilitar el mismo de la siguiente forma:
    
    1. Acceda a la funcionalidad de Parámetros de CITSmart a través de la navegación en el menú principal Parametrización > Parámetros CITSmart; Se mostrará la pantalla de Parámetros de CITSmart, haga clic en la pestaña de Búsqueda de Parámetros de CITSmart; Hecho esto, se mostrará la pantalla para la búsqueda de parámetros
    2. Realiza la búsqueda del parámetro "46 - ¿Habilitar Portal como Pantalla de inicio de CITSmart?" y seleccione el mismo. Después de eso, aparecerá la pantalla de registro del parámetro con el contenido referente al registro seleccionado;
    3. En el campo valor, introduzca el valor "S" para habilitar el portal como pantalla de inicio. Hecho esto, haga clic en el botón "Grabar" para efectuar la operación, en este caso la fecha, hora y usuario serán almacenados automáticamente para una futura auditoría;
    4. Después de configurar el parámetro, al iniciar sesión en el sistema, se mostrará como pantalla inicial el Portal.

!!! Question "¿Cómo habilitar la encuesta de satisfacción?"
    
    La encuesta de satisfacción es la evaluación de la atención de la solicitud hecha a través de la notificación por e-mail.

    Para habilitar esta encuesta de satisfacción, proceda conforme a las siguientes directrices:
    
    1. Cree la plantilla de correo electrónico (la plantilla de correo debe contener la siguiente palabra clave: $ {LINKPESQUISASATISFACAO});
    2. Acceda a la funcionalidad de Parámetros de CITSmart a través de la navegación en el menú principal Parametrización > Parámetros CITSmart.
    3. Se mostrará la pantalla de Parámetros de CITSmart, haga clic en la pestaña de Búsqueda de Parámetros de CITSmart;
    4. Realiza la búsqueda del parámetro "31 - Enviar e-mail flujos de ejecución de solicitudes/incidentes";
    5. Seleccione el mismo;
    6. Se mostrará la pantalla de registro del parámetro con el contenido referente al registro seleccionado, en el campo valor, informe el valor "S" para que sea habilitado el envío de e-mail referente a las solicitudes de servicio;
    7. Haga clic en el botón Grabar para realizar la operación;
    8. Acceda a los servicios de solicitud, incidente y procedimiento del contrato referente al servicio de negocio Gestión de Portafolio y Catálogo > Gestión de Portafolio > Menú Apoyo > Avanzar Portafolio > Catálogo de Servicios > Avanzar Servicio e servicio tecnico Gestión de Portafolio y Catálogo > Gestión de Portafolio > Menú Apoyo > Avanzar Portafolio > Catálogo de Servicios > Avanzar Servicio y asegúrese de que el modelo de correo electrónico que se creó está informado en el campo "Modelo de correo electrónico en la finalización de solicitudes / incidentes";
    9. Al recibir una notificación por correo electrónico de la solicitud de servicio que ha sido atendida, se mostrará un enlace para realizar la evaluación de la atención. Al hacer clic en el enlace se abrirá una pantalla para la evaluación de la atención.

!!! Question "¿Cómo mejorar el rendimiento de CITSmart Enterprise ITSM?"
    
    El rendimiento del sistema se define como el tiempo que el software tarda en realizar una tarea determinada, ya que este rendimiento es un fuerte atributo de calidad percibido por los usuarios del software.

    Existe la capacidad del sistema para funcionar con más de una instancia, para ello, será necesario utilizar el archivo de configuración (citsmart.cfg), donde es posible activar o inactivar rutinas.

    Para utilizar esta capacidad, debe existir el archivo citsmart.cfg en el directorio:
    ```sh
    \jboss\standalone\configuration\ (quando o Jboss sobe como uma única instância)
    \jboss\domain\configuration\ (quando é utilizado cluster, tem domains e hosts)
    ```
   
    REGLA: donde está $ {valor} reemplaza por los valores correspondientes.
	
    1. START_MODE_RULES=${valor} (Este parámetro define si procesa las reglas de escalado. Introduzca el valor TRUE para activar o FALSE para desactivar);
    2. START_MODE_ITSM=${valor} (Este parámetro define si se muestra la interfaz de ITSM. Introduzca el valor TRUE o FALSE. Si se establece con el valor FALSE, no permitirá abrir las características de incidentes, etc. (del ITSM);
    3. START_MONITORING_ASSETS=${valor}(Este parámetro define si el monitoreo de activos se activará. Introduzca el valor TRUE para activar o FALSE para desactivar);
    4. QUANTIDADE_BACKUPLOGDADOS=${valor} (Este parámetro define la cantidad de elementos de la tabla eliminados que se harán copia de seguridad. Introduzca la cantidad de elementos, por ejemplo: 1000);
    5. Los parámetros siguientes cuando no se activan hacen que el sistema suba con los subprocesos deshabilitados para mejorar el rendimiento del sistema. Es necesario configurar estos parámetros antes del inicio de Jboss para el funcionamiento de los mismos;
    6. START_MONITORA_INCIDENTES=${valor} (Este parámetro define si desactiva el seguimiento de incidentes. Indique el valor TRUE activar o FALSE desactivar);
    7. START_VERIFICA_EVENTOS=${valor} (Este parâmetro define se desativa a verificação de eventos. Informe o valor TRUE ativar o FALSE desativar);
    8. El uso de los parámetros a continuación es opcional. Los mismos hacen la separación del pool de conexión principal con el pool de ejecución del flujo, inventario e informe.
    - JDBC_ALIAS_BPM = java: / jdbc / $ {value} (Este parámetro define el nombre del datasource del flujo. Introduzca el nombre del datasource, ej.: java:/jdbc/citsmartFluxo).
    - JDBC_ALIAS_INVENTORY = java: / jdbc / $ {value} (Este parámetro define el nombre del datasource del inventario. Introduzca el nombre del datasource, ej.: java:/jdbc/citsmart_inventory).
    - JDBC_ALIAS_REPORTS = java: / jdbc / $ {value} (Este parámetro define el nombre del datasource de los informes. Introduzca el nombre del datasource, ej.: java:/jdbc/citsmart_reports).
    9. El parámetro siguiente separa el procesamiento de la rutina de eventos BPM en un grupo de subprocesos independientes del grupo de subprocesos principal del sistema para aliviar el uso de recursos de base de datos y servidor.
    - JDBC_ALIAS_BPM_EVENTOS=java:/jdbc/${valor} (Este parámetro define el nombre del datasource de eventos BPM. Introduzca el nombre del datasource, ej.: java:/jdbc/citsmartBpmEventos).

!!! Question "Como integrar o AD da empresa do cliente no CITSmart Enterprise ITSM que está na cloud ofertada pela CITSmart Corporation?"
    
    Em relação ao LDAP compliance do CITSmart Enterprise ITSM, existem dois cenários:
    
    1. Em ambientes on-demand: há necessidade de conexão ao servidor de diretórios do cliente.
    2. Em ambiente cloud (ofertado pela CITSmart Corporation): há necessidade de habilitar a conexão ao servidor de diretórios do cliente.

!!! Question "¿Cómo reemplazar cada imagen de los logotipos de CITSmart Enterprise ITSM?"
   
    Siempre que sea necesario personalizar correctamente los logotipos de CITSmart Enterprise ITSM, se debe realizar el siguiente procedimiento:
    
    1. Acceder al camino: Sistema > Configuración > Configuración de ambiente; aparecerá tres espacios para subir imágenes:
    
      - Logo inicio: Imagen/Logomarca que aparece en la pantalla inicial de inicio de sesión del sistema;
      
      - Logo portal: Imagen/Logomarca que aparece en el Portal de Servicios del sistema;
      
      - Logo sistema: Imagen/Logomarca que se presenta al acceder al sistema;
      
      - Logo Informe: Imagen/Logomarca que se presenta en los informes del tipo jasper.
	
    2. Realizar upload (pueden ser imágenes diferentes).
    
	REGLA: si el usuario no elige una nueva insignia, el logo predeterminado será el del CITSmart. Por motivos de derechos de autor, este cambio de logo sólo se permite en la versión Enterprise del producto CITSmart ITSM.

    CONFIGURACIÓN MÁS PRECISA DE LA IMAGEN PARA INFORMES JASPER
	
    El usuario tiene acceso a las propiedades de la imagen que aparecerá en los informes.

	REGLA: si la imagen personalizada por el usuario no está configurada correctamente en los informes, debe rediseñarse con las proporciones más adecuadas.

!!! Question "¿Qué es necesario para configurar un EC que está físicamente en la red de la empresa del cliente para ser inventariado por el CITSmart Enterprise ITSM que está en la cloud ofrecida por CITSmart Corporation?"
    
    [Original] En la nube, el mongodb y evm / inv quedan en la estructura del cliente, debido a que no es posible conectarse a un rango interno con origen de la nube.
    
    [Para validación] En este escenario específico, los componentes MongoDB, CITSmart EVM y CITSmart Inventory deben instalarse y configurarse dentro de la estructura de red del cliente, ya que no es posible que el CITSmart (Cloud) se conecte a un rango interno de un cliente.

!!! Question "¿Cuál es el límite de tamaño de archivo para Upload en las funcionalidades con estas característica?"
    
    El tamaño de upload de los datos adjuntos es especificado por el administrador del sisma en el parámetro 278, el tamaño por defecto es de 1GB.

!!! Question "¿Qué es la tabla Fato del módulo solicitud de servicio y cómo alimentarla?"
    
    La tabla de FATO solicitud de servicio tiene el propósito de recibir informaciones consolidadas, referentes a la solicitud de servicio.

    Tales como: 
    
              IDSOLICITACAOSERVICO
	      DATAHORASOLICITACAO
	      DIAABERTURA
	      MESABERTURA
	      ANOABERTURA
	      DATAHORAFIM
	      DIAFECHAMENTO
	      MESFECHAMENTO
	      ANOFECHAMENTO
	      IDGRUPOATUAL
	      GRUPOATUAL
	      IDPRIORIDADE
	      NOMEPRIORIDADE
	      IDSERVICOCONTRATO
	      IDCONTRATO
	      NUMEROCONTRATO
	      IDTIPOSERVICO
	      NOMETIPOSERVICO
	      IDPORTFOLIOSERVICO
	      DESCPORTFOLIOSERVICO
	      IDSOLICITANTE
	      SOLICITANTE
	      IDUSUARIORESPONSAVELATUAL
	      TECNICORESPONSAVEL
	      IDTIPODEMANDASERVICO
	      TIPOSOLICITACAO
	      IDCAUSAINCIDENTE
	      CAUSA
	      IDCATEGORIASOLUCAO
	      CATEGORIASOLUCAO
	      IDSTATUS
	      STATUS
	      IDACORDONIVELSERVICO
	      PRAZOSLA_HH
	      PRAZOSLA_MM
	      IDCALENDARIO
	      CALENDARIO
	      DATAHORALIMITE
	      DIALIMITESLA
	      MESLIMITESLA
	      ANOLIMITESLA
	      TAREFAATUAL
	      IDCLIENTE
	      CLIENTE
	      IDFORNECEDOR
	      FORNECEDOR
	      IDCATEGORIASERVICO
	      CATEGORIASERVICO
	      IDCONDICAOOPERACAO
	      NOMECONDICAOOPERACAO
	      IDORIGEM
	      ORIGEMDASOLICITACAO
	      IDMOEDA
	      MOEDA
	      IDTIPOFLUXO
	      FLUXO
	      IDIMPORTANCIANEGOCIO
	      IMPORTANCIASERVICOAONEGOCIO
	      IDLOCALIDADE
	      LOCALIDADE
	      IDUNIDADE
	      UNIDADE
	      URGENCIA
	      IMPACTO
	      RUPTURASLA
	      QTDEREABERTURAS
	      HOUVERECLASSIFICACAO
	      TEMPOATENDIMENTOHH
	      TEMPOATENDIMENTOMM
	      TEMPOATRASOHH
	      TEMPOATRASOMM
	      MAJOR
	      NOTAPESQUISASATISFACAO
	      QTDESOLICITACOESFILHAS
	      QTDESUBSOLICITACOES
	      QTDEBASECONHECIMENTO
	      QTDEPROBLEMAS
	      QTDELIBERACAO
	      QTDEMUDANCAS
	      QTDEICS
	      QTDEAPLICACOES
	      QTDEPROJETOS
	      QTDEANEXOS
	      QTDEAGENDAMENTOATIVIDADES
	      QTDEAGENDAMENTATIVFINALIZADAS
	      CONTRATOAPOIO
	      SERVICOAPOIO
	      CUSTOSERVICO
	      SERVICOINDISPONIVEL
	      QTDEELOGIOS
	      QTDEQUEIXAS
	      PROCEDIMENTOCONTINUIDADE
	      CUSTOINDISPONIBILIDADE
	      IDSERVICO
	      NOMESERVICO
	      IDATIVIDADE
	      NOMEATIVIDADE
	      DATAHORACARGA
	      
    Esta información se alimenta a través de la rutina de procesamiento por lotes del CITSmart, ejecutando los scripts Rhino según el Banco
    
    **Scripts disponibles para:**
    
    - Oracle SQL
    
    - Postgre SQL
        
    - SQL Server
	
    [Baixar Scripts](/pt-br/images/scripts-tabla-fato.zip)

!!! Question "¿Cuáles son los permisos necesarios en la carpeta de destino del backup de la tabla Logdados?"
    
    Los permisos en la carpeta deben ser de lectura y escritura para el usuario que utiliza JBoss.

!!! Question "¿Cuándo ocurre la sincronización de los datos con el LDAP?"
    
    El sistema sincroniza los datos de las credenciales de sus usuarios con LDAP en tres situaciones distintas:
    
    1. En la activación de la aplicación, generalmente siguiendo el procedimiento de actualización de la versión del producto;
    2. Cuando el usuario inicia sesión (el acceso al sistema con su login y contraseña), en ese momento el sistema automáticamente comprueba la autenticación y el permiso del usuario;
    3. En la función Configuración de LDAP, cuando el usuario hace clic en la opción Sincronizar.

!!! Question "¿Cuándo se produce la limpieza de los datos de la tabla Logdatos?"
    
    La rutina de copia de seguridad (backup) de la tabla de registros LogDados elimina los datos de la tabla y se guarda en el archivo, es decir, la tabla se queda limpia después del procesamiento.

!!! Question "¿Por qué los horarios creados por la herramienta son diferentes de la hora actual?"
    
    ESCENARIO
    1. Al crear un ticket, la hora es diferente a la hora real, alternando entre 1 (una) a 3 (tres) horas de retraso o antelación.

    QUÉ VERIFICAR
    1. Archivo de configuración del Banco Postgresql:
     - Postgresql.conf
     - timezone = 'BRAZIL/EAST'
     
    2. En el container cloud:
     - Setting timezone on the operating system. 
     
    3.Configuración de TimeZone en JRE: 
     - https://docs.oracle.com/javase/9/troubleshoot/time-zone-settings-jre.htm#JSTGD362

!!! Question "¿Por qué en algunos informes la misma solicitud aparece más de una vez?"
    
    En algunos informes como por ejemplo el "Informe Incidentes/Solicitudes de Servicios - Detallado", tanto en formato pdf como en el xls, puede existir sí la misma solicitud más de una vez, sin embargo son informaciones distintas porque trata de cada etapa de la solicitud, entonces cada vez que ella "repite" es porque cambia la tarea, o el responsable, o la fase, o la situación, o el grupo solucionador o la fecha hora final de atención.
    
    Ya en otros informes, tales como el "Informe Incidentes/Solicitudes de Servicios" no hay detalle de la solicitud de acuerdo con las actividades y por eso no se muestra la solicitud más de una vez.

!!! Question "¿Por qué el resultado es "Informe Vacío" al generar el informe control porcentual cuantitativo SLA seleccionando en el filtro la situación "en curso" y el "grupo solucionador"?"
    
    No se trata de un error, el campo de grupo de solucionador se completa sólo cuando se termina la solicitud, esto hace que sólo traiga resultados para las situaciones del tipo "Cerrada", incompatible con lo que se está pidiendo/informando en los filtros.

!!! Question "¿El archivo de backup se sobrescribe o tendrá un archivo para cada día?"
    
    Si su rutina es una copia de seguridad al día, se creará un archivo por día, que contiene en el nombre la fecha de su archivo.
    
