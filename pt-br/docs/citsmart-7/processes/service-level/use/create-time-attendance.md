title: Criar tempo de atendimento
Description: Disponibiliza ações diversas, tais como, incluir, alterar e excluir o tempo de atendimento do tipo Global (aplica-se a todos os serviços), Cliente (aplica-se aos serviços de um contrato) e Incidente/Requisição/Procedimento (aplica-se a um serviço específico).
# Criar tempo de atendimento

Esta funcionalidade disponibiliza ações diversas, tais como, incluir, alterar e
excluir o tempo de atendimento do tipo *Global* (aplica-se a todos os serviços),
*Cliente* (aplica-se aos serviços de um contrato)
e *Incidente/Requisição/Procedimento* (aplica-se a um serviço específico).

Antes de começar
--------------------

Para cadastrar o tempo de atendimento é necessário registrar previamente o
portfólio de serviços.

Procedimento
----------------

1.  Acessar a funcionalidade através da navegação no menu principal Processos \>
    Gerência de Nível de Serviço \> Tempo de Atendimento;

2.  Definir o tipo de tempo de atendimento e clicar na guia correspondente;

3.  Preencher os campos disponibilizados no quadro **Dados Básicos**;

    !!! Warning "IMPORTANTE"
    
        Indique no atributo "Mudança de Impacto/Urgência" se será permitido a mudança de Impacto e/ou Urgência.
        
    !!! Warning "ATENÇÃO" 
   
        Se o tempo de atendimento não permitir a alteração de impacto e urgência, o sistema substitui automaticamente o que for                 enviado via WebService para o impacto, urgência, prioridade e tempo de atendimento definidos neste cadastro.

4.  No quadro **Tempos de Atendimento por Prioridade** definir o tempo de
    atendimento dos serviços, levando em consideração a prioridade. A prioridade
    é usada para identificar os tempos requeridos para que ações adequadas sejam
    tomadas. A prioridade vai de 1 a 5, sendo que o 1 é a prioridade mais alta e
    5 é a mais baixa. Selecione a prioridade para definição do tempo:

    -   **Captura**: defina o tempo de captura da solicitação do serviço, conforme a
        prioridade selecionada;

    -   **Resolução**: defina o tempo de resolução do serviço, conforme a prioridade
        selecionada.

5.  Antes de preencher os campos do quadro **Automação** ela deve estar
    adequadamente parametrizada, para isso se faz necessário executar os passos
    contidos no conhecimento Criar Regra de Escalonamento, com exceção do
    parâmetro 190 que deverá estar igual a ‘N’ neste contexto;

6.  Após os N minutos (informado no tempo de ação) e caso não tenha realizado
    nenhuma ação na solicitação do serviço vinculado a este tempo de
    atendimento, o sistema atribuirá a prioridade e escalará o grupo para
    execução da solicitação do serviço;

7.  No quadro de **Incidente/Requisição/Procedimento**, selecione os serviços
    para aplicar as configurações, levando em consideração o tipo de tempo de
    atendimento selecionado;

8.  Clicar em "Gravar".


Relacionado
-------

[Cadastrar um serviço](/pt-br/citsmart-7/processes/portfolio-and-catalog/use/register-a-service.html)

[Configurar atributos de serviço](/pt-br/citsmart-7/processes/portfolio-and-catalog/use/configure-services-attributes.html)

[Criar portfólio](/pt-br/citsmart-7/processes/portfolio-and-catalog/use/create-the-portfolio.html)

[Configurar parametrização - ticket](/pt-br/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)

[Criar regra de escalonamento](/pt-br/citsmart-7/processes/tickets/use/create-escalation-rule.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROiBpoLlvJGu-Lsyzs6OYm-)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/16/2019 - Anna Martins
