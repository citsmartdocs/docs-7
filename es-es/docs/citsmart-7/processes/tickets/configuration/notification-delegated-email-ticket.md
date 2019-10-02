title: Notificar por correo electrónico de ticket delegado
Description: Permite implementar la forma de envío de correo electrónico de un ticket delegado, así que los tickets delegados tendrán un modelo de correo electrónico propio que se enviará al técnico.
# Notificar por correo electrónico de ticket delegado

Este documento permite implementar la forma de envío de correo electrónico de un
ticket delegado, así que los tickets delegados tendrán un modelo de correo
electrónico propio que se enviará al técnico

Antes de empezar
--------------------

Un modelo de correo electrónico deberá haber sido registrado previamente y que
las claves a ser usadas en su cuerpo de texto deberán ser las siguientes:

```html
${IDSOLICITACAOSERVICO}

${SERVICO}

${SOLICITANTE}

${DESCRICAO}
```

Procedimiento
-----------------

1.  Acceder al menú principal Procesos \> Gestión de Portafolio y Catálogo \>
    Portafolio;

2.  Elegir el portafolio y hacer clic en "Avanzar";

3.  Elegir el servicio y hacer clic en "Avanzar";

4.  Hacer clic en la pestaña *Contratos*;

5.  Seleccione el contrato y haga clic en "Avanzar";

6.  Hacer clic en la pestaña *Solicitudes* y haga clic en "Editar";

7.  Elegir la actividad;

8.  En el campo **Modelo de correo electrónico delegación** elegir por el modelo
    de correo electrónico registrado previamente;

9.  Hacer clic en "Guardar";

10.  En la pantalla parametrización, activar los parámetros 438 (informar plantilla
    de correo electrónico de delegación) y el 439 (opción "SÍ");
    
11.  En la pantalla de registro de grupo, en el campo "Colaboradores", seleccionar
    el checkbox "Email" de las personas que van recibir el correo de ese grupo.
    

Lo que hacer después
------------

Acceder el ticket que quieras y haga la delegación.


Relacionado
-------

[Delegar ticket](/es-es/citsmart-7/processes/tickets/use/delegate-ticket.html)

[Configurar modelo de e-mail](/es-es/citsmart-7/platform-administration/email-settings/email-templates-configure-email-template.html)

[Registrar grupo](/es-es/citsmart-7/initial-settings/access-settings/user/register-groups.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROl8PJLi-kszYhGzr17uvz-)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 – Anna Martins
