title: Reclassificar um ticket
Description: Após criar um ticket é possível reclassificar as informações de um ticket depois sua abertura.  
# Reclassificar um ticket
Após criar um ticket é possível reclassificar as informações de um ticket depois sua abertura. Essa ação desencadeia um e-mail para o solicitante informando sobre a alteração feita.
Não é permitido delegar ao ticket a um atendente se a situação dela for “Resolvida”.

Antes de começar
----------------

Para reclassificar um ticket o usuário tem que pertencer a um grupo executor, na
tela de grupo vincular o Fluxo a opção de "Alterar SLA", além de ter a permissão
para "criar" no fluxo da atividade destino, isso quando a reclassificação
incluir troca de atividade e se for um cenário de fluxos diferentes.

Procedimento
------------

1.  Acessar a funcionalidade pelo menu principal Processos \> Gerência de
    Requisição e Incidente \> Ticket;

2.  Selecionar ou procurar pelo ticket;

3.  Clicar sobre ele, selecionar o botão “Mais Opções” e escolher a opção
    "Reclassificar";

4.  Fazer as modificações.

!!! Abstract "ATENÇÃO"

    Ao reclassificar um ticket é necessário o preenchimento do campo
    **Justificativa da reclassificação** para que fique registrado para todas as
    pessoas envolvidas no processo, as atualizações quanto a mudanças
    relacionadas ao mesmo.


!!! Abstract "REGRA"

    Se a alteração for na descrição do ticket, será apresentado no e-mail de
    notificação (em destaque) a alteração feita na descrição. Lembrando que esse
    e-mail de notificação somente será enviado caso tenha habilitado o envio do
    mesmo no parâmetro "231 - Ativar envio de e-mail quando for editado um
    incidente (S ou N - Default: S)".  A reclassificação inclui uma delegação
    implícita para o Grupo ou Atendente destino, em versões anteriores, o
    usuário tinha que: reclassificar, capturar a atividade e delegar a outro
    grupo.


O que fazer a seguir
--------------------

Verificar na página de tickets relacionados se o mesmo teve a reclassificação.

Relacionado
-----------

[Cadastrar um grupo](/pt-br/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Criar um fluxo de trabalho](/pt-br/citsmart-7/workflow/use/create-flow.html)

[Configurar permissão de acesso do gerenciamento de requisições/incidentes](/pt-br/citsmart-7/processes/tickets/configuration/access-ticket-management.html)

[Configurar parametrização - ticket](/pt-br/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROn4Xs6UdH84Ujzta2iJ6Ei)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/17/2019 – Larissa Lourenço
