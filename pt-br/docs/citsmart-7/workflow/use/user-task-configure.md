title: Configurar atividade de usuário no fluxo
Description: Este documento tem por objetivo configurar a atividade dentro de fluxo chamada tarefa de usuário. 
# Configurar atividade de usuário no fluxo 

Ao desenhar um fluxo é possível inserir diversos elementos, dentre eles a Atividade de usuário. Este documento tem por objetivo orientar quanto a configuração deste elemento no fluxo de trabalho.

Antes de começar
---------------
Para utilizar o elemento "Atividade de Usuário" é necessário, no mínimo, ter um fluxo cadastrado na ferramenta contendo os elementos de eventos: "início" e "fim".


!!! Abstract "NOTA"

    Dentro da aba *Interface*, escolhendo o Tipo de Interação "Formulário Neuro": possuir 2 formulários de Neuro distintos e         configurados para que o formulário de criação seja mostrado junto ao formulário de acompanhamento. 
    É necessário também criar o Template de Ticket para cada um dos formulários.

Procedimento
------------

1.	Acessar o menu principal Workflow > Desenho de fluxo;
2.	Clicar no botão “Novo”;
3.	Clicar na aba Diagrama e em seguida na guia Atividade;
4.	Clicar no elemento Tarefa de Usuário e arrastá-lo até o painel de criação de fluxo;
5.	Serão abertas as seguintes abas de configuração do elemento:

**Identificação**

*	Nome: nome da tarefa de usuário;

*	Descrição: detalhar a tarefa de usuário;

*	Tipo de instância:

    *	Uma única instância: só pode ter uma única instância não executada da tarefa no fluxo;
    
    *	Mais de uma instância controlada pelo fluxo: pode ter várias instâncias não executadas da tarefa;
    
    *	Criar uma instância para cada usuário: na atribuição, se houver ponto e vírgula nos usuários, será criada uma tarefa para cada usuário;

*	Identificador: é uma sigla única pra tarefa serve pra codificar Rhino e pra formulários do neuro;

*	Contabiliza SLA: definir se “Sim” ou “Não” (o status “SLA Suspensa” aparecerá na interface de gestão de ticket);

*	Percentual de execução: campo informativo da quantidade que essa tarefa do fluxo tem em todo o fluxo;

*	É uma tarefa de aprovação?: definir se “Sim” ou “Não”;

**Atribuição**

*	Tipo de destinatário: selecionar se será para grupo ou usuário específico

*	Tipo atribuição: definir se a atribuição será de execução ou de acompanhamento

*	Grupo/Usuário: selecionar o grupo/usuário

*	Ou Expressão: buscar por expressão já cadastrada previamente

**Ações do usuário**

*	Selecione a ação do cadastro: buscar por ação já cadastrada previamente (ex. ação de aprovação, ou seja, uma expressão com essa finalidade);

**Ação de entrada**

*	Construir expressão: definir uma expressão diretamente
*	Selecione a ação do cadastro: buscar por ação já cadastrada previamente

**Ação de saída**

*	Construir expressão: definir uma expressão diretamente

*	Selecione a ação do cadastro: buscar por ação já cadastrada previamente

**Interface**

*	Tipo de interação: é o modo com que um Questionário ou um Formulário Neuro vai ser aplicado na interface de gestão de ticket em um determinado estado do fluxo. A configuração dos itens que estarão visíveis pode ser definida no portfólio ou configurado diretamente no elemento Atividade de Usuário (do fluxo):

    *	Definido no portfólio: é possível que um template de ticket (questionário ou formulário) apareça pontualmente em um estado     do fluxo, utilizando o que foi configurado no atributo de serviço “Atividade” (requisição/incidente) - campos: “Template         CRIAÇÃO” e “Template acompanhamento”. Esta opção é vantajosa quando se tem fluxos genéricos utilizados por vários serviços.

    *	Formulário padrão: default do sistema 

    *	Formulário Neuro: possui um identificador para chamar o fluxo disparado por este formulário

*	Template (Padrão/Neuro): permite a vinculação de template de ticket.

    !!! Abstract "ATENÇÃO"

        Caso não ocorra a vinculação de nenhum template de solicitação de serviço na aba interface, o sistema subentenderá e 
        aplicará as configurações de um formulário padrão, habilitando a vinculação de item de configuração, mudança, problema
        e solicitação relacionada ao ticket tela de gerenciamento de solicitação de serviço.
    
*	Permite direcionar para grupo: possibilita a ativação/desativação da opção "Direcionar para grupo" no cadastro de um ticket;

*	Permite alteração da situação: torna visível/invisível as opções de atendimento do ticket (Registrada/Em andamento; Resolvida e Cancelada);

*	Habilita notificação e-mail: torna visível/invisível as opções de notificação por e-mail;

*	Permite delegar atendimento: possibilita a ativação/desativação da opção "Delegar" para que esta esteja visível no menu opções do gerenciamento de um ticket;

*	Permite alterar dados da tela: possibilita a edição de questionários na tela de gerenciamento do ticket.

!!! Abstract "REGRA"    
    
    As normativas configuradas no fluxo terão prioridade em relação às marcações do template de solicitação de serviço,
    pois esta é um complemento do fluxo.
    
**Base de conhecimento**

   *  Vincular base de conhecimento: escolher o conhecimento que deseja
       vincular a tarefa de usuário.

!!! Abstract "ATENÇÃO"

    O objetivo principal desta vinculação de conhecimento é permitir que o
    atendente de uma requisição/incidente tenha facilmente acesso a ele. Assim
    que o fluxo chegue na atividade do fluxo vinculado a um conhecimento, o
    botão “Conhecimentos” é mostrado no canto superior direito da tela de
    Requisição/Incidente para dar acesso de leitura ao conteúdo, para tanto, tal
    conhecimento geralmente é escrito na forma de um passo a passo.
    
    
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/22/2019 – Anna Martins
