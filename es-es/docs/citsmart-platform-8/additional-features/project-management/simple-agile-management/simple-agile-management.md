Title: Gestión ágil Simple

# Gestión ágil Simple


Simple es una funcionalidad de CITSmart que permite la gestión fácil
y ágil de actividades. Fue creado para gestionar los proyectos de manera
más simple, con recursos para organizar, monitorear y delegar las actividades
entre los miembros de su equipo o individualmente.

El Simple se basa en la metodología Kanban, donde los mismos se organizan
visualmente en un cuadro dispuesto de tarjetas que señalan el progreso del flujo.

En el área de trabajo del Simple, las actividades se insertan y agrupan por
proyectos (en el Simple llamados de Workspaces), panel de tareas (en el Simple
llamados Sprint) y por fin las tareas, que pueden estar en grupos de tarjetas.


!!! warning "ATENCIÓN"    

    El idioma en las columnas que aparecen en la pantalla **Mis notificaciones (icono de 
    campana)** seguirá lo que se estableció en el parámetro 66 (Idioma predeterminado del 
    sistema).
    

Procedimiento
------------

### Crear Workspace

1.  Acceder al menú principal Gestión Integrada \>
    Simple – Gestión Ágil;

2.  Hacer clic en “Workspace” y poner un nombre para crear nuevo Workspace;

    ![pantalla sprint](images/figure-01-simple.png)
    
    Figura 1 - Pantalla Workspace

    -   **1**: busca cualquier información que esté en cualquier otro Workspace, Sprint, 
        Lista o Tarea. Es posible la búsqueda que selecciona las actividades por la fecha 
        estimada de su desarrollo (el período de inicio y conclusión). Para utilizar esta 
        función de búsqueda, se requieren las siguientes instrucciones: 
        
        -   Para el correcto funcionamiento de este campo, es necesario que el Workspace, 
            Sprint y Lista tengan una fecha estimada de inicio y fin;
            
        -   Hacer la búsqueda. El sistema luego devolverá una lista de Workspaces, Sprints y 
            Listas que están entre la fecha mencionada en la búsqueda.    

    -   **2**: crear nueva Sprint

    -   **3**: abreviatura de los nombres de los miembros agregados. Al hacer clic es posible 
        borrar y definir si el miembro será administrador o no

    -   **4**: añadir miembros que participarán de la Sprint
    
    -   **5**: acción de configuración del Workspace y acceso a *Perfiles y permisos*:
    
        -   Los permisos en Workspace y Sprint, cuando se registra el **Administrator**, se 
            seleccionarán de forma predeterminada y no se pueden cambiar. Solo cuando el usuario 
            sea de tipo **Normal** los permisos serán editables. El Administrador del Workspace 
            puede cambiar el gestor del proyecto (permiso del Administrador) en cada Sprint. Si 
            no es el Administrador del área de trabajo, no puede otorgar el permiso del administrador 
            a otro usuario.
            
        -   Con el perfil de tipo **Normal** dentro del Workspace o Sprint, si el usuario marca la 
            checkbox de **Cambiar los permisos de los miembros del Workspace/Sprint**, se liberará 
            el permiso de los otros miembros del proyecto al que pertenecen si un usuario que **no** 
            tiene el perfil de Administrador, puede cambiar el estado de permiso de cada miembro, 
            incluso si no es el Administrador.

3.  Cada Workspace contendrá en su pantalla inicial un resumen de Sprints 
    y sus plazos establecidos:

    -   Atrasadas: presenta el total de las **Sprints** que tenga la "Fecha de entrega" 
        menor que la fecha/hora actual;

    -   Por vencer: presenta el total de las **Sprints** que tenga la "Fecha de entrega" 
        que quedarán vencidas en 24h a partir de la fecha/hora actual;

    -   En el plazo: presenta el total de las **Sprints** que tenga la "Fecha de entrega" 
        mayor que 24h a partir de la fecha/hora actual;

    -   Total: suma de las **Sprints** que están dentro del Workspace.
    
 
!!! warning "ATENCIÓN"

    Para mover un **workspace** cambiando su ordenación, hacer clic y arrastrarlo 
    hasta la posición de prioridad deseada.


### Crear Sprint

1.  Hacer clic en el Workspace creado anteriormente;

2.  Hacer clic en “Sprint”, nombrar y "Guardar”;

3.  Cada Sprint contendrá en su pantalla inicial un contador de **tareas**, 
    horas gastas y planificaciones, totalización de tareas por plazos establecidos 
    y porcentaje de realización de las mismas:

    -   Retrasadas: presenta el total de **tareas** que tiene la "Fecha de entrega" 
        menor que la fecha/hora actual;

    -   Por vencer: presenta el total de **tareas** que tenga la "Fecha de entrega" 
        que quedarán retrasadas en 24h a partir de la fecha/hora actual;

    -   En el plazo: presenta el total de **tareas** con la "Fecha de entrega" mayor que
        24h a partir de la fecha/hora actual;

    -   Total: presenta el total de **tareas** de aquella Sprint;

    -   La barra de progresión tiene el siguiente cálculo:

        -   1º Se hace la suma del total de estimaciones de todas las **tareas** terminadas;

        -   2º Se hace la suma del total de estimaciones de todas las **tareas**;

        -   3º Progreso es el porcentaje calculado con el total de estimaciones de las 
            **tareas** completadas sobre el total de estimaciones de todas las tareas.

!!! info "INFORMACIÓN"

    El cálculo del progreso depende totalmente de las estimaciones informadas en las tareas.
    
    
!!! warning "ATENCIÓN"    

    Para mover un **sprint** cambiando su ordenación, hacer clic y arrastrarla a la posición 
    de prioridad deseada.


### Crear listas

1.  Dentro de cada Sprint se ofrecen listas por defecto del sistema: "To do, In progress y Finished";

2.  Para crear nueva lista, hacer clic en “+Lista”, nombrar y “Guardar”.

    ![pantalla lista](images/figure-2-simple.png)
    
    Figura 2 - Pantalla de lista


    -   **1**: buscar tareas con filtros de miembros, tags y estado de la lista 
        (completada y no completada)

    -   **2**: crear nueva lista

    -   **3**: actualizar la pantalla

    -   **4**: abreviatura del nombre del miembro agregado. Al hacer clic se puede borrar 
        y definir si el miembro será administrador o no

    -   **6**: definir fecha, hora y estimación de horas para la entrega

    -   **7**: ver el historial de acciones

    -   **8**: archivar lista de tareas

### Crear tareas

   ![pantalla tarea](images/figure-3-simple.png)
    
   Figura 3 - Pantalla tarea


   -   **1**: crear nueva tarea

   -   **2**: definir en qué etapa la tarea se encuentra

   -   **3**: mover la lista físicamente dentro del cuadro

!!! warning "ATENCIÓN"

    Para mover una **tarea** de una lista a otra, hacer clic y arrastrar para la 
    lista deseada.

### Completar tarjeta Simple

La tarjeta Simple contiene campos y botones para describir una tarea/acción con
planificación y control de fechas, horarios, checklist y diversos otros
dispositivos de control y gestión.

1.  Cada tarjeta tiene dispositivos de control e información:

     ![pantalla tarjeta](images/figure-4-simple.png)
    
      Figura 4 - Pantalla de tarjeta


    -   **1**: agregar o eliminar miembros en la tarea

    -   **2**: agregar listas de acciones que serán vistas en la pestaña Checklist

    -   **3**: agregar comentarios

    -   **4**: cada miembro puede contabilizar horas relativas a su tiempo empleado en 
        la tarea, además de detallar la acción tomada

    -   **5**: agregar tags para identificar visualmente la tarjeta de tarea

    -   **6**: haga clic para notificarse acerca de cualquier modificación en esta tarea. La
        comunicación será a través del botón de notificaciones del CITSmart

    -   **7**: indicar la finalización de la tarea

    -   **8**: Mover la tarea a otro Sprint:

        -   Sprint del *mismo* Workspace: las tags se mantienen, pero los miembros son quitados
            de la tarea

        -   Sprint de *otro* Workspace: las tags y miembros son quitados de la tarea

    -   **9**: archivar la tarjeta - Una vez archivado, en esta versión, la tarjeta no podrá 
        ser reutilizado.

1.  Describir la tarea en el campo "Descripción";

2.  Definir la fecha y hora de entrega en el campo "Fecha de entrega";

3.  Estimar la cantidad de horas que se utilizarán en la tarea;

4.  En el campo "Horas contabilizadas", el sistema contabilizará automáticamente el total;

5.  Las pestañas disponibles presentan:

    -   **Checklist**: al agregar un checklists se creará un elemento en esta pestaña. Para nombrar, 
    pcolocar el ratón en el campo "Agregar elemento ...", hacer clic en el botón de agregar "+" 
    para agregar nuevo elemento. Para indicar la finalización de un elemento dentro de un checklist, 
    seleccione el checkbox;

    -   **Comentarios**: lista los comentarios hechos;
    
          -  Editar comentario;
          
          -  Eliminar comentario. Si opta por no participar, el comentario no se guardará en la 
             pestaña "Historial".

    -   **Adjuntos**: ofrece campo para agregar datos adjuntos;

    -   **Horas lanzadas**: relaciona las horas lanzadas de cada miembro participante de la
        tarea;

    -   **Historial**: presenta todas las acciones hechas en la tarjeta, con fecha y hora.


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/watch?v=ZpBJQymV9wU)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/13/2019 – Anna Martins
