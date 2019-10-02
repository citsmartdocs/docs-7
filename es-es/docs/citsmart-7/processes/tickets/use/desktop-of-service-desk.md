Title: El área de trabajo del service desk
Description:  Interfaz de gestión de tickets en CITSmart. Procesos de gestión de incidentes y  cumplimiento de solicitudes.

# El área de trabajo del service desk

El área de trabajo de la service desk es un espacio donde están disponibles los tickets que se han abierto para actividades vinculadas a su grupo, donde puede ver varias informaciones acerca del ticket.

## Antes de empezar

Para tener acceso a las funciones de la interfaz de gestión de tickets, es esencial tener permisos en grupo de trabajo y también acceso a catálogos de servicios. Además, debe tener al menos un ticket en la cola de atención.

## Procedimiento

1.	Acceder al menú Procesos > Gestión de ticket > Ticket.

## Interfaz

La pantalla principal de gestión de tickets es la interfaz del analista de atención con pedidos y/o incidentes que están en proceso o en espera de atención. Esta interfaz consta de: Funciones de búsqueda, Listado de Tickets y Menú Principal.

### Búsqueda

Es posible usar la barra de búsqueda para facilitar la búsqueda de un ticket específico - ingresando el número - o un conjunto de tickets con características similares - utilizando varios atributos - por ejemplo:

![Search Ticket Citsmart][1]

**1: Número del ticket**;

**2: Solicitante** del ticket (Quién solicitó atención);

**3: Tipo** – de servicio (Solicitud, Incidente o Procedimiento);

**4: Estado** del ticket (estados/expresiones registradas para un flujo);

**5: Contrato** el que el ticket está vinculado;

**6: Grupo ejecutor** actual (Conjunto de personas que pueden atender un servicio);

**7: Tarea actual** (Tarea de usuario en un flujo);

**8: Responsable** actual del ticket (Persona que asiste un servicio);

**9: Status SLA**: Expirado, Normal y otros;

**10: Ordenar por**: No Ticket, Fecha/hora creación, Actividad, Servicio, Responsable,
 Prioridad, Situación, fecha/tiempo límite y Fecha de la última actualización;

**11: Ver**: Todas los tickets o solo las que pueda rastrear o ejecutar;

**12: Unidad** – del Solicitante;

**13: Visualización**: Todos, Chat – apenas abiertas a través de este canal - y críticos – solo incidentes críticos;

**14: Opción para mostrar los tickets relacionados** – en la lista de atención;

Para aplicar una búsqueda basada en los filtros que establezca, use el botón "buscar". Después de realizar la búsqueda, el icono cambiará para identificar el estado de búsqueda, como:

 ![Search Ticket Citsmart][2] Icono sin búsqueda activa

 ![Search Ticket Citsmart][3] Icono con búsqueda activa

Se puede limpiar todos los filtros seleccionados y volver al formato predeterminado haciendo clic en "limpiar".

### Lista de Tickets

•	En la lista podemos ver los tickets disponibles en una cola de atención - según los permisos de grupo - donde encontramos las siguientes columnas:

 ![List Ticket Citsmart][4]

**1: Seleccionar Ticket(s)** – para delegar o suspender/reactivar;

**2: Número** del Ticket;

**3: Prioridad** – de atención (SLA);

**4: Servicio**;

**5: Solicitud** (Solicitud/Incidente);

**6: Solicitante**;

**7: Contrato**;

**8: Creado por** (Quién registró el ticket);

**9: Fecha creación** del ticket;

**10: Tarea** – del flujo;

**11: Grupo actual** – de la atención;

**12: Unidad**;

**13: Responsable** – por la atención;

**14: Estado de tareas** – en el flujo;

**15: SLA** – tiempo máximo de atención;

**16: Fecha limite** - para atención;

**17: Estado del SLA**;

Ubicados en la parte superior derecha, podemos ver una serie de iconos que representan, respectivamente:

![List Ticket Citsmart][5]

#### Paginación:

**1: Volver** a la primera página;

**2: Volver** una página;

**3: Número** identificador del ticket inicial de la página;

**4: Número** identificador del ticket final de la página;

**5: Número** total de tickets;

**6: Avanzar** una página;

**7: Avanzar** para la ultima página;

#### Delegación:

**8: Delegar** – ticket(s) para un grupo;

!!! Warning “ATENCIÓN”
    
    El botón "Actualización automática" vendrá por defecto no habilitado en los parámetros de CITSmart, para habilitarlo es necesario cambiar el parámetro 418 a la opción "SÍ". Esto hará que el botón esté disponible en la pantalla del ticket para actualizar automáticamente la página cada 25 segundos.

#### Actualización de la Página:

**9: Actualización automática** (25 y 25 segundos);

**10: Actualización de lista manual**;

#### Informes

**11: Informes**;

**12:	(Otras) opciones**;

**a: Suspensión/Reactivación** - de ticket;

**b: Cambiar columnas** (para personalización de la lista);

#### Opciones del Ticket:

Al hacer clic en un ticket en su cola de atención, se le mostrarán las acciones que puede tomar:

![Option Ticket Citsmart][6]

#### Opciones principales:

**1: Abrir**;

**2: Ver**;

**3: Descripción** ver la descripción del ticket sin abrirlo;

**4: Informes**;

**5: Ver Flujo** – del servicio;

**6: Más opciones** (presenta los elementos abajo);

#### Opciones secundarias:

**7: Delegar**;

**8: Suspender**;

**9: Cambiar SLA**;

**10: Reclasificar**;

**11: Crear Sub-ticket por copia**;

**12: Crear ticket relacionado**;

**13: Programar actividad**;

**14: Imprimir**;

!!! Warning "ATENCIÓN"
    
    Estas opciones se basan en los permisos otorgados a su perfil, por lo que es posible que no pueda utilizar todas las opciones anteriores.

### Menú Principal

#### Visión Global:

•	**Listado** – Presenta un listado con los tickets de su cola;

•	**Por asistente** – Gestión de ticket en una visión de Kanban;

•	**Por Situación de SLA** – Una vista sintética clasificada por estado de SLA;

•	**Por Estado del Flujo** – Estado actual (expresiones registradas para um flujo) de tickets asignados a un grupo;

#### Visión por Mapa:

•	**Mapa** – Permite ver tickets reservados para la atención en una unidad;

#### Visión por Búsqueda:

•	**Filtros** – Al seleccionar un filtro (expresiones registradas para un flujo) se mostrarán los tickets de acuerdo con el elemento seleccionado;

#### Otras opciones

•	**Agenda**: Permite ver eventos relacionados con Tickets, Cambios, Problemas y Liberación;

•	**Resumen**: Un informe cuantitativo de tickets;

•	**Búsqueda Avanzada**: Permite buscar tickets más detalladas, así como la información generada en su atención;

•	**Auditoría**: Presenta todos los cambios que se producen en un ticket, ya sea automático o manual;

[1]:images/ticket-search-citsmart.png
[2]:images/ticket-search-inactive-citsmart.png
[3]:images/ticket-search-active-citsmart.png
[4]:images/ticket-list-citsmart.png
[5]:images/ticket-list-options-citsmart.png
[6]:images/ticket-list-options-details-citsmart.png
