title: Configurar instância para uso do aplicativo CITSmart GO
Description: O aplicativo CITSmart GO possibilita a realização de atendimentos em modo offline
# Configurar instância para uso do aplicativo CITSmart GO
O aplicativo CITSmart GO possibilita a realização de atendimentos em modo offline - em que o atendente não possui internet. Após o aplicativo se conectar a internet, a aplicação enviará, automaticamente, as informações para o ambiente em produção. Vale lembrar que a delegação da solicitação para um atendente deve ser realizada manualmente por um responsável.
 O atendente visualizará apenas solicitações que foram delegadas a ele.

Antes de começar
----------------

1.  Instalar o aplicativo CITSmart GO;

2.  No ambiente - instância do CITSmart -, configurar as seguintes
    funcionalidades:

    -   Webservice: indicar no item "permissões" os grupos de atendimento que poderão visualizar os tickets;

    -   Unidade: obter as coordenadas da unidade cadastrada.

Procedimento
------------

***Webservice***

1. Acessar a funcionalidade através do menu principal Sistema \> Webservice \>
    Operação Webservice;

2.  Na aba **Pesquisa de Operações**, buscar por cada um dos webservices
    abaixo, em seguida em cada um clicar no botão "Adicionar grupo" e incluir
    o(s) grupo(s) que o(s) atendente(s) estão vinculados:

    -   request_add_attachments

    -   request_updateRequestList

    -   request_userLocation

    -   request_saveRequest

    -   request_uploadAttachment

    -   request_getByUser
    
    -   request_saveRequestNote
    
    -   request_updateRequestNoteList
    
    -   request_updateRequestListGroups
    
    -   request_uploadSignature
    
    -   parameter_query

3.  Clicar no botão "Gravar" após configurar os grupos em cada webservice.

***Unidade***

1.  Acessar a funcionalidade através do menu principal Cadastros Gerais \>
    Gerência de Pessoal \> Unidade;

2.  Buscar pela unidade na aba Pesquisa de Unidade e selecionar a escolhida;

3.  Na aba Cadastro de Unidade com a unidade já escolhida, clicar no botão
    "Obter Coordenadas";

4.  Clicar em "Gravar".

O que fazer a seguir
--------------------

Logar no aplicativo CITSmart GO já instalado, inserindo a URL, usuário e a senha
do ambiente. Verificar os tickets e realizar atendimento.

Relacionado
-----------

[Manual de utilização do aplicativo CITSmart GO](/pt-br/citsmart-7/additional-features/mobile-and-field-service/apps/citsmart-field-service-manual.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/17/2019 – Larissa Lourenço
