title: Pesquisar ticket no modo avançado 
Description: Permite refinar a busca pelos tickets através filtros taxativos. 
# Pesquisar ticket no modo avançado

A funcionalidade permite refinar a busca pelos tickets através filtros
taxativos.

Antes de começar
----------------

Para realizar a pesquisa avançada dos ticket é necessário o cadastro prévio do
mesmo e possuir chamados abertos, em qualquer situação e configurar os seguintes
parâmetros: 40, 41, 261, 260 (com o valor default 1-Lista sem Restrição), 343
(com o valor default: "S") e o parâmetro 378 (se o usuário informar o valor
igual a 0, o sistema sempre irá fazer o download em segundo plano. Se o usuário
deixar o campo em branco, o sistema limita o download em segundo plano para
cinco mil registros. Se o usuário colocar valor superior ou inferior a cinco mil
registros o sistema considera o valor informado pelo usuário).

Procedimento
------------

1.  Acessar a funcionalidade Ticket navegando pelo menu principal Processos \>
    Gerência de Requisição e Incidente \> Ticket;

2.  Clicar no botão de menu localizado no canto superior esquerdo a tela e em
    seguida no item de "Pesquisa Avançada";

3.  Preencher os filtros com a informação desejada. Lembrando que a eficácia da
    pesquisa depende do seguimento de algumas regras de permissão pelo filtro,
    tais como: execução, delegação, acompanhamento, visualização, grupo de
    usuários, vínculo com contrato, unidades e colaborador logado. Por isso,
    caso o parâmetro 61 esteja habilitado, serão disponibilizados somente as
    unidades vinculadas ao contrato ao qual tem vínculo com os grupos a que
    pertence;

4.  No filtro “Unidade”, o sistema pesquisa pelas Unidades que o usuário poderá
    atender. O sistema apresenta as Unidades que o usuário logado pode atender
    de acordo com o vínculo de grupo, uma vez que esse grupo é vinculado à
    contratos, e esses contratos possuem as Unidades vinculadas a eles;

5.  Clicar no botão "Pesquisar";

6.  Escolher um dos formatos de arquivo (PDF, XLS e CSV) para gerar o relatório.
    Depois de escolher o formato, o sistema verificará o parâmetro 261 e
    encontrando registro maior que a quantidade permitida, será exibida a
    seguinte mensagem:

    -   "A quantidade de registros encontrados ultrapassa a quantidade máxima
        permitida de visualização. Favor redefinir os filtros de pesquisa";

7.  Porém, caso a quantidade de registro retornada da pesquisa for menor que o
    limite no parâmetro 261, então o sistema verifica a configuração do
    parâmetro 378;

8.  É verificada a quantidade de registros para gerar o relatório em 2° plano,
    se a quantidade for maior que a quantidade parametrizada, então o sistema
    exibe a seguinte mensagem:

    -   "O relatório está sendo processado. Uma notificação lhe será enviada
        quando estiver pronto"

9.  Caso o arquivo a ser gerado for muito extenso, o sistema disparará uma
    notificação na tela principal, informando que o download do mesmo está
    finalizado. Ao concluir, clicar no botão "Visualizar" para acessar o
    relatório através do link disponibilizado.

Relacionado
-----------

[Criar um
ticket](/pt-br/citsmart-7/processes/tickets/use/create-ticket.html)

[Configurar parametrização -
ticket](/pt-br/citsmart-7/platform-administration/parameters-list/configure-parametrization-ticket.html)

[Configurar parametrização -
sistema](/pt-br/citsmart-7/platform-administration/parameters-list/configure-parametrization-system.html)

[Video
Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROn4Xs6UdH84Ujzta2iJ6Ei)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/17/2019 – Larissa Lourenço
