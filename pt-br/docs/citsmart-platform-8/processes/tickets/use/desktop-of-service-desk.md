Title: A área de trabalho da Central de Serviços
Description:  Interface de gerenciamento de tickets no CITSmart. Processos de gerenciamento de incidente e cumprimento de requisição.

# A área de trabalho da Central de Serviços

A área de trabalho da Central de Serviços é um espaço onde estão disponíveis os tickets que foram abertos nas atividades vinculadas ao seu grupo, nela é possível visualizar diversas informações sobre o ticket.

## Antes de começar

Para ter o acesso aos recursos da interface de gerenciamento de ticket é imprescindível possuir permissões em grupos de trabalho e, também, acesso à catálogos de serviços. Além disso, é necessário ter pelo menos um ticket na fila de atendimento.

## Procedimento

1.	Acessar a funcionalidade pelo menu Processos > Gerência de ticket > Ticket.

## Interface

A tela inicial da gerência de ticket é a interface do analista de atendimento com os pedidos e/ou incidentes registrados e que estão em processo ou aguardando por atendimento. Esta interface é composta por: Recursos de pesquisa, Listagem de Tickets e Menu Principal.

### Pesquisa

É possível utilizar a barra de pesquisa para facilitar a busca de um ticket específico – informando o número - ou um conjunto de tickets com características similares – utilizando diversos atributos - como por exemplo:

![Search Ticket Citsmart][1]

**1: Número do ticket**;

**2: Solicitante** do ticket (Quem pediu atendimento);

**3: Tipo** – de serviço (Requisição, Incidente ou Procedimento);

**4: Situação atual** do ticket (estados/expressões cadastradas para um fluxo);

**5: Contrato** a qual o ticket está vinculado;

**6: Grupo executor** atual (Conjunto de pessoas que podem atender um serviço);

**7: Tarefa atual** (Tarefa de usuário em um fluxo);

**8: Responsável** atual do ticket (Pessoa que atende um serviço);

**9: Situação** (do) SLA: Vencido, Normal etc;

**10: Ordenar por**: Data/hora criação, Atividade, Serviço, Responsável,
 Prioridade, Situação, Data hora limite e Data última atualização;

**11: Visualizar**: Todos os tickets ou apenas os que posso acompanhar ou executar;

**12: Unidade** – do Solicitante;

**13: Exibição**: Todos, Chat – apenas abertas por este canal - e críticos – apenas incidentes críticos;

**14: Opção para visualizar os tickets relacionados** – na lista de atendimento;

Para aplicar uma pesquisa com base nos filtros definidos, utilize o botão “pesquisar”. Após a pesquisa ser realizada ocorrerá a alteração do ícone para identificar o status da pesquisa, como por exemplo:

 ![Search Ticket Citsmart][2] Ícone sem pesquisa ativa

 ![Search Ticket Citsmart][3] Ícone com pesquisa ativa

É possível limpar todos os filtros selecionados e retornar ao formato padrão ao clicar em “limpar”.

### Lista de Tickets

•	Na lista podemos visualizar os tickets disponíveis em uma fila de atendimento – com base nas permissões de grupos – onde encontramos as seguintes colunas:

 ![List Ticket Citsmart][4]

**1: Selecionar Ticket(s)** – para delegar ou suspender/reativar;

**2: Número** do Ticket;

**3: Prioridade** – de atendimento (SLA);

**4: Serviço**;

**5: Solicitação** (Requisição/Incidente);

**6: Solicitante**;

**7: Contrato**;

**8: Criado por** (Quem registrou o ticket);

**9: Data da criação** do ticket;

**10: Tarefa** – do fluxo;

**11: Grupo atual** – do atendimento;

**12: Unidade**;

**13: Responsável** – pelo atendimento;

**14: Situação da tarefa** – no fluxo;

**15: SLA** – tempo máximo de atendimento;

**16: Data limite** - para atendimento;

**17: Status do SLA**;

Localizado no canto superior direito podemos visualizar uma serie de ícones que representam respectivamente:

![List Ticket Citsmart][5]

#### Paginação:

**1: Voltar** para a primeira página;

**2: Voltar** uma página;

**3: Número** identificador do ticket inicial da página;

**4: Número** identificador do ticket final da página;

**5: Número** total de tickets;

**6: Avançar** uma página;

**7: Avançar** para a última página;

#### Delegação:

**8: Delegar** – ticket(s) para um grupo;

!!! Warning “Atenção”
    O botão “Atualização automática” virá por padrão não habilitado nos parâmetros do CITSmart, para habilitá-lo é necessário mudar o parâmetro 418 para a opção “SIM”. Desse modo, o botão ficará disponível na tela de ticket para realizar a atualização automática da página a cada 25 segundos.

#### Atualização da Página:

**9: Atualização automática** (25 em 25 segundos);

**10: Atualização manual**;

#### Relatórios

**11: Relatórios**;

**12:	(Outras) opções**;

**a: Suspensão/Reativação** - de ticket;

**b: Alterar colunas** (para personalização da lista);

#### Opções do Ticket:

Ao clicar em um ticket em sua fila de atendimento, aparecerão as ações que podem ser realizadas por você:

![Option Ticket Citsmart][6]

#### Opções principais:

**1: Abrir**;

**2: Apenas visualizar**;

**3: Visualizar** a descrição sem abrir;

**4: Relatórios**;

**5: Visualizar o Fluxo** – do serviço;

**6: Mais opções** (mostra os itens abaixo);

#### Opções secundárias:

**7: Delegar**;

**8: Suspender**;

**9: Alterar o SLA**;

**10: Reclassificar**;

**11: Criar Sub-ticket**;

**12: Criar ticket relacionado**;

**13: Agendar atividade**;

**14: Imprimir**;

!!! Warning "Atenção"
    Essas opções são baseadas nas permissões dadas ao seu perfil, em razão disso, eventualmente não será possível utilizar todas as opções disponíveis acima.

### Menu Principal

#### Visão Global:

•	**Listagem** – Apresenta uma lista com os chamados da sua fila;

•	**Por atendente** – Gerenciamento de ticket em uma visão Kanban;

•	**Por Situação de SLA** – Uma visão sintética categorizada por status de SLA;

•	**Por Status do Fluxo** – Estado atual (expressões cadastradas para um fluxo) de tickets atribuídos a um grupo;

#### Visão por Mapa:

•	**Mapa** – Permite visualizar tickets registrados para o atendimento em uma unidade;

#### Visão por Pesquisa:

•	**Filtros** – Ao selecionar um filtro (expressões cadastradas para um fluxo) serão mostrados os tickets conforme o item selecionado;

#### Outras opções

•	**Agenda**: Permite visualizar eventos relacionados à Tickets, Mudança, Problema e Liberação;

•	**Resumo**: Um relatório quantitativo de tickets;

•	**Pesquisa Avançada**: Permite realizar buscas mais detalhadas de tickets bem como as informações geradas em seu atendimento;

•	**Auditoria**: Apresenta todas as alterações que ocorrem em um ticket sejam automáticas ou manuais;

[1]:images/ticket-search-citsmart.png
[2]:images/ticket-search-inactive-citsmart.png
[3]:images/ticket-search-active-citsmart.png
[4]:images/ticket-list-citsmart.png
[5]:images/ticket-list-options-citsmart.png
[6]:images/ticket-list-options-details-citsmart.png
