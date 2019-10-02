title: Criar um ticket automaticamente a partir do recebimento de um e-mail
Description: Permite a criação automática de um ticket quando uma mensagem de e-mail é enviada para um determinado endereço.

# Criar um ticket automaticamente a partir do recebimento de um e-mail

Esta funcionalidade permite a criação automática de um ticket quando uma
mensagem de e-mail é enviada para um determinado endereço. Neste contexto, a
solução monitora constantemente a presença de mensagens na caixa de e-mail, e
caso alguma mensagem tenha o status não lida, esta será utilizada para registro
de um novo ticket.

Por exemplo, um usuário poderia solicitar determinado serviço enviando uma
mensagem para servico\@empresa.com, após o recebimento do e-mail, a
funcionalidade, após checar que existe uma mensagem, registra um ticket
automaticamente. É importante destacar que após o registro do ticket, o e-mail é
marcado como lido.

## Antes de começar

Para criar um ticket através de um recebimento de e-mail é necessário configurar
uma conta de e-mail para permitir o acesso via IMAP previamente. Além disso, é 
necessário configurar a instância para utilização de rotinas batch, uma vez que a 
verificação de e-mail é uma tarefa agendada.

## Procedimento

**Passo 1 - Cria um modelo de ticket**

1.  Acessar a funcionalidade através da navegação do menu principal Sistema \>
    Ações automáticas \> Ações Incidentes/Requisições (ver
    Cadastrar Ação automática de Incidentes/Requisições/Procedimentos).

**Passo 2 - Configurar acceso a la bandeja de correo electrónico**

1.  Criar ação automática de e-mail, acessando o menu principal Sistema \>
    Configurações \> Configuração de Ação automática via e-mail. Este cadastro é usado 
    para disparar a leitura e o registro de solicitações (ver Criar ação automática de e-mail).

**Passo 3 - Criar rotina de verificação (batch)**

1.  Criar Rotina batch, acessando o menu principal Sistema \> Processamento
    Batch (ver Processamento Batch), do tipo "Classe Java" com o seguinte conteúdo:

```java
 br.com.centralit.citcorpore.quartz.job.JobConfiguracaoAberturaAutomaticaViaEmail
```


!!! info "NOTA"

    É possível ler o título do e-mail enviado, ele está guardado no campo *subject* da tabela reademaildatarequest.

Além disso, caso haja a necessidade de recuperar outras informações constantes nos campos do e-mail, como destinatários marcados como cópia (CC) ou cópia oculta (BCC) utilize o script Rhino abaixo:

```java
var importNames = JavaImporter(); importNames.importPackage(Packages.br.com.citframework.util); var print = java.lang.System.out; var readEmailDataDTO = serviceRequest.getReadEmailDataDTO(); if (readEmailDataDTO!=null){ print.println("Dados do E-mail de Origem: "); print.println("From: "); print.println(readEmailDataDTO.getMessageFrom()); print.println("To: "); print.println(readEmailDataDTO.getMessageTo()); print.println("CC (Carbon Copy): "); print.println(readEmailDataDTO.getMessageCC()); }
```

Relacionado
-------

[Cadastrar ação automática de incidentes/requisições/procedimentos](/pt-br/citsmart-7/additional-features/automation-of-operation/configuration/register-automatic-actions-incident-request-procedure.html)

[Criar ação automática via email](/pt-br/citsmart-7/platform-administration/configuring-automatic-actions/email-create-automatic-action-via-email.html)

[Processamento Batch](/pt-br/citsmart-7/platform-administration/configuring-automatic-actions/batch-batch-processing.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RN9wA1DbVHEot2QD2gW8_jq)'


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/16/2019 – Anna Martins

[1]:/pt-br/citsmart-7/processes/tickets/images/rotina-verificar-email.docx

[2]:/pt-br/citsmart-7/processes/tickets/images/script-rhino-dados-email.rtf
