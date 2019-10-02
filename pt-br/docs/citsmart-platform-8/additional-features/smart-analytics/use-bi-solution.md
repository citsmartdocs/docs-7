title: Usar o Smart Analytcs (BI) para gerar relatórios
Description: Analisar dados em sua instância onde é possível elaborar inúmeras possibilidades de gráficos, painéis e tabelas com informações de dados mensuráveis.
# Usar o Smart Analytics (BI) para gerar relatórios


Segundo o site Wikipedia Business Inteligence “refere-se ao processo de coleta,
organização, análise, compartilhamento e monitoramento de informações que
oferecem suporte a gestão de negócios. É um conjunto de técnicas e ferramentas
para auxiliar na transformação de dados brutos em informações significativas e
úteis a fim de analisar o negócio”.

O CITSmart Analytics é a solução de BI para a análise de dados do CITSmart. Com esta funcionalidade é possível elaborar inúmeras possibilidades de gráficos, painéis e tabelas com informações de dados registrados na instância.

Antes de começar
----------------

Ter a aplicação de BI instalada, configurada e comunicável com sua instância
CITSmart.

Procedimento
------------

1.  Acessar a funcionalidade através do menu principal Processos \> Relatórios
    \> Smart Analytics \> Smart Analytics;

2.  Selecionar uma opção na guia **Cubes** (default: Change Requests, Releases,
    Tickets);

3.  Na guia **Measures** selecionar um tipo de medida para usar no relatório, ao
    clicar a mesma já será adicionada no campo **Measure** do dashboard;


    !!! Abstract "NOTA"

        É possível elaborar um novo tipo de medida, para isso clicar no botão “Add” e elaborar nova fórmula.
        
    
1.  Na guia **Dimensions** são disponibilizadas opções que servirão como base de
    dados do relatório. Selecionar e arrastar uma opção para dentro de uma das
    caixas de medidas e dimensões no dashboard: Columns, Rows e Filters;

2.  Ao lado direito do dashboard é possível configurar o relatório em diversos
    formatos de tabela e de gráfico;

3.  Para mudar a posição das unidades de medida na tabela/gráfico, clicar no
    botão de detalhes disponível em cada caixa de medidas do dashboard;

4.  Para exportar o relatório clicar no botão “Export” e selecionar uma opção de
    formato (PNG e PDF);

5.  Após finalizar o relatório clicar no botão “Save query”.



### Unidades disponíveis

|             Dimensão            |                                      Objetivo                                     |
|:-------------------------------:|:---------------------------------------------------------------------------------:|
|             Activity            |            Mostra as atividades que   foram criadas dentro da instância           |
|               Date              |    Disponibiliza dia,   mês, ano, bimestre, trimestre, quadrimestre e semestre    |
|          Executor group         |                    Código/ID   do grupo, nome do grupo executor                   |
|           Group Solver          |                      Código/ID, nome do grupo   solucionador                      |
|             Locality            |                        Mostra a localidade do   solicitante                       |
|             Priority            |                          Mostra a prioridade do   ticket                          |
|            Requester            |                            Mostra nome do   solicitante                           |
|           Responsible           |                            Mostra nome do   responsável                           |
|            SLA Status           |                               Mostra o status do SLA                              |
|    Service Level   Agreement    |                              Mostra código/ID e o SLA                             |
|              Source             |                          Mostra   a origem do atendimento                         |
|            Technical            |                               Mostra nome do técnico                              |
|          Ticket Status          |                     Mostra o código/ID e o   status do ticket                     |
|              Unity              |                   Mostra   o código/ID e unidade do solicitante                   |



Relacionado
-----------

[Configurar solução BI (Smart Analytics) via Docker](/pt-br/citsmart-7/additional-features/smart-analytics/install-bi-docker.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/28/2019 – Anna Martins
