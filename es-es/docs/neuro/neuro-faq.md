Title: FAQ (Neuro)
Description: CITSmart - FAQ

# FAQ (Neuro)

!!! Question "¿Cuál es la diferencia entre crear un formulario a través del menú Formulario y a través del menú Objeto de negocio?"
    La creación a través del menú Formulario se produce de forma 100% manual. A través del menú de objeto de negocio, se puede generar el formulario desde el modelo de base de datos. El formulario generado se puede editar en el menú de registro de formulario.

	¿Cómo creo un menú para acceder a mi proceso de negocio?

	La creación del menú para proceso de negocio se realiza en el propio registro de proceso de negocio, definiendo el campo "Menú asociado".

	Es necesario que esté previamente registrado un menú con dos niveles para que pueda ser vinculado a este proceso de negocio.

	También es necesario que, después de guardar el proceso de negocio con menú asociado, se asigne permiso para el elemento de menú nuevo. La asignación de permisos se puede realizar a través de la pantalla de menú o de la pantalla de Perfil de Acceso.

!!! Question "¿Cómo creo relaciones "muchos para muchos" en el objeto de negocio?"
	Para crear una relación "Muchos para muchos", es necesario crear un objeto de negocio tercero para relacionar los dos objetos de negocio deseados.

	Ej.: Vamos a crear una relación muchos para muchos entre dos objetos, A y B. Para ello, necesitaremos un objeto C que relacionará los dos.

	El objeto A tendrá una relación "uno para muchos" con el objeto C, y el objeto B también tendrá una relación "uno para muchos" con el objeto C.

	Dentro de nuestro objeto C tendremos que tener dos relaciones, uno de ellos "muchos para uno" con el objeto A y el otro "muchos para uno" con el objeto B.

	Así, podemos relacionar un dado del objeto A a varios datos del objeto B, y un dado del objeto B a varios datos del objeto A, a través del objeto de negocio C, teniendo efectivamente una relación "muchos para muchos".

!!! Question "¿Todo flujo de trabajo necesita tener un proceso de negocio relacionado?"
	No todo flujo de trabajo necesita tener un proceso de negocio relacionado. Se puede decir que todo flujo de trabajo principal necesita un proceso de negocio, pero los subprocesos no necesitan otros procesos de negocio para ellos.   
	
	Además, esta regla se aplica sólo a los flujos de integración de procesos, ya que los flujos de integración de servicio no necesitan proceso de negocio relacionado.

!!! Question "¿Hay alguna alternativa para acceder a mis tareas de flujo de trabajo abiertas en un menú personalizado, es decir, fuera de la gestión de tareas?"
	Es posible hacer su propia lista de tareas para acceder a las tareas del flujo de trabajo. Para un tutorial completo, véase la documentación técnica.  

!!! Question "¿Es posible crear componentes personalizados que puedan utilizarse en la creación de formularios?"
	Puede crear sus propios componentes para su uso en el formulario. Para un tutorial completo, véase la documentación técnica.

!!! Question "¿Por qué debo comenzar la construcción de una aplicación utilizando Neuro?"
	Se recomienda que el primer paso a ser ejecutado en Neuro sea el registro de la aplicación o el registro de una conexión de base de datos, de acuerdo con la necesidad de la aplicación.  

!!! Question "¿Cómo funciona la inyección de dependencias propias dentro de un formulario en Neuro? ¿Qué pasos se deben realizar?"
	Para inyectar una dependencia propia, es necesario registrarla antes. Las dependencias que se pueden inyectar dentro de un formulario Neuro son solamente del tipo CSS y Javascript.

	Cree un nuevo registro según el tipo de su dependencia a través del menú "Neuro → Recursos" y suba la dependencia.

	Para importarla en el formulario, seleccione la pestaña del tipo de página que desea importar y elija la pestaña "Dependencias". 

	Haga clic en el icono "+ Agregar" para incluir una nueva dependencia, en el campo "Nombre" escriba el nombre registrado del recurso de su dependencia y seleccione la opción correspondiente. Para más información sobre las dependencias de formulario, véase la documentación técnica.

!!! Question "¿Cómo defino las acciones que deben estar disponibles en cada tarea del flujo de trabajo?"
	Las acciones se registran en las pestañas principales del registro del flujo. Para asociar una acción a una tarea específica, vaya al dibujo del flujo de trabajo, abra las propiedades de aquel elemento, seleccione las acciones deseadas y guarde los cambios.

!!! Question "¿Cómo elimino un elemento del flujo de trabajo?"
	Para borrar un elemento del flujo de trabajo, seleccione el elemento que desea borrar y haga clic en Ctrl + Del.

!!! Question "¿Qué hago cuando se produce el error "Proceso de negocio no informado"?"
	Este error se produce porque el proceso de negocio no se hace referencia en el controller del formulario que inicia el proceso de negocio. Para corregir este problema, acceda al formulario referente al proceso de negocio, e inserte el siguiente comando en el controller de la "Página p/ proceso": $ scope.businessProcessName = 'nombre_proceso_de_negocio'

!!! Question "Cuando registro un subproceso, la información del proceso principal es heredada por el subproceso?"
	No. Al incluir un nuevo subproceso, sea del tipo ESI o del tipo BPE en un flujo de trabajo principal, usted deberá, informar en la pestaña "Atributos", el nombre exacto del subproceso que deberá ser creado manualmente en el registro del flujo de trabajo.

	Todas las informaciones, como acciones y estados del flujo principal deberán ser replicados en el registro del subproceso.

	Resumiendo en pasos, se recomienda seguir el siguiente orden:

	1. Registro del flujo principal;
	2. Registro del subproceso;
	3. Inclusión del elemento de subproceso, haciendo referencia al subproceso ya creado.

!!! Question "¿Cuál es la diferencia entre un flujo de integración de procesos y un flujo de integración de servicios?"
	Los flujos de integración de procesos son flujos de trabajo que tienen tareas ejecutadas por usuarios, pudiendo también poseer tareas automáticas ejecutadas por el sistema.

	Los flujos de integración de servicios, como el propio nombre dice, involucra flujos de trabajo ejecutados en base a servicios del sistema, como integraciones y conversiones, por ejemplo.

	Nada impide que un flujo de integración de procesos utilice un subproceso de integración de servicios, por ejemplo.
	
