title: Crear tiempo de servicio
Description: Ofrece acciones diversas, como, incluir, cambiar y borrar el tiempo de respuesta del tipo Global (se aplica a todos los servicios), Cliente (se aplica a los servicios de un contrato) e Incidente/Requerimiento/Procedimiento (se aplica a un servicio específico).
# Crear tiempo de atención


Esta funcionalidad ofrece diversas funciones, como, incluir, cambiar y borrar 
el tiempo de respuesta del tipo *Global* (se aplica a todos los servicios), 
*Cliente* (se aplica a los servicios de un contrato) y *Incidente/Requerimiento/Procedimiento* 
(se aplica a un servicio específico).

Antes de empezar
--------------------

Para registrar el tiempo de servicio, es necesario registrar previamente el
portafolio de servicios.

Procedimiento
-----------------

1.  Acceder a la funcionalidad por el menú principal Procesos \> Gestión de
    Nivel de Servicio \> Tiempo de Servicio;

2.  Definir el tiempo de servicio y hacer clic en la pestaña correspondiente:

3.  Completar los campos disponibles en el cuadro **Datos Básicos**;

    !!! Abstract "IMPORTANTE"

        Indicar en el atributo "Cambio de Impacto/Urgencia" si se va permitir el cambio
        de Impacto y/o Urgencia.

    !!! Abstract "ATENCIÓN"
    
        Si el tiempo de atención no permite el cambio de impacto y la urgencia, el sistema 
        reemplaza automáticamente lo que se envía a través de WebService para el impacto, 
        la urgencia, la prioridad y el tiempo de respuesta definidos en este registro.

4.  En el cuadro **Tiempo de Atención por Prioridad**, definir el tiempo de
    atención de los servicios, teniendo en cuenta la prioridad. La prioridad se
    utiliza para identificar los tiempos requeridos para que las acciones
    adecuadas sean tomadas. La prioridad va de 1 a 5, siendo 1 la prioridad más
    alta y 5 la más baja. Seleccione la prioridad para la definición del tiempo:

    -  **Captura**: definir el tiempo de captura de la solicitud de servicio, o
        tempo de captura da solicitação do serviço, según la prioridad seleccionada;

    -  **Resolución**: definir el tiempo de solución del servicio, según la
        prioridad seleccionada.

5.  Antes de completar los campos del cuadro **Automatización**, debe estar
    adecuadamente parametrizada, para ello se hace necesario ejecutar los pasos
    contenidos en el conocimiento Crear regla de escalonamiento, con excepción
    del parámetro 190 que deberá ser igual a 'N' en este contexto;

6.  Después de N minutos (informado en el tiempo de acción), y si no ha
    realizado ninguna acción en la solicitud del servicio vinculado a este
    tiempo de atención, el sistema asignará la prioridad y escalará el grupo
    para ejecutar la solicitud del servicio;

7.  En el cuadro de **Incidente/Requerimiento/Procedimiento**, seleccione los
    servicios para aplicar la configuración, teniendo en cuenta el tipo de
    tiempo de respuesta seleccionado;

8.  Hacer clic en "Guardar".


Relacionado
-------

[Registrar servicio](/es-es/citsmart-7/processes/portfolio-and-catalog/use/register-a-service.html)

[Configurar atributos del servicio](/es-es/citsmart-7/processes/portfolio-and-catalog/use/configure-services-attributes.html)

[Crear portafolio](/es-es/citsmart-7/processes/portfolio-and-catalog/use/create-the-portfolio.html)

[Configurar parametrización - ticket](/es-es/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)

[Crear regla de escalonamiento](/es-es/citsmart-7/processes/tickets/use/create-escalation-rule.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RO_W3fA7hiLL0qbrsk6GyV9)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/24/2019 - Anna Martins
