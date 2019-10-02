title: Configurar servicio de cambio de contraseña
Description: El cambio de contraseña del usuario es una de las posibilidades permitidas por el sistema.  
# Configurar servicio de cambio de contraseña

El cambio de contraseña del usuario es una de las posibilidades permitidas por el sistema. Para configurar esta opción, es necesario seguir los procedimientos aquí descritos.

!!! Abstract "ATENCIÓN"

    Esta opción sólo está disponible para la autenticación de cuentas manuales.

Antes de empezar
----------------

Es necesario previamente tener un servicio de correo electrónico (SMTP) funcional, ya que el envío de la contraseña se realiza vía correo electrónico.

Procedimiento
------------

*1º Paso: Crear una plantilla de correo electrónico para cambiar la contraseña*

1.  Acceder al menú principal Sistema \> Configuración \> Modelo de e-mail;

2.  Crear la plantilla de correo electrónico para cambiar la contraseña;

    !!! Abstract "ATENCIÓN"

        Para que el usuario reciba la nueva información de acceso es necesario utilizar, en el mensaje de correo electrónico la         clave ‘${NOVASENHA}’ (ejemplo de clave referente a "Nueva contraseña"). Además, también se puede enviar el usuario de           login utilizando la clave ‘${LOGIN}’ (ejemplo de clave referente a “Login”).  

*2° Paso: Establecer la parametrización referente al servicio de cambio de contraseña*

1.  Acceder al menú principal Parametrización \> Parámetros CITSmart;

2.  Editar y guardar el parámetro 116 asignándole el valor numérico del ID generado para el modelo de correo electrónico recién creado.

Lo que hacer después
------------------

Para probar el servicio de cambio de contraseña, acceder a la página de login, hacer clic en la opción
"¿Olvidaste tu contraseña?", informar un login de usuario local y hacer clic en "Guardar".

## Relacionados

[Crear Plantilla de Correo Electrónico][1]

[Configurar Cuenta de Correo Electrónico][2]

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/21/2019 – Larissa Lourenço

[1]:/es-es/citsmart-7/platform-administration/email-settings/email-templates-configure-email-template.html
[2]:/es-es/citsmart-7/platform-administration/email-settings/configuration.html
