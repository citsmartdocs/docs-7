title: Criar um fluxo de trabalho
Description: É possível criar fluxos de trabalho que melhor se adequam a realidade do usuário

# Criar um fluxo de trabalho

 É possível criar fluxos de trabalho que melhor se adequam a realidade do usuário, personalizando os cenários de cada organização.

Procedimento
------------

1.  Acessar o menu principal Workflow > Desenho de fluxo;

2.  Clicar no botão “Novo";

3.  Na aba “Dados do Fluxo” é necessário preencher os dados obrigatórios: nomear
    o fluxo (seu identificador interno, deve ser informado sem espaço, acentos e
    caracteres especiais); o processo a que está vinculado (o fluxo estará
    visível apenas para o processo a que está vinculado) e a opção para permitir
    a reabertura de um serviço independentemente das configurações de grupo.
    Também é possível visualizar qual versão o fluxo se encontra.

4.  Na aba “Diagrama” é apresentada a ferramenta para desenhar o fluxo inserindo os
    elementos que representam o cenário pretendido. Para tanto, basta clicar no
    elemento e arrastá-lo para a área de desenho. Ao fazer isso, será exibida
    uma tela para definir as propriedades. Devemos levar em consideração que sempre
    um fluxo começa com o elemento "Evento Início" e termina com o elemento "Evento Fim".

    !!! Abstract "IMPORTANTE"
    
        Os caminhos condicionais de um fluxo devem ser definidos na Conexão (Fluxo de Sequência). 
        Para acessar essas opções clicar uma vez na conexão, clicar no ícone de propriedades. É possível identificar a conexão (ex. aprovado) e indicar uma Condição, Ação ou Estado. [Ver Construir Expressões][2].
	

5.  As propriedades de um elemento podem ser definidas ao clicar duas
    vezes no elemento e em seguida no ícone apresentado ao lado do mesmo (ícone de propriedades).
    Defina os dados desta propriedade ao informar os dados necessários em cada uma das
    abas da tela de propriedade. Aqui também é liberado vincular um conhecimento
    ao fluxo na aba “Base de conhecimento” e implementar funcionalidades no
    fluxo sobre a atividade ao clicar na aba “Interface”;

    !!! Abstract "ATENÇÃO"

        A aba “Interface” possibilita escolher qual o modo de interação (formulário
        padrão, questionário ou formulário neuro) que será aplicado ao serviço.
        Porém, caso não ocorra a vinculação de nenhum template de
        solicitação de serviço nesta aba, o sistema subentenderá e aplicará as
        configurações de um formulário padrão, habilitado a vinculação de item de
        configuração, mudança, problema e solicitação relacionado ao ticket na tela
        de gerenciamento de tickets.  
        Podemos citar também outra regra referente a esta aba: as normativas aqui
        configuradas terão prioridade em relação às marcações do template de
        solicitação de serviço, pois esta é um complemento do fluxo.  

6.  Além disso, a funcionalidade admite importar fluxos ao clicar no botão
    “Importar”. Poderá importar no formato “JSON” ou “XML”.

7.  Após definir o fluxo, clicar no botão “Gravar” para efetuar a operação.

Relacionado
------------

[Cadastrar template de ticket](/pt-br/citsmart-7/platform-administration/questionnaires/ticket-template.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/21/2019 – Larissa Lourenço

[2]:/pt-br/citsmart-7/workflow/configuration/expressions-creator.html
