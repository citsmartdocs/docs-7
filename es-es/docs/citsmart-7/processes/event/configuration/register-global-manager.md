title: Registrar gerente Global
Description: Crear reglas para monitorear varios tipos de eventos.
# Registrar gerente Global

Esta funcionalidad tiene como objetivo crear reglas para monitorear varios tipos
de eventos.

Cada gerente de eventos global contiene una EPL para *information* (información),
*Warning* (advertencia) y/o *Exception* (excepción). EPL es un lenguaje de
correlación de eventos utilizado por Esper (Espertech). En la inicialización del
CITSmart Event Monitor, estos EPL se importan al engine del Esper, de modo que
un nuevo evento correlacionado se creará cada vez que se cumpla la condición
definida en la EPL. Ejemplo de una EPL que hace correlación entre los eventos de
CITSmart Inventory y Nagios: \@Description ('Para cualquier evento de Nagios que
se produzca después de un evento cualquiera de Inventory, en los últimos 10
minutos) select \* from pattern [every
a=EventoCheckInventory-\>b=EventoServicoNagios where timer:within(10minutes)].

Esta funcionalidad ofrece diversas acciones, como, incluir, cambiar y borrar un
gerente Global.

Antes de empezar
--------------------

Para registrar el gerente Global, es necesario registrar previamente la conexión
del CITSmart Event Monitor, el horario, categoría de ocurrencia, acción
automática y la conexión del CITSmart Inventory.

Procedimiento
-----------------

1.  Acceder al menú principal Procesos \> Gestión de Evento \> Gerente Global;

2.  Completar los campos disponibles en cada area:

    -  Informe los datos de la **Acción de Information**:

        -  Seleccionar la acción que se disparará cuando haya una ocurrencia de
           evento del tipo *information*, el grado de urgencia e impacto. Las reglas
           para esta acción se definen utilizando el Lenguaje de Procesamiento de
           Eventos - EPL. Haga clic en el botón *Validar EPL de Information* para
           validar la EPL informada.  

    -   Informe los datos de la **Acción de Warning**:  

        -  Seleccionar la acción que se disparará cuando haya una ocurrencia de
           evento del tipo *warning*, el grado de urgencia e impacto. Las reglas para
           esta acción se definen utilizando el Lenguaje de Procesamiento de
           Eventos - EPL. Haga clic en el botón *Validar EPL de Warning* para
           validar la EPL informada.   

    -   Informe los datos da la **Acción de Exception**:

        -  Seleccionar la acción que se disparará cuando haya una ocurrencia de
           evento del tipo *exception*, el grado de urgencia e impacto. Las reglas
           para esta acción se definen utilizando el Lenguaje de Procesamiento de
           Eventos - EPL. Haga clic en el botón *Validar EPL de Exception* para
           validar la EPL informada.   

3.  Hacer clic en "Guardar".


Relacionado
-----------

[Registrar categoría de ocurrencia](/es-es/citsmart-7/processes/event/configuration/register-occurence-category.html)

[Registrar Conexión Event Monitor](/es-es/citsmart-7/processes/event/configuration/register-event-monitor-connection.html)

[Registrar horario](/es-es/citsmart-7/processes/event/configuration/register-time.html)

[Configurar Conexión Inventory](/es-es/citsmart-7/processes/event/configuration/set-inventory-connection.html)

[Registrar acción automatica](/es-es/citsmart-7/additional-features/automation-of-operation/configuration/register-automatic-action.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/24/2019 – Anna Martins
 
