title: Configurar la aprobación de solicitud por correo electrónic
Description: Aprobar o rechazar la solicitud de un ticket a través del e-mail, sin la necesidad de que el administrador esté registrado.
# Configurar la aprobación de solicitud por correo electrónic


Esta funcionalidad tiene por objeto aprobar o rechazar la solicitud de un ticket
a través del e-mail, sin la necesidad de que el administrador esté registrado.

Antes de empezar
--------------------

Para hacer la configuración del e-mail en el ticket, es necesario registrar
previamente el usuario, grupo y configurar los parámetros 33 y 370 conforme
orientaciones de las reglas de parametrización referente al sistema. También es
necesario saber dibujar y tener registrado el flujo de aprobación de solicitud
vía e-mail. En este flujo, deberá existir la tarea "Aprobación" y el diseño para
envío de e-mail, registrar el modelo de e-mail con el modelo "Aguardando
Aprobación", y el servidor de correo electrónico deberá ser configurado con
todos los parámetros referentes a las reglas de parametrización de correo
electrónico.

!!! Abstract "ATENCIÓN"

    La aprobación de ticket vía correo electrónico será posible sólo con los 
    siguientes navegadores configurados por defecto: Mozilla Firefox, Google 
    Chrome y Microsoft Edge a partir de la versión 42.17134.1.0.

Procedimiento
-----------------

1.  Acceder a la funcionalidad en el menú principal Workflow \> Diseño de
    flujo;

2.  Seleccionar el flujo de apobación de solicitud y hacer clic en "Editar";

3.  Clic en la pestaña **Diagrama**;

4.  En el flujo de aprobación de solicitud, haga clic en el icono "Envío de Mensaje - e-mail" y después, en el pequeño cuadro gris cerca del conector configurado;

5.  Registrar, en la pestaña **Identificación**, el nombre y modelo de correo
    electrónico a utilizarse;

6.  Configurar, en la pestaña **Destinatarios**, los tipos de destinatarios
    (grupo/usuario) del correo electrónico que se va enviar (el sistema no hace
    búsqueda por destinatarios por "Expresión".

###Configurar la notificación de aprobación del correo electrónico

1.  Acceder a la funcionalidad en el menú Sistema \> Configuración \> Modelo
    de e-mail;

2.  Pegar el modelo de correo electrónico disponible en HTML adjunto en el campo
    Texto y comprobar las siguientes directrices:

    +   href="{TOKEN(serviceRequestIncident, \${IDSOLICITACAOSERVICO}, VIEW, 50)};

    +   serviceRequestIncident = Dirección de la interface : este campo no puede ser
        cambiado por el usuario;

    +   \${IDSOLICITACAOSERVICO} = Clave para incrementar el número de solicitud de
        servicio: este campo no puede ser cambiado por el usuario;

    +   VIEW - llama al comando para abrir la solicitud: este campo no puede ser
        cambiado por el usuario;

    +   MM (50) - Tiempo de expiración del token en minutos: este campo puede ser
        cambiado por el usuario;

3.  Haga clic en "Guardar".


Relacionado
-------

[Registrar grupo](/es-es/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Registrar usuario](/es-es/citsmart-7/initial-settings/access-settings/user/users.html)

[Flujo de trabajo](/es-es/citsmart-7/workflow/overview.html)

[Configurar parametrización - correo eletronico](/es-es/citsmart-7/platform-administration/parameters-list/configure-parametrization-email.html)

[Configurar parametrización -sistema](/es-es/citsmart-7/platform-administration/parameters-list/configure-parametrization-system.html)

Adjunto
----------
[Download - Aprobación][1]


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROl8PJLi-kszYhGzr17uvz-)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 – Anna Martins


[1]:/es-es/citsmart-7/processes/tickets/images/aprobacion.docx
