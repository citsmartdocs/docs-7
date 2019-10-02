title:  Configurar buzón de correo electrónico 
Description: Esta funcionalidad tiene por objetivo configurar el envío y la recepción de correo electrónico
# Configurar buzón de correo electrónico

Esta funcionalidad tiene por objetivo configurar el envío y la recepción de correo electrónico desde diferentes servidores, para atender contratos distintos, así que un mismo CITSmart podrá atender diferentes clientes y cada uno tendrá su propia caja de correo electrónico. En este caso, puede utilizar una cuenta de correo electrónico de envío/lectura (Ej.: email@empresa.com) en un contrato de la empresa XPTO y otra cuenta de correo electrónico perteneciente a un contrato de empresa distinta (Ej.: email@empresa2.com).

Procedimiento
-------------

1.  Acceder al menú principal Parametrización \> Buzón de Correo Electrónico;

2.  Hacer clic en "Nuevo";

3.  Elegir el tipo de buzón. Si optar el tipo "Entrada" (significa que el
    usuario va a parametrizar una ruta por donde los correos electrónicos que
    necesitan ser leídos llegarán), será abierto nuevos campos catastrales,
    tales como: servidor, puerto del servidor, usuario (dirección del correo
    electrónico), contraseña, provider y carpeta de la bandeja de entrada, por
    lo que es necesario completar los campos;

4.  Si optar por el tipo "Salida" (significa que el usuario va a parametrizar
    una ruta por donde los correos electrónicos que necesitan ser enviados desde
    el sistema saldrán), se abrirá nuevos campos catastrales, tales como:
    servidor, puerto de servidor, usuario, contraseña, remitente, definir si
    será necesario la autenticación de TSL/SSL (ambos son protocolos de
    seguridad) y la autenticación del usuario, por lo tanto, es necesario
    completar los campos;

5.  Hacer clic en "Guardar";

6.  Vincular buzón de correo electrónico al contrato. Para eso: acceder a la
    funcionalidad Procesos \> Gestión de Portafolio Y Catálogo \> Contrato,
    después vincula en el campo "Bandeja de Salida de Correo Electrónico" el
    buzónn de correo registrado previamente y hacer clic en "Guardar";

7.  Vincular el buzón de corro electrónico a un flujo. Para eso:

    -   Acceder a la funcionalidad Sistema \> Mantenimiento de Flujos, después,
        al registrar/editar un flujo, localizar en la pestaña "Diagrama"
        la figura llamada “Envio de Mesaje -E_mail” en el flujo, y hacer clic
        para editar;

    -   En la opción "Configuración de la bandeja de salida de correo
        electrónico", abierta al hacer clic en la pestaña" Mensaje ",
        seleccionar la opción "Específica" para utilizar el cuadro de correo
        electrónico configurado en el contrato;

    -   Concluir la parametrización del flujo incluido en los "Destinatarios"
        seleccionados;

    -   El uso de diferentes cajas de correo electrónico de salida puede ser
        percibido después de abrir una solicitud de servicio, que posee
        parametrizado el flujo que posee la caja de correo seleccionada.

    -   Hacer clic en "Guardar".

!!! Abstract "ATENCIÓN"

    Vincular el buzón de correo electrónico no es un paso obligatorio. Esta
    funcionalidad sólo será necesaria para registrar el flujo, si el usuario
    siente necesidad de dirigir el correo electrónico a un buzón de salida
    distinta de la predeterminada. El correo electrónico de salida
    predeterminado del sistema continuará funcionando, incluso si este parámetro
    no se realiza.
    
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Larissa Lourenço



