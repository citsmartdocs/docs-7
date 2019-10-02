title: Administrar os contratos
Description: A administração dos contratos é utilizada com o objetivo de gerenciar os contratos já cadastrados no sistema.  
# Administrar os contratos

A administração dos contratos é utilizada com o objetivo de gerenciar os contratos já cadastrados no sistema. Este processo permite verificar, adicionar e excluir serviços, além de dispor de vínculos para a criação de OS, de fatura e notificação.

Antes de começar
----------------

É necessário o cadastro prévio do grupo, dos contratos, dos serviços, do modelo
de e-mail. Também é imprescindível o cadastro do acordo de nível de serviço
(geral).

Para criar uma ordem de serviço, é necessário que o usuário tenha permissão para
abertura de OS e cadastrar o serviço do tipo "Ordem de Serviço",
vincular o serviço ao contrato, vincular o acordo de nível de serviço do tipo
"OS - Resultados Esperados" ao serviço. Do mesmo modo, é imperativo registrar as
atividades, com os seus respectivos valores, sendo um custo total ou calculado
por fórmula, do serviço do contrato. Todas estas ações serão explanadas ao longo
deste artigo.

Procedimento para vincular um serviço ao contrato
-------------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Serviços do Contrato" e em seguida no botão "Adicionar
    Serviço ao Contrato";

4.  Preencher os campos necessários. Para vincular um fluxo de serviço, clicar
    no ícone “+” do fluxo e selecionar o fluxo desejado e clicar em "Gravar".

    !!! Abstract "ATENÇÃO"

        Caso seja necessário fazer uso de mais de um fluxo, é importante informar
        qual é o principal.

5.  Após preencher os campos, clicar em "Gravar" para efetuar a operação.

Procedimento para vincular vários serviços ao contrato
------------------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Serviços do Contrato" e em seguida no botão "Adicionar
    VÁRIOS Serviços ao Contrato";

4.  Preencher os campos necessários. Para vincular um fluxo de serviço, clicar
    no ícone “+” do fluxo, selecionar o fluxo desejado e clicar em "Gravar".

    !!! Abstract "ATENÇÃO"

        Caso seja necessário fazer uso de mais de um fluxo, é importante informar
        qual é o principal.

5.  Após preencher os campos, clicar em "Gravar" para efetuar a operação.

Procedimento para verificar os serviços do contrato
---------------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Serão apresentados todos os serviços que estão vinculados ao contrato. Caso
    queira buscar um serviço específico, informar o nome dele no campo
    **Pesquisa Serviços Contrato** e clicar em "Pesquisar".

Procedimento para editar as informações do vínculo do serviço ao contrato
-------------------------------------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Serviços do Contrato", pesquisar o serviço desejado e em
    seguida no ícone “Editar o serviço” do serviço que deseja editar;

4.  Alterar os dados conforme a necessidade e clicar no botão "Gravar" para
    efetuar a operação.

Procedimento para vincular SLA específico ao serviço do contrato
----------------------------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Serviços do Contrato" e em seguida no ícone “Acordos de
    Nível de Serviço” do serviço desejado. Clicar no botão "Criar acordo
    específico" para este serviço que será apresentado;

4.  Preencher os campos necessários com as seguintes recomendações:

    -   Se informar o tipo de acordo como **Disponibilidade**, além dos campos
    gerais, será necessário informar o índice de disponibilidade, isto é,
    definir o percentual de disponibilidade do serviço;

    -   Se informar o tipo de acordo como **Falhas repetitivas**, além dos campos
    gerais, será necessário informar a quantidade de glosas e o percentual de
    desconto. Lembrar que é possível informar outros dados do acordo de serviço
    por falhas repetitivas, ao clicar no ícone “+”;

    -   Se informar o tipo de acordo como **OS -Resultados esperados**, além dos
    campos gerais, será necessário informar os dados de resultados esperados e
    os níveis de qualidade exigidos (resultados esperados, limites, glosa e
    limite glosa);

    -   Se informar o tipo de acordo como **Tempo (fases)**, além dos campos gerais,
    será necessário definir os prazos de SLA (acordo de nível de serviço),
    levando em consideração a prioridade.


    !!! Abstract "ATENÇÃO"

        Após os "N" minutos configurados e caso não tenha realizado nenhuma ação
        na solicitação do serviço, o sistema atribuirá Prioridade e escalará o Grupo
        que foram configurados para execução da solicitação do serviço.

    -   Se informar o tipo de acordo como **Informações diversas capturadas de
    outras fontes**, será necessário informar os dados de acordo de serviço (o
    valor limite, a unidade, a glosa e o limite glosa). Para copiar, editar ou
    excluir o acordo de nível de serviço cadastrado, seguir os passos:

        +  Para editar ou excluir um acordo de nível de serviço que foi adicionado ao
           serviço de contrato, basta clicar no ícone “Editar o serviço” ao lado do
           acordo;

        +  Para copiar um acordo de nível de serviço que foi adicionado ao serviço de
           contrato, basta clicar no ícone “Copiar Acordo para outro serviço” ao lado
           do acordo.

5.  Clicar no botão "Gravar" para efetuar a operação.

Procedimento para vincular SLA Global ao serviço do contrato
------------------------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo o contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Há duas formas de vincular o SLA global ao Serviço do Contrato, sendo:

**Primeira forma**:

1.  Clicar na aba "Serviços do Contrato" e em seguida "Gerenciar SLAs Globais";

2.  Selecionar o acordo de nível de serviço que deseja vincular ao Serviço do
    Contrato. Ao selecionar este acordo, será exibida uma lista de Serviços do
    Contrato;

3.  Selecionar os serviços desejados e clicar no botão "Gravar" para vincular o
    SLA com os serviços.

**Segunda forma**:

1.  Clicar na aba "Serviços do Contrato" e em seguida no ícone “Acordos de
    Nível de Serviço” do serviço desejado. Clicar no botão "Vincular Acordo" e
    preencher os campos necessários;

2.  Clicar em "Gravar" para efetuar a operação;

3.  Após efetuar o vínculo do acordo de nível de serviço ao serviço, clicar
    no botão "Habilita" para que o SLA seja habilitado.

Procedimento para registrar atividades do serviço do contrato
-------------------------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Serviços do Contrato" e em seguida no ícone “Atividades do
    Serviço” do serviço desejado;

4.  Apertar o botão "Adicionar Nova Atividade";

5.  Preencher os campos necessários com as seguintes recomendações:

    !!! Abstract "ATENÇÃO"

        Ao informar se deseja contabilizar as solicitações, lembrar que a
        contabilização será feita das solicitações "fechadas", no período da OS
        (Ordem de Serviço), do serviço do tipo requisição/incidente.**

    +  Se informar o tipo de custo como **Custo Total**, além dos campos gerais,
    será necessário indicar o custo total a complexidade da atividade;

    +  Se informar o tipo de como **Fórmula**, além dos campos gerais, será
    necessário selecionar a fórmula desejada. Feita a escolha, preencher os
    campos exibidos (horas, complexidade e quantidade).

6.  Clicar no botão "Gravar" para efetuar a operação.

Procedimento para verificar o desempenho do contrato
----------------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Serviços do Contrato" e em seguida no botão "Desempenho do
    Contrato";

Procedimento para excluir vínculo dos serviços com o contrato
-------------------------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Serviços do Contrato"*,* selecione o serviço a ser excluído.
    Depois, apertar no botão "Remover Serviço(s) do Contrato";

4.  Apertar em "OK" para confirmar a exclusão;

Procedimento para criar as ordens de serviço
--------------------------------------------

*Ordem de Serviço é um documento que irá fornecer a permissão de execução
relativa a algum serviço.*

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo o contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Ordens de Serviço" e em seguida no botão "Criar ordem de
    Serviço";

4.  Preencher os campos necessários.

    !!! Abstract "ATENÇÃO"

        Lembrar que caso o parâmetro 243 esteja habilitado, será acrescentado o
        campo Grupo de assinaturas.

        Após o preenchimento dos campos, será realizado o arrendondamento do custo
        total, após a soma dos custos totais de cada atividade do serviço.

5.  Clicar no botão "Gravar Dados" para efetuar a operação.

Procedimento para verificar as informações de ordem de serviço
--------------------------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo o contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Ordens de Serviço" e utilizar os botões contidos na barra
    (todas, em criação, solicitada, autorizada, aprovadas, em execução,
    executada e canceladas) para verificar as ordens de serviço por situação.
    Também poderá buscar as ordens de serviço por período;

4.  Ao lado de cada registro de Ordem de Serviço, serão exibidos ícones que
    possibilitarão a edição da OS, impressão da OS e RA (relatório de
    atividade), geração de RA e execução da OS.

Procedimento para editar a ordem de serviço
-------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Ordens de Serviço" e pesquisar a ordem de serviço desejada;

4.  Apertar no ícone “Editar a OS” da OS que deseja editar;

5.  Alterar os dados conforme a necessidade e clicar no botão "Gravar" para
    efetuar a operação.

Procedimento para imprimir a ordem de serviço
---------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo o contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Ordens de Serviço" e pesquisar a ordem de serviço desejada;

4.  Apertar no ícone “Imprimir a OS” para gerar o relatório da OS em formato PDF
    para impressão;

5.  Apertar no ícone “Imprimir a OS” para gerar o relatório da OS em formato
    Excel para impressão.

    !!! Abstract "ATENÇÃO"

        O Relatório de Atividade (R.A) só pode ser gerado a partir das ordens de
        serviço com uma situação "Aprovado".

Procedimento para gerar o relatório de atividade (R.A)
------------------------------------------------------

*O R.A (Relatório de Atividades) serve para comprovar que o serviço foi
entregue.*

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo o contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Ordens de Serviço" e em seguida na guia Aprovadas;

4.  Apertar no ícone “Gerar R.A” da OS aprovada e preencher os campos
    necessários;

5.  Pressionar o botão "Gravar" para efetuar a operação.

Procedimento para executar a ordem de serviço
---------------------------------------------

*Somente as Ordens de Serviço que foram geradas R.A (Relatório de atividades)
podem ser executadas.*

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Ordens de Serviço". Após gerar o R.A da OS, pressione a guia
    "Em execução";

4.  Apertar o ícone “Expandir OS” da OS para expandir a área e exibir os
    relatórios de atividade da OS.

5.  Pressionar o ícone “Executar OS” da OS desejada e mudar a situação da mesma
    para Executada e clicar no botão "Gravar dados" para efetuar a operação.

6.  Após executar a OS, poderá gerar uma fatura para a mesma.

Procedimento para criar fatura
------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Faturas" e em seguida no botão "Criar Fatura";

4.  Preencher os campos necessários. É possível vincular a OS à fatura ao clicar
    no botão "Adicionar OS", selecionar a OS já executada e, depois, clicar em
    "Associar" para efetuar a adição;

5.  Clicar em "Gravar" para efetuar a operação.

Procedimento para verificar as faturas
--------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo o contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Faturas" e utilizar os botões contidos na barra (todas, em
    criação, solicitada, autorizada, aguardando aprovação e aprovadas) para
    verificar as faturas por situação. Também poderá buscar as faturas por
    período;

4.  Ao lado de cada registro de Ordem de Serviço, serão exibidos ícones que
    possibilitarão a edição da fatura (em criação), impressão da fatura tanto no
    formato PDF como no formato Excel e apontamento da situação para fatura;

Procedimento para editar as faturas
-----------------------------------

*Somente as faturas que estão "na criação" podem ser editadas.*

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo o contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Faturas" e em seguida no ícone “Editar a Fatura” da fatura
    que deseja editar. Alterar os dados conforme a necessidade e apertar o botão
    "Gravar" para efetuar a operação.

Procedimento para imprimir a fatura
-----------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Fatura" e pesquisar a fatura desejada;

4.  Apertar no ícone “Imprimir a Fatura” para gerar o relatório da fatura em
    formato PDF para impressão;

5.  Apertar no ícone “Imprimir a Fatura” para gerar o relatório da fatura em
    formato Excel para impressão.

Procedimento para apontar a situação da fatura
----------------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Fatura" e pesquisar a fatura desejada;

4.  Apertar no ícone “Apontar situação para a Fatura” da fatura que deseja
    apontar uma situação. 

5.  Alterar a situação e clicar em "Atualizar Situação da Fatura" para efetuar a
    operação.

Procedimento para adicionar notificação
---------------------------------------

1.  Acessar a funcionalidade através da navegação no menu principal Gestão
    Integrada \> Gerência de Contratos \> Administração de Contratos;

2.  Clicar sobre o campo contrato e selecionar o contrato desejado. Em seguida
    clicar no botão "Pesquisar";

3.  Clicar na aba "Notificações" e em seguida no botão "Adicionar Notificação";

4.  Preencher os campos necessários. Lembrar que é possível adicionar um usuário
    ou grupo ao apertar no ícone disponível e pesquisar e vincular o item
    desejado;

5.  Pressionar o botão "Gravar" para efetuar a operação.

Relacionado
----------------------------------------------
[Acordo de Nível de Serviço](/pt-br/citsmart-7/processes/service-level/use/service-level-agreement.html)

[Cadastrar um grupo](/pt-br/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Cadastrar um contrato](/pt-br/citsmart-7/processes/portfolio-and-catalog/configuration/register-contract.html)

[Configurar modelo de e-mail](/pt-br/citsmart-7/platform-administration/email-settings/email-templates-configure-email-template.html)

[Cadastrar um serviço](/pt-br/citsmart-7/processes/portfolio-and-catalog/use/register-a-service.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RNUc7XoNAAOyo3Ex5fKM2db)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/17/2019 – Larissa Lourenço

