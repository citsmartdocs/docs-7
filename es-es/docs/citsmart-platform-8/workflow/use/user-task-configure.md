title: Configurar actividad de usuario en el workflow
Description: Este documento tiene por objetivo configurar la actividad tarea de usuario dentro del workflow. 
# Configurar actividad de usuario en el workflow 

Al diseña un workflow, es posible insertar diversos elementos, entre ellos, la Actividad de usuario. Este documento tiene como objetivo orientar la configuración de este elemento en el workflow.

Antes de empezar
---------------
Para utilizar el elemento "Actividad de Usuario" es necesario, como mínimo, tener un workflow registrado en la herramienta, conteniendo los elementos de eventos: "inicio" y "fin".


!!! Abstract "NOTA"

    Dentro de la pestaña *Interfaz*, eligiendo el Tipo de Interacción "Formulario Neuro": poseer 2 
    formularios de Neuro distintos y configurados para que el formulario de creación sea mostrado 
    junto al formulario de monitoreo. Es necesario también crear la Plantilla de Ticket para cada uno de 
    los formularios.
   
Procedimiento
------------

1.	Acceder al menú Workflow > Diseño de flujo;
2.	Hacer clic en "Nuevo”;
3.	Hacer clic en la pestaña Diagrama y después en Actividad;
4.	Hacer clic en el elemento de tarea de usuario y arrástrelo al panel de creación de workflow;
5.	Se abrirán las siguientes pestañas de configuración del elemento:

**Identificación**

*	Nombre: nombre de la tarea de negocio;

*	Descripción: detallar la tarea de usuario;

*	Tipo de instancia:

    *	Una solo instancia: sólo puede tener una sola instancia no ejecutada de la tarea en el workflow;
    
    *	Más de una instancia controlada por el workflow: puede tener varias instancias no ejecutadas de la tarea;
    
    *	Crear una instancia para cada usuario: en la asignación, si hay punto y coma en los usuarios, se creará una tarea para cada usuario;

*	Identificador: es una sigla única para la tarea. Se sirve para codificar Rhino y para formularios del Neuro;

*	Cuenta SLA: definir si "Sí" o "No" (el status "SLA Suspendida" aparecerá en la interfaz de gestión de tickets);

*	Percentaje de ejecución: campo informativo de la cantidad que esa tarea del flujo tiene en todo el workflow;

*	¿Es una tarea de aprobación?: definir si "Sí" o "No";

**Asignación**

*	Tipo de destinatario: seleccionar si será para grupo o usuario específico

*	Tipo asignación: definir si la asignación será de ejecución o de monitoreo

*	Grupo/Usuario: seleccionar el grupo/usuário

*	O Expresión: buscar por expresión ya registrada previamente

**Acciones del usuario**

*	Seleccione la acción de registro: buscar por acción ya registrada previamente (por ejemplo: acción de aprobación, es decir, una expresión con esa finalidad);

**Acción de entrada**

*	Construir expresión: definir una expresión directamente
*	Seleccione la acción del registro: buscar por la acción ya registrada previamente

**Acción de salida**

*	Construir expresión: definir una expresión diretamente

*	Seleccione la acción del registro: buscar por la acción ya registrada previamente

**Interfaz**

*	Tipo de interacción: es el modo en que un Cuestionario o un Formulario Neuro se aplicará en la interfaz de gestión de tickets en un status determinado del workflow. La configuración de los elementos que serán visibles se puede definir en el portafolio, o configurada directamente en el elemento Actividad de Usuario (del workflow):

    *	Definido en el portafolio: es posible que una plantilla de ticket (cuestionario o formulario) aparezca puntualmente en un status del workflow, utilizando lo que se configuró en el atributo de servicio "Actividad" (solicitud/incidente) - campos: “Plantilla CREACIÓN” Y “Plantilla monitoreo”. Esta opción es ventajosa cuando se tienen workflows genéricos utilizados por varios servicios.

    *	Formulario estándar: default del sistema 

    *	Formulario Neuro: tiene un identificador para llamar el workflow disparado por este formulario

*	Plantilla (Estándar/Neuro): permite la vinculación de plantilla de ticket.

    !!! Abstract "ATENCIÓN"

        En caso de no ocurrir la vinculación de ninguna plantilla de solicitud de servicio en la pestaña interfaz, el sistema
        subentendirá y aplicará la configuración de un formulario estándar, habilitando la vinculación de elemento de 
        configuración, cambio, problema y solicitud relacionada con el ticket de la pantalla de gestión de solicitud de servicio.
    
*	Permite dirigir a grupo: permite la activación/desactivación de la opción "Dirigir a grupo" en el registro de un ticket;

*	Permite cambio de status: hace visible/invisible las opciones de atención del ticket (Registrada/En curso; Resuelta y Cancelada);

*	Habilita notificación por correo electrónico: hace visible/invisible las opciones de notificación por correo electrónico;

*	Permite delegar atención: permite la activación/desactivación de la opción "Delegar" para que ésta sea visible en el menú de opciones de la gestión de un ticket;

*	Permite cambiar datos de la pantalla: permite la edición de cuestionarios en la pantalla de gestión de ticket.

!!! Abstract "REGLA"    
    
    Las normativas configuradas en el workflow tendrán prioridad en relación a las marcas de la plantilla de solicitud de 
    servicio, pues ésta es un complemento del workflow.
    
**Base de conocimiento**

   *  Vincular base de conocimiento: elegir el conocimiento que desea vincular la tarea de usuario.

!!! Abstract "ATENCIÓN"

    El objetivo principal de esta vinculación de conocimiento es permitir que el asistente de una solicitud/incidente tenga fácil acceso. Una vez que el workflow llegue a la actividad del flujo vinculado a un conocimiento, el botón "Conocimientos" se muestra en la esquina superior derecha de la pantalla de Solicitud/Incidente para dar acceso de lectura al contenido, para ello, tal conocimiento generalmente está escrito en la forma de un paso a paso.
    
    
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/22/2019 – Anna Martins
