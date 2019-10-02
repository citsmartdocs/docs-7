title: Configurar parametrización – telefonía
Description: Acciones posibles a fin de configurar el uso de la telefonía en el CITSmart.
# Configurar parametrización – telefonía

La parametrización de la "Telefonía", permite definir si activa la integración del webservices con la telefonía, informar el número de identificación del servicio de solicitud, entre otras acciones posibles a fin de configurar el uso de la telefonía en el CITSmart.

Procedimiento
-------------

1.  Acceder al menú principal Parametrización \> Telefonía;

2.  Definir los valores de los parámetros (atributos);

3.  Hacer clic en "Guardar";

4.  La lista siguiente representa los parámetros de la "Telefonía" y la
    finalidad de cada uno de ellos:

| **#** |                                                                          **Nombre**                                                                          | **Valores posibles** |                                                                                            **Finalidad**                                                                                           |                                    **Orientaciones complementarias**                                   |
|:-----:|:------------------------------------------------------------------------------------------------------------------------------------------------------------:|:--------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------:|
|  281  |                                      Activar Servicio Web de integración con Telefonía - Valores: "S" o "N" Default: "N"                                     |  S o N (Default: N)  |                                                                Definir si activa la integración de los webservices con la telefonía.                                                               | Si no se establece el valor para el parámetro, el sistema automáticamente definirá el valor: "N" (No). |
|  282  | ¿La telefonía debe lanzar una solicitud hija, referente a la visualización de informaciones de una solicitud ya existente? - Valores: "S" o "N" Default: "N" |  S o N (Default: N)  |               Definir si activa el lanzamiento automático de una solicitud de servicio hija, de la que está siendo visualizada o ejecutada, por el webservice "visualizarSolicitud".               | Si no se establece el valor para el parámetro, el sistema automáticamente definirá el valor: "N" (No). |
|  283  |                                         ID del servicio de solicitud de información sobre una solicitud ya existente.                                        |         S o N        | Informar el número de identificación (ID) del servicio de solicitud, el cual se utilizará para lanzar la solicitud hija referente a la visualización de información de una solicitud ya existente. |                                              No se aplica                                              |
                                                                                        
Tabla 1 - Lista de parámetros

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Larissa Lourenço  
