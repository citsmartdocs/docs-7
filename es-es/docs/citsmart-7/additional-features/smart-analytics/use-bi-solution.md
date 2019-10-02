title: Usar Smart Analytcs (BI) para generar informes
Description: Analizar datos en su instancia, donde es posible elaborar innumerables posibilidades de gráficos, paneles y tablas con informaciones de datos mensurables.
# Usar Smart Analytics (BI) para generar informes


Según la Wikipedia Business Inteligence “Se denomina inteligencia empresarial, inteligencia 
de negocios o BI (del inglés business intelligence), al conjunto de estrategias, aplicaciones, 
datos, productos, tecnologías y arquitectura técnicas, los cuales están enfocados a la 
administración y creación de conocimiento sobre el medio, a través del análisis de los datos existentes 
en una organización o empresa".

CITSmart Analytics es la solución de BI para el análisis de datos de CITSmart.
Con esta funcionalidad, es posible elaborar innumerables posibilidades de
gráficos, paneles y tablas con información de datos registrados en la instancia.

Antes de empezar
----------------

Tener la aplicación de BI instalada, configurada y comunicable con su instancia
CITSmart.

Procedimiento
------------

1.  Acceder al menú principal Informes
    \> Smart Analytics \> Smart Analytics;

2.  Seleccionar una opción en la pestaña **Cubes** (default: Change Requests, Releases,
    Tickets);

3.  En la pestaña **Measures** seleccionar un tipo de medida para usar en el informe,
    hacer clic y después se agregará en el campo **Measure** del tablero de instrumentos;


    !!! Abstract "NOTA"

        Es posible elaborar un nuevo tipo de medida, para ello haga clic en el botón "Add" y elaborar nueva fórmula.
        
    
1.  En la pestaña **Dimensions** se ofrecen opciones que servirán de base de
    datos del informe. Seleccione y arrastre una opción dentro de una de los
    cuadros de medidas y dimensiones en el dashboard: Columns, Rows y Filters;

2.  Ael lado derecho del dashboard puede configurar el informe en varios formatos 
    de tabla y gráfico;

3.  Para cambiar la posición de las unidades de medida en la tabla/gráfico, haga clic en 
    el botón de detalles disponible en cada cuadro de medidas del dashboard;

4.  Para exportar el informe, haga clic en "Export" y seleccione una opción de
    formato (PNG y PDF);

5.  Después de finalizar el informe, haga clic en "Save query".



### Unidades disponibles

|             Dimensión           |                                      Objetivo                                     |
|:-------------------------------:|:---------------------------------------------------------------------------------:|
|             Activity            |           Presenta las actividades que se crearon dentro de la instancia          |
|               Date              |         Ofrece día, mes, año, bimestre, trimestre, cuatrimestre y semestre        |
|          Executor group         |                   Código/ID del grupo, nombre del grupo ejecutor                  |
|           Group Solver          |                     Código/ID, nombre del grupo solucionador                      |
|             Locality            |                       Presenta la ubicación del solicitante                       |
|             Priority            |                         Presenta la prioridad del ticket                          |
|            Requester            |                         Presenta el nombre del solicitante                        |
|           Responsible           |                         Presenta el nombre del responsable                        |
|            SLA Status           |                             Presenta el estado del SLA                            |
|    Service Level   Agreement    |                           Presenta el código/ID y el SLA                          |
|              Source             |                         Presenta el origen de la atención                         |
|            Technical            |                           Presenta el nombre del técnico                          |
|          Ticket Status          |                   Presenta el código/ID y el estado del ticket                    |
|              Unity              |                 Presenta el código/ID y la unidad del solicitante                 |



Relacionado
-----------

[Configurar solución BI (Smart Analytics) vía Docker](/es-es/citsmart-7/additional-features/smart-analytics/install-bi-docker.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/28/2019 – Anna Martins
