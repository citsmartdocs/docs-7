title: Cadastrar template de ticket
Description: habilitar algumas funcionalidades na tela de solicitação de serviço (ticket).
# Cadastrar template de ticket

Esta funcionalidade tem o objetivo de habilitar algumas funcionalidades na tela
de solicitação de serviço (ticket).

Esta funcionalidade disponibiliza ações diversas, tais como, incluir, alterar e
excluir template de ticket.

Antes de começar
--------------------

O template de ticket do tipo Questionário requer o registro de um questionário
previamente.

O template de ticket do tipo Neuro requer o registro prévio de um formulário do
tipo **Neuro** previamente.

Procedimento
----------------

1.  Acessar a funcionalidade de Template de Solicitação de Serviço através da
    navegação no menu principal Sistema \> Template de Ticket;

2.  Clicar no botão " Novo";

3.  O Tipo de Template selecionado irá definir os campos para preenchimento:

    -   **JSP**: esta funcionalidade permite personalizar a tela de serviços com
        referência, principalmente, na gerência de compras e viagens. Dentro do tipo
        JSP existem sub-tipos previamente cadastrados. A utilidade deste tipo de
        template só é observada nas versões anteriores à 7.2.3.9. Esta classe de
        template deverá ser manipulada por analista que possua conhecimento de
        programação JAVA

    -   **Questionário**: mesmo que desabilitada a opção de "Habilita editar
    questionário", essa edição será possível quando ocorrer o cadastro do
    ticket. Existem duas funções de aprovação que podem ser configuradas, na
    tela de template de solicitação de serviço ou na de manutenção de fluxo. Via
    de regra, para o sistema, somente as configurações realizadas na tela de
    fluxo terão validade. A função de aprovação existente na tela de template de
    solicitação de serviço só terá validade se vinculada ao cadastro de um
    formulário JSP nos modelos mais antigos do sistema. Os campos de habilitação
    apesar de selecionados por default, terão sua visualização não disponível no
    momento de criação de ticket , esta visualização ocorrerá com a efetivação
    do cadastro. No momento de cadastro do ticket que tenha um formulário do
    tipo padrão, estarão disponíveis no botão "Menu", localizado no canto superior
    esquerdo, apenas as funcionalidades: IC do Solicitante, Anexos, Agenda,
    Liberação, Projeto, Conhecimento e Leitura de e-mails. Todas as
    funcionalidades de habilitação que são apresentadas tanto na tela de
    template de solicitação de serviço quanto na de manutenção de fluxo, só
    terão validade as marcações configuradas na tela de fluxo, pois a primeira
    mencionada é um complemento da segunda. Se o template de solicitação de
    serviço estiver vinculado somente a atividades do portfólio o sistema vai
    subentender que o formulário é padrão, por isso ele não vai atender às
    normativas (habilitação ou não da funcionalidade) do template. Para a regra
    de reclassificação onde o template de serviço do tipo Questionário ou Neuro
    tiver que ser apresentado para a resposta do usuário, é preciso que o
    template ou formulário esteja vinculado ao template de solicitação de
    serviço concomitantemente com a tela de manutenção de fluxo e a atividade do
    portfólio.

    -   **Neuro**: ao selecionar esta opção, o campo de vinculação de formulário
    Neuro e página Neuro são disponibilizados. Também é possível eleger
    a versão do formulário ao clicar no botão "Versão específica do
    formulário". As regras do template do tipo *Questionário* são válidas para o
    template do tipo Neuro.


Relacionado
-----------

[Criar um fluxo do trabalho](/pt-br/citsmart-7/workflow/use/create-flow.html)

[Cadastrar questionário](/pt-br/citsmart-7/platform-administration/questionnaires/questionaires-management/register-questionnaire.html)



!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 – Anna Martins

