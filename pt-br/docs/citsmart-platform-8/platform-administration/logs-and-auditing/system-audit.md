title:  Realizar auditoria no sistema
Description: Permite gerenciar os eventuais riscos ao sistema
# Realizar auditoria no sistema

Esta funcionalidade permite gerenciar os eventuais riscos ao sistema, ao auditar todas as execuções efetivadas no sistema em forma de logs.
Foram feitas algumas mudanças na auditoria (itsm-audit-0.4.0), mudanças essas apenas a nível de configuração.

Antes de começar 
-----------------

Configurar a funcionalidade "Audit" em sua instância.
   
Procedimento
------------

***Processo para configurar a Auditoria:***

*Configuração para gerar o backup das auditorias*.

Primeiramente, é imprescindível configurar os parâmetros específicos da
funcionalidade.

1.  Acessar a funcionalidade através da navegação no menu principal
    Parametrização \> Parametrização de Auditoria;

2.  Informar no campo “Diretório” a pasta onde será mantido todos *logs* de
    auditoria realizados;

3.  No campo “Frequência em dias” é possível ajustar uma rotina de backup dos
    logs de auditoria, ao escolher a periodicidade do backup em dias.

    !!! Abstract "NOTA"

        A escolha da frequência deve ser a partir de 1 (um) dia para a execução do backup.  

4.  É disponibilizado a possibilidade de determinar um período específico (data
    de início e fim) para a geração dos logs de auditoria do sistema.

    !!! Abstract "IMPORTANTE"

        São oferecidos três tipos de auditoria de sistema: auditoria dos dados do sistema, do acesso ao sistema e as licenças do mesmo.

***Auditoria de dados do sistema***

*Apresenta o histórico de todos dados de alteração, inclusão e exclusão
realizadas no sistema.*

1.  Acessar a funcionalidade através da navegação no menu principal Sistema \>
    Trilha de auditoria \> Auditoria de dados;

2.  Serão exibidos os logs de auditoria de toda movimentação realizada no
    programa, mostrando a data e hora das atualizações, o endereço de IP, o nome
    do executor da atualização, o nome da tabela, o tipo de operação efetivada
    no sistema. Ao clicar no botão "dados" será apresentado o que de fato foi
    atualizado no programa.

    !!! Abstract "ATENÇÃO"

        O campo “Operações” apresenta o tipo de ação realizada na atualização do
        sistema em tese. É definida por símbolos, e seus significados são:

        -   A letra “A” significa “Alteração” nos dados do sistema;

        -   A letra “I” simboliza a “Inserção” de novos dados ao sistema;

        -   A letra “E” significa a “Exclusão” de dados do sistema.  

3.  É liberado também a busca de determinado *log* através dos filtros dispostos
    na tela.

***Auditoria de acessos ao sistema***

*Apresenta o histórico dos acessos ao sistema (entradas e saídas).*

1.  Acessar a funcionalidade através da navegação no menu principal Sistema \>
    Trilha de auditoria \> Auditoria de acesso;

2.  Serão expostos os usuários que efetuaram o login e logout no sistema,
    registrando também a data e a hora de cada uma destas atividades;

    !!! Abstract "NOTA" 
    
        Se porventura o sistema expirar, não será possível captar o logout do
        sistema, ficando registrado, portanto, só as informações de entrada da
        sessão de acesso.  

3.  Existem filtros para auxiliar a busca de determinado acesso.

***Auditoria de licenças do sistema***

*Informa as licenças utilizadas para a validação do sistema.*

1.  Acessar a funcionalidade através da navegação no menu principal Sistema \>
    Trilha de auditoria \> Auditoria de licença;

2.  Apresenta os dados das licenças adquiridas e usadas para a execução do
    sistema;

3.  É possível pesquisar uma determinada licença e seu prazo de validade pelos
    filtros liberados na tela principal.
    
Relacionado
-------------
    
[Configurar o Audit 0.4.0](/pt-br/citsmart-7/platform-administration/logs-and-auditing/audit040-configure.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/15/2019 – Larissa Lourenço
