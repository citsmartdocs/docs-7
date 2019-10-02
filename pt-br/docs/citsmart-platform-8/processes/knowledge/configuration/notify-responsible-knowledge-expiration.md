title: Notificar responsável da expiração de conhecimento
Description: Tem por objetivo configurar a notificação por e-mail para avisar o responsável (criador e publicador) acerca da expiração de conhecimentos.
# Notificar responsável da expiração de conhecimento

Este conhecimento tem por objetivo configurar a notificação por e-mail para
avisar o responsável (criador e publicador) acerca da expiração de
conhecimentos.

Antes de Começar
--------------------

É necessário ter ao menos um conhecimento cadastrado na base de conhecimento.

Procedimento
----------------

1.  Configurar o parâmetro 78 com a quantidade de dias anteriores a expiração do
    conhecimento do qual deseja notificar o responsável pelo conhecimento;

2.  Criar um rotina de processamento batch de notificação:

    -   Acessar a funcionalidade através do menu principal Sistema \>
        Processamento Batch e clicar no botão "Novo";

    -   Definir a descrição da rotina, selecionar o tipo "Classe Java" e
        estabelecer a situação como "Ativo";

    -   Selecionar o agendamento como "Diário" e indicar o horário em que será
        processado a rotina;

    -   Na área "Conteúdo" copiar o script abaixo:

        -   br.com.centralit.citcorpore.quartz.job.VerificaValidadeBaseConhecimento

    -   Clicar no botão "Gravar" para efetuar a operação.

3.  Se desejar, é possível personalizar o modelo de e-mail. Basta acessar a
    funcionalidade através do menu principal Sistema \> Configuração \> Modelo
    de e-mail, selecionar o modelo de e-mail com ID = "7" e realizar a mudança
    pretendida.


Relacionado
----------
[Configurar parametrização - conhecimento](/pt-br/citsmart-7/platform-administration/parameters-list/configure-parametrization-knowledge.html)

[Criar conhecimento](/pt-br/citsmart-7/processes/knowledge/use/create-knowledge.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RMbaWr-pRsc9bsaVnc_xTzd)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/16/2019 - Anna Martins
