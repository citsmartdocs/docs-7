title:  Configurar parametrización - orden de servicio 
Description: La parametrización de "Orden de Servicio" permite definir la fórmula de cálculo de la glosa de la orden
# Configurar parametrización - orden de servicio

La orden de servicio es un documento que proporcionará el permiso de ejecución relativo a algún servicio. La parametrización de "Orden de Servicio" permite definir la fórmula de cálculo de la glosa de la orden, habilitar firmas personalizadas en el informe de las Órdenes de Servico, dentro de otras acciones viables.

Procedimiento
-------------

1.  Acceder al menú principal Parametrización \> Orden de Servicio (OS);

2.  Definir los valores de los parámetros (atributos);

3.  Hacer clic en "Guardar";

4.  La lista siguiente representa los parámetros de la orden de servicio y la
    finalidad de cada uno de ellos:

| **#** |                                               **Nombre**                                              | **Valores posibles** |                                                                                                                                                                                                           **Finalidad**                                                                                                                                                                                                          |                                                             **Orientaciones complementarias**                                                             |
|:-----:|:-----------------------------------------------------------------------------------------------------:|:--------------------:|:--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------:|
|   51  |                                   FORMULA GLOSA OS - Código Estándar                                  |                      |                                                                                                                                            Definir la fórmula de Cálculo de la Glosa de la Orden de Servicio. De forma predeterminada, la fórmula ya está definida en la herramienta.                                                                                                                                            |                                                                        No se aplica                                                                       |
|  130  | Permitir Orden de lista de servicios con carácter retroactivo (por ejemplo, S o N - por default: 'N') |  S o N (Default: N)  |                                                                                                                                                                           Definir si se permitirá la lista de orden de servicio con fecha retroactiva.                                                                                                                                                                           |                            Si no se indica el valor del parámetro, se utilizará el valor predeterminado del sistema: "N" (No).                            |
|  229  |                    Reconfigurar fórmulas de actividades (Ej: S o N - Default: 'S')                    |  S o N (Default: S)  | Cambiar la estructura de la fórmula de las actividades ya registradas para la nueva estructura que es configurable en la pantalla de Fórmula OS. Al informar el valor predeterminado "S", el sistema ejecutará la rutina de reconfiguración de la fórmula de las actividades, en el momento en que JBoss se reinicie en una actualización del sistema CITSmart, y asignar "N" a este parámetro en el momento de su finalización. | Una vez informado el valor "S", la fórmula de las actividades del contrato, aún no configurada, quedará de acuerdo con la nueva estructura de Fórmula OS. |
|  243  |               Activar suscripciones personalizadas en el informe de órdenes de servicio               |                      |                                              Habilitar firmas para utilizar en la impresión de los informes de la Orden de Servicio. Cuando el parámetro está activado (valor = S), el sistema mostrará un campo en la pantalla de registro de Orden de Servicio y el usuario podrá elegir qué configuración de los cuadros de firmas se utilizará en la impresión de sus informes.                                              |                Cuando se habilita el parámetro, obliga al usuario a definir y configurar otro campo antes de grabar una orden de servicio.                |



Tabla 1 - Lista de parámetros

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Larissa Lourenço
