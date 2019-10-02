title: Configurar relatório para visualizar dados de atendimento
Description: Tem a finalidade de demostrar como configurar Smart Reports para utilizar na gestão de atendimento (Ticket management).
# Configurar relatório para visualizar dados de atendimento

Este documento tem a finalidade de demostrar como configurar Smart Reports para
utilizar na gestão de atendimento (Ticket management).

Relatórios por Ticket/Atendimento
-------------------------------------

Este relatório tem por objetivo demostrar em um período de tempo, os tickets
atendidos e o tempo gasto em cada ticket, bem como auxiliar na identificação de
expiração de tempo.

### Procedimento

1.  Acessar a funcionalidade através do menu principal Relatórios \> Relatórios
    Smart \> Gerador de Relatórios Smart;

2.  Realizar o download do arquivo abaixo, chamado "TicketAtendimento";

3.  Clicar no botão "Importar" e selecionar o arquivo citado logo acima;

4.  Selecionar o relatório chamado "RelatorioPorTicketAtendimento" da listagem
    da funcionalidade e clicar no seu botão de "Editar";

5.  Escolher o módulo de título "N/A" e definir os grupos que terão permissão de
    visualizar o relatório criado.

### Uso

1.  Acessar a funcionalidade através do menu principal Relatórios \> Relatórios
    Smart \> Relatórios Smart;

2.  Clicar no botão "Incidentes/Requisições" e selecionar o item
    "RelatórioPorTicketAtendimento";

3.  Definir os filtros com período desejado (com as datas de início e
    encerramento dos tickets);

4.  Será apresentado uma listagem com os dados: Solicitação
    de serviço, tipo, serviço, atividade, status, solicitante, data e hora da
    solicitação, data hora limite, SLA , tempo de atendimento (é a soma dos
    imputs das horas registradas nas ocorrências do ticket), data e hora do
    encerramento (se houver) além de um relatório sintético referente ao
    contrato escolhido;

    -   É possível clicar no número da solicitação de serviço para apresentar
        maiores detalhes sobre o técnico e as horas gastas pelo mesmo para
        atender o ticket.

5.  É possível também visualizar estes Relatórios no dashboard, se assim o
    configurar ao personalizar o mesmo Smart Decisions.

!!! Abstract "ATENÇÃO"

    Existe na aba "Relacionados" no canto superior esquerdo da tela, um
    conhecimento instruindo sobre a criação personalizada de dashboards.

Relatório por Técnico e Tempo Gasto
---------------------------------------

Este relatório tem por objetivo identificar o tempo de ociosidade por cada
técnico, uma vez que apresenta a soma da quantidade de ticket que cada técnico
executou e a soma dos tempos executados por cada técnico.

### Procedimento

1.  Acessar a funcionalidade através do menu principal Relatórios \> Relatórios
    Smart \> Gerador de Relatórios Smart;

2.  Realizar o download do arquivo abaixo, chamado "TecnicoTempo";

3.  Clicar no botão "Importar" e selecionar o arquivo citado logo acima. Clicar,
    então, no botão "Editar" e renomear o relatório com o título "Ticket - Tempo
    gasto por técnico";

4.  Selecionar o relatório chamado renomeado e clicar no seu botão de "Editar";

5.  Escolher o módulo de título "N/A" e definir os grupos que terão permissão de
    visualizar o relatório criado.

### Uso

1.  Acessar a funcionalidade através do menu principal Relatórios \> Relatórios
    Smart \> Relatórios Smart;

2.  Clicar no botão "Incidentes/Requisições" e selecionar o item "Ticket - Tempo
    gasto por técnico";

3.  Será apresentado uma listagem com os dados dos seguintes dados: Técnico,
    ticket e tempo gasto;

4.  é possível também visualizar estes Relatórios no dashboard, se assim o
    configurar ao personalizar o mesmo Smart Decisions.

!!! Abstract "ATENÇÃO"

    Existe na aba "Relacionados" no canto superior esquerdo da tela, um
    conhecimento instruindo sobre a criação personalizada de dashboards.



Relacionado
-------

[Personalizar o painel gerencial (Smart Decision)](/pt-br/citsmart-7/additional-features/reports/create/dashboard-customize-management-panel-smart-decision.html)

Anexo
------
[Download-Técnico tempo][1]

[Download-Ticket atendimento][2]



!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 – Anna Martins


[1]:/pt-br/citsmart-7/additional-features/reports/create/smart-reports/configuration/images/tecnico-tempo.citreport

[2]:/pt-br/citsmart-7/additional-features/reports/create/smart-reports/configuration/images/ticket-atendimento.citreport
