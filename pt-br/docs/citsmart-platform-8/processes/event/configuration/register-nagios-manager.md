title: Cadastrar gerente Nagios
Description: Cadastrar e manter os gerentes que serão responsáveis por monitorar os itens de configuração e ocorrência de eventos capturadas a partir do Nagios.
# Cadastrar gerente Nagios

Nagios é uma ferramenta de monitoramento de rede. Ele pode monitorar tanto hosts
quanto serviços, alertando quando ocorrerem problemas e também quando os
problemas são resolvidos. Os Hosts são os equipamentos e os Serviços são os
recursos oferecidos pelos equipamentos.

O objetivo desta funcionalidade é cadastrar e manter os gerentes que serão
responsáveis por monitorar os itens de configuração e ocorrência de eventos
capturadas a partir do Nagios. Permite ao usuário informar de quanto em quanto
tempo o Gerente será processado, quais os itens de configuração que ele irá
gerenciar e as ações a serem tomadas automaticamente.

Esta funcionalidade disponibiliza ações diversas, tais como, incluir, alterar e
excluir um gerente Nagios.

Antes de começar
--------------------

Para cadastrar o gerente Nagios é necessário cadastrar previamente a conexão do
CITSmart Event Monitor, o horário, a categoria de ocorrência, a ação automática
e a conexão do CITSmart Inventory.

Procedimento
----------------

1.  Acessar a funcionalidade através da navegação no menu principal Processos \>
    Gerência de Evento \> Monitor Nagios \> Gerente Nagios;

2.  Preencher os campos disponibilizados em cada área;

3.  Na área Item de configuração pai é possível cadastrar o IC no CITSmart com
    os dados do Host selecionado. Clicar no botão "Criar IC". Vale lembrar que
    esse registro só poderá ser realizado caso não haja um IC com a mesma
    identificação do Host:

    -   Informar os dados do item de configuração filho;

    -   Conduzir uma relação entre o serviço Host e o item de configuração filho.
        Cada serviço host deve estar relacionado ao seu respectivo item de
        configuração filho;

1.  Clicar no botão "Gravar".


Relacionado
-----------

[Cadastrar categoria de ocorrência](/pt-br/citsmart-7/processes/event/configuration/register-occurence-category.html)

[Cadastrar Conexão Event Monitor](/pt-br/citsmart-7/processes/event/configuration/register-event-monitor-connection.html)

[Cadastrar conexão Nagios/Zabbix](/pt-br/citsmart-7/processes/event/configuration/register-nagios-zabbix-connection.html)

[Cadastrar horário](/pt-br/citsmart-7/processes/event/configuration/register-time.html)

[Cadastrar ação automática](/pt-br/citsmart-7/additional-features/automation-of-operation/configuration/register-automatic-action.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/15/2019 – Anna Martins
