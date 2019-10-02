title: Cadastrar gerente Zabbix
Description: Registrar e manter os gerentes responsáveis pelo monitoramento dos itens de configuração cujo status será consultado no Zabbix.
# Cadastrar gerente Zabbix

O Zabbix é uma ferramenta para monitorar redes, servidores e serviços,
projetados para monitorar disponibilidade, experiência do usuário e qualidade de
serviços.

O objetivo desta funcionalidade é registrar e manter os gerentes responsáveis
pelo monitoramento dos itens de configuração cujo status será consultado no
Zabbix. Ele permite ao usuário associar os elementos de configuração aos seus
respectivos disparadores e às ações que devem ser tomadas na ocorrência de
eventos.

Esta funcionalidade disponibiliza ações diversas, tais como, incluir, alterar e
excluir um gerente Zabbix.

Antes de começar
--------------------

Para cadastrar o gerente Zabbix é necessário cadastrar previamente a conexão do
CITSmart Event Monitor, o horário, a categoria de ocorrência, a ação automática
e a conexão do CITSmart Inventory.

Procedimento
----------------

1.  Acessar a funcionalidade através da navegação no menu principal Processos \>
    Gerência de Evento \> Monitor Zabbix \> Gerente Zabbix;

2.  Preencher os campos disponibilizados em cada área;

3.  Na área Item de configuração pai é possível cadastrar o IC no CITSmart com
    os dados do Host selecionado. Clicar no botão "Criar IC". Vale lembrar que
    esse registro só poderá ser realizado caso não haja um IC com a mesma
    identificação do Host:

    -   Informe os dados do item de configuração filho;

    -   Conduzir uma relação entre o serviço Host e o item de configuração filho.
        Cada serviço host deve estar relacionado ao seu respectivo item de
        configuração filho.

1.  Clicar no botão "Gravar".


Relacionado
----------

[Cadastrar categoria de ocorrência](/pt-br/citsmart-7/processes/event/configuration/register-occurence-category.html)

[Cadastrar Conexão Event Monitor](/pt-br/citsmart-7/processes/event/configuration/register-event-monitor-connection.html)

[Cadastrar horário](/pt-br/citsmart-7/processes/event/configuration/register-time.html)

[Configurar conexão Inventory](/pt-br/citsmart-7/processes/event/configuration/set-inventory-connection.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/15/2019 – Anna Martins
