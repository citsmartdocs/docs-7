title:  Registrara conexiones LDAP
Description: Permite registrar múltiples conexiones LDAP y definir las configuraciones para cada una de ellas.
# Registrara conexiones LDAP

El LDAP (Lightweight Directory Access Protocol - Protocolo Ligero/Simplificado de Acceso a Directorios) es un protocolo estándar que permite administrar directorios, es decir, acceder a bancos de información sobre los usuarios de una red a través de protocolos TCP/IP.
Esta funcionalidad permite registrar múltiples conexiones LDAP y definir las configuraciones para cada una de ellas.

![Autenticación CITSmart LDAP](images/cloud-arch-authentication.png)

Antes de empezar
----------------

Es necesario tener registrado el horario para la programación de la
sincronización automática.

Procedimiento
-------------

1.  Acceder al menú principal Acessar o menu principal Parametrización \>
    Configuración LDAP;

2.  Hacer clic en "Nuevo";

    !!! Abstract "REGLA"

        Todos los campos son igualmente relevantes para viabilizar la conexión           con el LDAP, mientras la prueba no es correcta, el procedimiento de
        configuración no puede ser considerado completado.

3.  Completar los campos disponibles;

    !!! Abstract "REGLA"

        Si no hay grupos LDAP, complete el campo "DN Group" sólo con un                 asterisco. Esto hará que el sistema compruebe todo el dominio.

4.  Es posible vincular nuevos grupos, para ello, haga clic en "Agregar" en el
    área Grupos LDAP;

    !!! Abstract "REGLA"

        Antes de solicitar la prueba, se DEBE hacer clic en "Guardar" para               guardar la configuración, de lo contrario, la prueba utilizará los datos         anteriores a los cambios hechos en la pantalla.
        Cuando hay una solicitud de autenticación en la pantalla de                     identificación del sistema (login y contraseña), se ejecuta un ciclo de         búsqueda de la conexión correcta sobre la base de esta configuración, es         decir, hay un intento de autenticación para cada dominio aquí registrado         (esto si hay más de uno).

5.  Es posible vincular mapas de campos, para ello, haga clic en "Agregar" en el
    área **Mapeo de campos**;

6.  Hacer clic en "Guardar".

!!! Abstract "REGLA"

    El sistema no permite eliminar un usuario que tiene origen en el LDAP.

### LDAP Seguro (LDAPS)

URL: ldaps://your-host.com:636

!!! success "Certificado digital"

    Exportar el certificado público del servidor LDAP y agregar en el               repositorio de certificados de CA de Java desde su instancia CITSmart.


Relacionado
-----------

[Registrar horario](/es-es/citsmart-7/processes/event/configuration/register-time.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 - Larissa Lourenço
