title: Registrar fórmula de la orden de servicio
Description: Registrar las fórmulas personalizadas para configurar "cómo" será el cálculo del valor del costo total de la actividad del servicio del contrato.
# Registrar fórmula de la orden de servicio

Esta funcionalidad tiene el objetivo de registrar las fórmulas personalizadas
para configurar "cómo" será el cálculo del valor del costo total de la actividad
del servicio del contrato.

Procedimiento
-----------------

1.  Acceder al menú principal Gestión Integrada \> Gestión de Contratos \>
    Fórmula OS;

2.  En la pestaña "**Registro de Fórmula**", es necesario completar los campos
    necesarios. Al informar las opciones de la fórmula, es necesario recordar el
    propósito de cada variable disponible para describir la fórmula:

    |     Variable    |     Descripción    |                                                                          Objetivo                                                                         |
    |:---------------:|:------------------:|:-------------------------------------------------------------------------------------------     --------------------------------------------------------------:|
    |      vValor     |        Valor       |                              Permite que el usuario informe un valor que se utilizará en el cálculo del valor de la actividad                             |
    |    vDiasUteis   |    Días hábiles    | Permite el retorno de la cantidad de días hábiles entre la fecha inicial y la fecha final de la orden de servicio en función del calendario del contrato. |
    |  vDíasCorridos  |    Días corridos   |                                              Cantidad de días entre la fecha inicial de la orden de servicio.                                             |
    | vNumeroUsuarios | Número de usuarios |                                               Permite devolver el número de usuarios activos en el Sistema.                                               |
    |   vComplejidad  |     Complejidad    |    Con base en la complejidad elegida por el usuario, el Sistema retornará su valor correspondiente informado en la pantalla de registro del contrato.    |
 


3.  Después de describir la fórmula, hacer clic en "Mostrar Fórmula". Este botón
    representa la validación de la fórmula y donde se presenta el proceso del
    cálculo, transformando el texto de la fórmula en una expresión matemática y
    devolviendo su resultado calculado, después de hacer clic en "Simular".
    Recordar que es posible utilizar las llaves "{}" para delimitar un texto que
    desee incluir en la fórmula, donde el mismo no influenciará el cálculo del
    valor de la actividad;

4.  Haga clic en "Guardar" para hacer la operación. Pero antes de guardar la
    fórmula, el sistema debe validar la sintaxis y sólo permitir la grabación si
    es correcta.


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROTLt6Tt7uegzqwpXHX5nA2)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/17/2019 – Anna Martins


