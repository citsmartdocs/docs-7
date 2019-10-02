title: Implementar reglas de seguridad de contraseña
Description: Configuración de contraseñas de uso del sistema, ofreciendo mayor nivel de seguridad con uso de diferentes caracteres.
# Implementar reglas de seguridad de contraseña

Esta funcionalidad retrata la configuración de contraseñas de uso del sistema,
ofreciendo mayor nivel de seguridad con el uso de diferentes caracteres.

!!! Abstract "ATENCIÓN"

     Esta política de seguridad no está disponible para los usuarios LDAP.
     

Reglas por defecto al habilitar la Política de Seguridad:

-   Tamaño mínimo de 8 caracteres;

-   Al menos una letra minúscula;

-   Al menos una letra mayúscula;

-   Al menos un número;

-   Por lo menos un carácter especial (símbolo);

-   La contraseña no puede ser igual a las últimas 3 contraseñas utilizadas;

-   La contraseña caduca en 3 meses.

Procedimiento
------------

1.  Acceder al menú principal Sistema \> Configuración \> Política de Seguridad;

2.  Habilitar la clave "Habilitar política de contraseña";

3.  En el campo **Complejidad de la contraseña** el administrador debe establecer el número mínimo
    de caracteres de la contraseña (valor mínimo de 8) y si la misma contendrá requisitos
    de: letras mayúsculas, minúsculas, números y símbolos;

4.  Establecer la cantidad de contraseñas anteriores en la que la nueva no puede ser igual, en el limitador **La nueva contraseña no puede ser igual que las anteriores**;

5.  Para nuevos usuarios, el cambio de contraseña se puede definir al hacer clic en la clave
    “Forzar el cambio de contraseña la primera vez que se inicie sesión”

6.  En el campo **Duración de la contraseña** definir el tiempo para caducar la contraseña;

7.  Para usuarios que ya están en operación, es posible forzar el cambio de contraseña de la nueva configuración, desde el siguiente inicio de sesión, haga clic en la clave “Forzar el cambio de contraseña la primera vez que se inicie sesión”;

8.  Hacer clic en "Guardar”.

!!! Abstract "NOTA"

    El sistema notifica al usuario 3 días antes de la expiración de la contraseña
    actual, haciendo esta alerta a través de mensajería en cuadro de texto que
    surgirá una vez al día al iniciar sesión en el sistema. Después de que la
    contraseña esté expirado, el usuario se envía automáticamente a la pantalla de
    perfil de usuario con panel de cambio de contraseña abierto (sólo podrá utilizar
    el sistema de nuevo si realiza el cambio de contraseña).
  

!!! Abstract "NOTA"

    Para cambiar la contraseña, el usuario puede redefinir la contraseña por dos caminos
    diferentes, ver [Registrar usuario][1] y [Editar información de la cuenta][2].


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/31/2019 - Anna Martins

[1]:/es-es/citsmart-7/initial-settings/access-settings/user/users.html
[2]:/es-es/citsmart-7/initial-settings/access-settings/user/user-data.html
