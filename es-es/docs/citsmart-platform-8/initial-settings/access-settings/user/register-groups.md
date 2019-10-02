title: Crear grupo
Description: Permite el registro de grupos y el vínculo con usuarios, perfil, contratos y correos electrónicos para notificación.

# Crear grupo

Un grupo es un conjunto de uno o más empleados que tienen los mismos objetivos
relacionados con sus funciones.

Los dos usos más comunes para los grupos creados son:

1.  Gestión de seguridad/confidencialidad de accesos a varios tipos de registros
    (por ejemplo, carpetas de la base de conocimiento, portafolios de servicios,
    etc).

2.  Programación de notificación automática basada en alguna situación/evento
    específico;

Esta funcionalidad permite el registro de grupos y el vínculo con usuarios,
perfil, contratos y correos electrónicos para notificación.

Esta funcionalidad ofrece diversas acciones, como, incluir, cambiar y borrar un
grupo.

## Antes de empezar

Para registrar un grupo, es necesario registrar previamente el perfil de acceso
y empleado.

## Procedimiento

1.  Acceder a la funcionalidad por el menú principal Acceso y Permisos \> Grupo;

2.  Hacer clic en "Nuevo";

3.  Completar los campos disponibles;

    - **Informaciones básicas**

    |Campo|Descripción|
    |-|-|
    |Nombre *	|[Nombre del Grupo]|
    |Sigla *	|[NG]|
    |ID Grupo|[01] - Creado automáticamente|
    |Líder|[Nombre del Líder] - Se utiliza para identificar al gestor del grupo|
    |Perfil de Acceso *	|[Perfil] - Perfil de acceso heredado|
    |Grupo de Service Desk|[Sí/No] - Si el grupo hace atención (= SÍ), de lo contrario, el grupo no aparecerá en la lista de grupos para la dirección/delegación de tickets|
    |Solicitante del Chat|[Sí/No] - Si los miembros del grupo pueden abrir tickets a través del chat|
    |Comité Asesor del Cambio|[Sí/No] - Si el grupo es parte de un Comité (Gestión de Cambios)|
    |Suspensión/Reactivación |Parámetro para permitir la suspensión/reactivación de tickets independientemente de los permisos del workflow (reactivar/suspender)|
    |Notificaciones de e-mail obligatorias (Abierto, En progreso y Cerrado)|Si está habilitado, hace que el envío de correo electrónico, proveniente de las diversas acciones de los flujos, sea obligatorio (no configurable por el asistente). Cuando se deja deshabilitado, el asistente puede configurar las opciones de envío de correo electrónico.|
    |Descripción |Detalles para ayudar a identificar el grupo.|

    - **Contratos:** Acuerdos a los que el grupo tendrá acceso (para registrar un servicio, realizar una atención, entre otros).

    - **Permisos en los flujos de trabajo**

    |Acción```*```| Descripción|
	  |-|-|
	  |Crear|Permiso para registrar ticket/actividad|
	  |Ejecutar|Permiso para ejecutar ticket/actividad|
    |Delegar|Permiso para delegar ticket/actividad|
	  |Suspender|Permiso para suspender ticket/actividad|
    |Reactivar|Permiso para reactivar ticket/actividad|
    |Cambiar SLA|Permiso para cambiar el SLA del ticket/actividad|
	  |Reabrir|Permiso para reabrir ticket/actividad|
    |Cancelar|Permiso para cancelar ticket/actividad|
    |Reclasificar|Permiso para reclasificar ticket/actividad|

    ```*```Seleccionar solo los permisos específicos para el contexto de acción.

    - **Colaboradores (usuarios del sistema):** miembros del grupo.
    - **E-mail:** Direcciones de correo electrónico que recibirán notificaciones procedentes de un workflow. Esta opción es muy útil cuando es necesario que una persona esté "informada" de las interacciones del grupo sin participar en el grupo..

4.  Definir las configuraciones necesarias;
5.  Hacer clic en "Guardar".


!!! Abstract "REGLA"

    La exclusión de grupo depende de que no exista portafolios, colaboradores
    y contratos vinculados.
    

Relacionado
-----------

[Registrar colaborador](/es-es/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Crear perfil de acceso](/es-es/citsmart-7/initial-settings/access-settings/profile/create-profile-access.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Anna Martins
