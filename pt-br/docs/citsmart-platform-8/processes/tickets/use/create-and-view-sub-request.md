title:  Criar e visualizar sub-ticket
Description: É possível criar sub-ticket através da solicitação original e visualiza-la após de criada. 
# Criar e visualizar sub-ticket

A funcionalidade permite cadastrar um ticket com atividades relacionadas ao ticket original.

Antes de começar
----------------

É necessário o cadastro prévio do colaborador, contrato e unidade. Também é
preciso vincular o grupo ao contrato, a unidade ao contrato e o contrato ao
serviço.

Cadastrar o portfólio com os serviços e as atividades de requisição e incidente.
Definir o tempo de atendimento das atividades de requisição e incidente.

Vincular as atividades de requisição e incidente ao contrato do serviço.
Configurar o parâmetro 385 com o valor 'S'.

Procedimento
------------

1.  Acessar a funcionalidade Gerenciamento de Ticket navegando pelo menu
    principal Processos \> Gerência de Ticket \> Ticket;

2.  Clicar sobre o ticket desejado e selecionar a alternativa "Criar sub-ticket" no menu opções;

3.  Preencher os campos necessários e clicar no botão "Gravar". O sub-ticket será direcionado para o grupo executor definido
    no registro do vínculo da atividade, o mesmo será direcionado para o grupo executor definido no parâmetro 9;

4.  Lembre-se que o sistema enviará e-mails de notificação a respeito de
    criação, escalonamento, captura, encerramento e demais alterações dos
    tickets relacionados para o grupo executor do ticket principal.
    
5.  Para pesquisar os sub-tickets, será necessário marcar o filtro "Exibir relacionadas" na área de 
    pesquisa na tela principal da funcionalidade.

        
!!! Abstract "ATENÇÃO"

    O sub-ticket tem um fluxo próprio, portanto, não é encerrado juntamente
    com o fechamento do ticket de origem. Deverá, assim sendo, ser executado e encerrado de
    forma autônoma.  
    
!!! Abstract "ATENÇÃO"

    O sub-ticket poderá ser reaberto a qualquer momento, independemente do status da solicitação pai (se está reaberta ou fechada).  
    
Relacionado
-----------

[Criar um ticket](/pt-br/citsmart-7/processes/tickets/use/create-ticket.html)

[Cadastrar um grupo](/pt-br/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Cadastrar um colaborador](/pt-br/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Cadastrar uma unidade](/pt-br/citsmart-7/platform-administration/region-and-language/register-unit.html)

[Configurar permissão de acesso do gerenciamento de requisições/incidentes](/pt-br/citsmart-7/processes/tickets/configuration/access-ticket-management.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROn4Xs6UdH84Ujzta2iJ6Ei)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/16/2019 - Larissa Lourenço


