title: Crear ticket automático desde el recebimiento del correo electrónico
Description: Permite la creación automática de un ticket cuando se envía un mensaje de correo electrónico a una dirección determinada.

# Crear ticket automático desde el recebimiento del correo electrónico

Esta funcionalidad permite la creación automática de un ticket cuando se envía
un mensaje de correo electrónico a una dirección determinada. En este contexto,
la solución monitorea constantemente la presencia de mensajes en el buzón de
correo, y si algún mensaje tiene el estado no leído, éste se utilizará para
registrar un nuevo ticket.

Por ejemplo, un usuario podría solicitar cierto servicio enviando un mensaje a
servico\@empresa.com, después de recibir el correo electrónico, la
funcionalidad, luego que comprobar que existe un mensaje, registra un ticket
automáticamente. Es importante destacar que después del registro del ticket, el
correo electrónico es marcado como leído.

## Antes de empezar

Para crear un ticket a través del recibimiento del correo electrónico, es
necesario configurar previamente una cuenta de correo electrónico para permitir
el acceso a través del IMAP. Además, es necesario configurar la instancia para 
el uso de rutinas batch, ya que la comprobación de correo electrónico es una 
tarea programada.

Procedimiento
-----------------

**Paso 1 - Crear plantilla de ticket**

1.  Acceder al menú principal Sistema \> Acciones Automaticas \> Acciones de
    Incidentes/Requerimientos/Procedimientos (ver Registrar acciones
    automaticas de incidentes/requerimientos/precedimientos).

**Paso 2 - Configurar acceso a la bandeja del correo electrónico**

1.  Crear acción automatica de correo electrónico al acceder al menú principal
    Sistema \> Configuración \> Configuración de la acción automatica a través
    de correo electrónico Este registro se utiliza para disparar la lectura y 
    el registro de solicitudes (ver Crear acción automatica de correo electrónico).

**Paso 3 - Crear rutina de verificación (batch)** 

1.  Crear Rutina Batch al acceder al menú principal Sistema \> Procesamiento
    Batch (ver Procesamiento Batch), del tipo "Clase Java" con el siguiente
    contenido:
    
```java
 br.com.centralit.citcorpore.quartz.job.JobConfiguracaoAberturaAutomaticaViaEmail
```    


!!! Abstract "NOTA"

    Se puede leer el título del correo electrónico enviado, está guardado en el campo 
    *subject* de la tabla reademaildatarequest.

Además, si hay necesidad de recuperar otra información en los campos de correo electrónico, 
como destinatarios marcados como copia (CC) o copia oculta (BCC), utilice el script Rhino abajo:

```java
var importNames = JavaImporter(); importNames.importPackage(Packages.br.com.citframework.util); var print = java.lang.System.out; var readEmailDataDTO = serviceRequest.getReadEmailDataDTO(); if (readEmailDataDTO!=null){ print.println("Dados do E-mail de Origem: "); print.println("From: "); print.println(readEmailDataDTO.getMessageFrom()); print.println("To: "); print.println(readEmailDataDTO.getMessageTo()); print.println("CC (Carbon Copy): "); print.println(readEmailDataDTO.getMessageCC()); }
```

Relacionado
-------

[Registrar acciones automaticas de incidentes/solicitudes/procedimientos](/es-es/citsmart-7/additional-features/automation-of-operation/configuration/register-automatic-actions-incident-request-procedure.html)

[Crear acción automatica via correo eletronico](/es-es/citsmart-7/platform-administration/configuring-automatic-actions/email-create-automatic-action-via-email.html)

[Procesamiento Batch](/es-es/citsmart-7/platform-administration/configuring-automatic-actions/batch-batch-processing.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROl8PJLi-kszYhGzr17uvz-)'


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 – Anna Martins
    
[1]:/es-es/citsmart-7/processes/tickets/images/rotina-verificar-email.docx
  
[2]:/es-es/citsmart-7/processes/tickets/images/script-rhino-email.rtf
