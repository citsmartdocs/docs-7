title: Configurar parametrización – móvil
Description: La parametrización de "Mobile" tiene la finalidad de configuración,
# Configurar parametrización – móvil

La parametrización de "Mobile" tiene la finalidad de configuración, personalización para adecuación de escenario en lo que se refiere al uso de las aplicaciones móviles (por ejemplo, el CITSmart GO).

Procedimiento
-------------

1.  Acceder al menú principal Parametrización \> Móvil;

2.  Definir los valores de los parámetros (atributos);

3.  Hacer clic en "Guardar";

4.  La lista siguiente representa los parámetros del "Mobile" y la finalidad de
    cada uno de ellos:


| **#** |                                                         **Nombre**                                                         | **Valores posibles** |                                                                                                                                               **Finalidad**                                                                                                                                              | **Orientaciones Complementarias** |
|:-----:|:--------------------------------------------------------------------------------------------------------------------------:|:--------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------:|
|  255  |                            Rayo de Acción/Visualización del asistente en Mobile - (Default: 30)                            |                      |                                                                     Definir el radio de acción de un asistente, utilizado en el APP móvil. Definir el radio máximo de atención de solicitudes que estén con situación "No Dirigida".                                                                     |            No se aplica           |
|  256  |                   Intervalo (en minutos) de tiempo para reporte de posición del Asistente - (Default: 10)                  |                      |                                                                                             Definir el intervalo que la aplicación Móvil debe informar al servidor de la ubicación geográfica del asistente.                                                                                             |            No se aplica           |
|  257  |                         Tamaño de página para retorno en los servicios REST paginados (Default: 10)                        |                      |                                                                                                     Establecer la cantidad de registros devueltos en los servicios de lista consumidos por el Móvil.                                                                                                     |            No se aplica           |
|  258  |                                   Intervalo máximo de días para la consulta (Default: 30)                                  |                      |                                                                                 Definir la restricción del intervalo máximo de consulta en las pantallas, inicialmente utilizadas en la gestión de la fuerza de atención.                                                                                |            No se aplica           |
|  267  |                        Tamaño de página para retorno en los servicios REST V1 mobile (Default: 200)                        |                      |                                                                                                                    Establecer el tamaño de la página para volver a los servicios REST.                                                                                                                   |            No se aplica           |
|  272  |    Determina si se notificarán sólo solicitudes sin responsabilidad en Citsmart Mobile. Valores: "S" o "N" Default: "N"    |  S o N (Default: N)  | Establecer qué solicitudes se pueden notificar al usuario. En caso de que el valor del parámetro sea "S", se presentarán solamente las notificaciones de solicitudes sin responsable actual por la atención. Si el valor del parámetro es "N", se mostrarán las notificaciones de todas las solicitudes. |            No se aplica           |
|  284  |                ID de contrato estándar para la creación de nuevos incidentes/solicitudes en Citsmart Mobile                |                      |                                                                                           Indicar el número de identificación (ID) del contrato para realizar la apertura de solicitudes de servicio vía móvil.                                                                                          |            No se aplica           |
|  285  |           ID de servicio predeterminado para las solicitudes de servicios e incidentes creados en Citsmart Mobile          |                      |                                                                                      Indicar el número de identificación (ID) del servicio que será estándar para el registro de solicitudes de servicios vía móvil.                                                                                     |            No se aplica           |
|  286  |            ID de origen predeterminado para las solicitudes de servicio e incidentes creados en Citsmart Mobile            |                      |                                                                                        Indicar el número de identificación (ID) del origen predeterminado para la apertura de la solicitud de servicio vía móvil.                                                                                        |            No se aplica           |
|  350  |                                      Habilita el envío de notificaciones para móviles                                      |  S o N (Default: N)  |                                                                                                     Permite controlar si las notificaciones del sistema se envían a dispositivos móviles (generales).                                                                                                    |            No se aplica           |
|  352  |                     Habilita el envío de notificaciones para móviles durante la creación de solicitudes                    |  S o N (Default: N)  |                                                                                                     Permite controlar si las notificaciones del sistema se envían a dispositivos móviles (generales).                                                                                                    |            No se aplica           |
|  353  | Habilita el envío de notificaciones para móviles durante la actualización de solicitudes informando atendimientos cercanos |  S o N (Default: N)  |                                                                                                     Permite controlar si las notificaciones del sistema se envían a dispositivos móviles (generales).                                                                                                    |            No se aplica           |

Tabla 1 - Lista de parámetros

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Larissa Lourenço
