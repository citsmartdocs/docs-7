title: Configurar uma caixa de e-mail
Description:Configurar o envio e o recebimento de e-mail a partir de diferentes servidores com vistas a atender contratos distintos, assim um mesmo CITSmart poderá atender diferentes clientes e cada um terá sua própria caixa de e-mail.
# Configurar uma caixa de e-mail

Esta funcionalidade tem por objetivo configurar o envio e o recebimento de
e-mail a partir de diferentes servidores com vistas a atender contratos
distintos, assim um mesmo CITSmart poderá atender diferentes clientes e cada um
terá sua própria caixa de e-mail. Neste caso, é possível utilizar uma conta de
e-mail de envio/leitura (Ex: email@empresa.com) em um contrato da empresa XPTO
e outra conta de e-mail pertencente a um contrato de empresa distinta (Ex:
email@empresa2.com).

Procedimento
----------------

1.  Acessar a funcionalidade através da navegação no menu principal
    Parametrização \> Caixa de e-mail;

2.  Clicar no botão "Novo";

3.  Escolher o tipo de caixa. Se optar pelo tipo "Entrada" (significa que o
    usuário irá parametrizar uma rota por onde os e-mails que precisam ser lidos
    chegarão), serão abertos novos campos cadastrais, tais como: servidor, porta
    do servidor, usuário (endereço do e-mail), senha , provider e pasta da caixa
    de entrada, sendo portanto, necessário preencher os campos;

4.  Se optar pelo tipo "Saída" (significa que o usuário irá parametrizar uma
    rota por onde os e-mails que precisam ser enviados a partir do sistema
    sairão), serão abertos novos campos cadastrais, tais como: servidor, porta de
    servidor, usuário, senha, remetente, definir se será necessário a
    autenticação TSL/SSL (ambos são protocolos de segurança) e a autenticação do
    usuário sendo portanto, necessário preencher os campos;

5.  Clicar no botão "Gravar" para efetuar a operação;

6.  Vincular a caixa de e-mail ao contrato. Para tanto: acessar a funcionalidade
    Processos \> Gerência de Portfólio e Catálogo \> Contrato e vincular no
    campo *Caixa de e-mail* a caixa de e-mail previamente cadastrada e clicar no
    botão "Gravar" para efetuar a operação;

7.  Vincular a caixa de e-mail a um fluxo. Para tanto:

    -   Acessar a funcionalidade Sistema \> Manutenção de fluxos e ao
        cadastrar/editar um fluxo, localizar na aba "Diagrama" o conector "Envio de mensagem - email" no fluxo e clicar para editar;

    -   Na opção "Configuração da caixa de saída de e-mail", aberta ao clicar
        sobre a aba *Mensagem*, selecionar a opção "Específica" para utilizar a
        caixa de e-mail configurada no contrato;

    -   Concluir a parametrização do fluxo incluído os "Destinatários"
        selecionados;

    -   O uso de diferentes caixas de e-mail de saída poderá ser percebido após
        aberta uma solicitação de serviço, que possui parametrizado o fluxo que
        possui a caixa de e-mail selecionada;

    -   Clicar no botão "Gravar" para efetuar a operação.

!!! Abstract "ATENÇÃO"

    Vincular a caixa de e-mail não é um passo obrigatório. Esta funcionalidade
    somente será necessária ao cadastrar o fluxo, o usuário sentir necessidade
    de direcionar o e-mail para uma caixa de saída diferente da padrão. O e-mail
    de saída padrão do sistema continuará funcionado, mesmo que esta
    parametrização não seja feita.

    
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 – Anna Martins



