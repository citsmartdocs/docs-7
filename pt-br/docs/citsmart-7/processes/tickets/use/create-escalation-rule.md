title:  Criar regra de escalonamento 
Description: Esta funcionalidade disponibiliza ações diversas, tais como, incluir, alterar e excluir a regra de escalonamento.
# Criar regra de escalonamento

Esta funcionalidade permite criar regras de escalonamento a fim de fornecer uma perspectiva de impacto à empresa ao gerir os atendimentos dos tickets (e suas eventuais requisições e incidentes) dentro de um tempo hábil pré-estabelecido. Ao criar regras para a notificação do responsável quando o ticket está em nível crítico de ruptura de seu SLA é possível evitar esta através de ações preventivas, escalonar este atendimento a outros grupos executores e respeitar assim seu tempo de atendimento.
Esta funcionalidade disponibiliza ações diversas, tais como, incluir, alterar e excluir a regra de escalonamento.

Antes de começar 
-----------------

Para criar as regras de escalonamento, é necessário configurar o parâmetro
190 o valor **S** e cadastrar previamente os contratos, colaboradores,
grupos, os portfólios de serviços e a ação automática do tipo escalonamento.

Já no arquivo **citsmart.cfg**, é preciso configurar a propriedade 
**START**\_**MONITORA**\_**INCIDENTES** informando o parâmetro TRUE (somente o
administrador do sistema operacional do servidor da aplicação realiza este
ajuste).

Procedimento
------------

1.  Acessar a funcionalidade Regras de Escalonamento navegando pelo menu
    principal Processos \> Gerência de Requisição e Incidente \> Regras de
    escalonamento;

2.  Clicar em "Novo";

3.  Informar os dados gerais da Regra de escalonamento (Título, situação, o
    solicitante, o grupo executor do atendimento, o portfólio e contrato a ser
    vinculado à regra e o impacto e urgência do atendimento do ticket);

4.  Informar os dados específicos da Regra de Escalonamento:

| **Campo** |                                                   **Objetivo**                                                   |
|:---------:|:----------------------------------------------------------------------------------------------------------------:|
|   Tempo   |                              Informar o prazo de escalonamento/notificação do ticket                             |
|  Formato  |        Informar se a regra se refere a minutos (tempo da regra) ou percentual (referente ao tempo do SLA)        |
|  Condição | Selecionar o marco do escalonamento/notificação (se esta ocorrerá antes ou depois da ruptura do prazo escolhido) |
|    Data   | Selecionar a data de referência da regra (a data de sua criação, a data da última ocorrência ou sua data limite) |
|    Ação   |                                  Vincular o tipo de ação automática a nova regra                                 |

Relacionado
-----------

[Criar portfólio](/pt-br/citsmart-7/processes/portfolio-and-catalog/use/create-the-portfolio.html)

[Cadastrar um grupo](/pt-br/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Cadastrar um colaborador](/pt-br/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Cadastrar um contrato](/pt-br/citsmart-7/additional-features/contract-management/use/register-contract.html)

[Cadastrar ação automática de escalonamento](/pt-br/citsmart-7/additional-features/automation-of-operation/configuration/register-escation-automatic-action.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROn4Xs6UdH84Ujzta2iJ6Ei)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/16/2019 - Larissa Lourenço
