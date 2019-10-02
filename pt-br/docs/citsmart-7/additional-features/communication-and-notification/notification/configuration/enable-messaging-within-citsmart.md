title: Configurar a mensageria dentro do CITSmart
Description: Disponibiliza um canal de comunicação entre o solicitante (Smart Portal) e o técnico (área de solicitação de serviço/ticket) via mensagem (email).
# Configurar a mensageria dentro do CITSmart

O CITSmart disponibiliza um canal de comunicação entre o solicitante (Smart
Portal) e o técnico (área de solicitação de serviço/ticket) via mensagem
(email). Essa comunicação visa facilitar a resolução de um chamado. Este
conhecimento reúne informações pertinentes à configuração do serviço de
mensageria.


Antes de começar
--------------

É preciso realizar a configuração da conta de e-mail (SMTP) previamente (verificar item relacionado).

Procedimento
----------------

1.  Para que o serviço de mensageria esteja disponibilizado dentro do CITSmart é
    necessário setar o parâmetro 417 com o número do ID do modelo de e-mail que
    contenha algumas variáveis para poder ser enviado a mensageria;

2.  Abaixo estão listadas chaves para o envio de e-mail:

    -   \${IDSOLICITACAOSERVICO} - ID do ticket (chave pública);

    -   \${NOMECONTATO} - Nome do Contato;

    -   \${REGISTRADOPOR} - Registrado por;

    -   \${DATAHORA} - Data Hora;

    -   \${DEMANDA} - Tipo da atividade;

    -   \${SERVICO} - Atividade;
    
    -   \${SERVICORELACIONADO} - Serviço;
    
    -   \${PORTFOLIO} - Portfólio;
    
    -   \${CATEGORIA} - Categoria da ocorrência;
    
    -   \${TEMPOGASTODATA} - Tempo Gasto Data;
    
    -   \${TEMPOGASTOHORA} - Tempo Gasto Hora.


Relacionado
-------

[Configurar conta de e-mail](/pt-br/citsmart-7/platform-administration/email-settings/configuration.html)

[A área de trabalho da Central de Serviços](/pt-br/citsmart-7/processes/tickets/use/desktop-of-service-desk.html)

[Configurar parametrização - ticket](/pt-br/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)

[Configurar modelo de email](/pt-br/citsmart-7/platform-administration/email-settings/email-templates-configure-email-template.html)

[Gerenciar minhas solicitações pelo Smart Portal](/pt-br/citsmart-7/processes/portfolio-and-catalog/use/request-through-Smart-Portal.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/16/2019 - Anna Martins
