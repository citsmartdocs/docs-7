title: Automatically create a ticket from the receiving of an email
Description: It allows to automatic create ticket when an email message is sent to a a certain address.

# Automatically create a ticket from the receiving of an email

This functionality allows to automatic create ticket when an email message is
sent to a a certain address. In this context, the solution constantly monitors
the presence of messages in the mailbox, and if some message has the status of
not read, this will be used to register a new ticket.

For example, an user should request a service by sending a message to
service\@company.com, after receiving the email, the functionality, after check
the existence of a message, automatically registers the ticket. It's important
to highlight that after the ticket registration, the email is marked as read.

## Before getting started

To create a ticket through the receiving of an e-mail, it is necessary to configure 
an e-mail account to previously allow the access via IMAP. In addition, it is necessary 
to configure the instance to use batch routines, since the email verification is a 
scheduled task.

## Procedure

**Step 1 - Creating ticket template**

1.  Access the functionality through the main menu System \> Automatic actions
    \> Incident/Request/Procedure Actions (see Register automatic
    actions of incident/request/procedure).

**Step 2 - Set up access to the email box**

1.  Create the email automatic action by accessing the main menu System \>
    Settings \> Automatic Action Setting Via Email. This register is used 
    to trigger the rading and register of requests (see Create automatic 
    action via email).

**Step 3 - Create verification routine (batch)**

1.  Create batch routine, by accessing the main menu System \> Batch Processing
    (see Batch Processing), of "Java Class" type with the following content:
    
```java
 br.com.centralit.citcorpore.quartz.job.JobConfiguracaoAberturaAutomaticaViaEmail
```    


!!! Abstract "NOTE"

    It's possible to read the title of the email sent, it stored in the field
    *subject* of the table reademaildatarequest.
    
In addition, if there is a need to retrieve other information contained in the email fields, 
as recipients marked as copy (CC) or hidden copy (BCC) use the Rhino script below:

```java
var importNames = JavaImporter(); importNames.importPackage(Packages.br.com.citframework.util); var print = java.lang.System.out; var readEmailDataDTO = serviceRequest.getReadEmailDataDTO(); if (readEmailDataDTO!=null){ print.println("Dados do E-mail de Origem: "); print.println("From: "); print.println(readEmailDataDTO.getMessageFrom()); print.println("To: "); print.println(readEmailDataDTO.getMessageTo()); print.println("CC (Carbon Copy): "); print.println(readEmailDataDTO.getMessageCC()); }
```

Related
-------

[Register automatic actions of incident/request/procedure](/en-us/citsmart-7/additional-features/automation-of-operation/configuration/register-automatic-actions-incident-request-procedure.html)

[Create automatic action via email](/en-us/citsmart-7/platform-administration/configuring-automatic-actions/email-create-automatic-action-via-email.html)

[Batch Processing](/en-us/citsmart-7/platform-administration/configuring-automatic-actions/batch-batch-processing.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RN9wA1DbVHEot2QD2gW8_jq)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/17/2019 – Anna Martins

[1]:/en-us/citsmart-7/processes/tickets/images/rotina-verificar-email.docx

[2]:/en-us/citsmart-7/processes/tickets/images/script-rhino-dados-email.rtf
