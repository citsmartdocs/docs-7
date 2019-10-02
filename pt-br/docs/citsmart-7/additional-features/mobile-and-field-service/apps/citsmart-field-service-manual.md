title: Manual de utilização do aplicativo CITSmart GO
Description: O objetivo do aplicativo CITSmart GO é permitir a realização de atendimentos em do técnico em campo no modo offline (onde o atendente não possui internet).
# Manual de utilização do aplicativo CITSmart GO

O objetivo do aplicativo CITSmart GO é permitir a realização de atendimentos do técnico em campo no modo offline (onde o atendente não possui internet).

Antes de começar 
-----------------

1.  Ter configurado o aplicativo na instância ITSM;

2.  Instalar o aplicativo CITSmart GO (Android e iOS);

3.  É necessário delegar tarefas ao técnico no site CITSmart para que o mesmo as
    possa atender em campo no modo offline.

Procedimento
------------

!!! Abstract "ATENÇÃO"

    Ao logar no aplicativo CITSmart GO, a primeira sincronização pode demorar
    alguns instantes, pois para funcionar offline tem que baixar todas as
    solicitações e enviar as que tiveram mudanças para que o aplicativo funcione
    corretamente.


1.  Informar os dados para login do aplicativo;

2.  Selecionar o ticket desejado e clicar sobre o mesmo. Será apresentado uma
    tela com os dados da solicitação, inclusive um mapa do local onde será
    realizado o atendimento;

    !!! warning "ATENÇÃO"

        A visualização de determinado ticket, além de estar condicionada às permissões do grupo pode estar atrelada também ao parâmetro 435 - que condiciona a visão no app apenas à ticket delegados para o usuário autenticado.

3.  Clicar no botão "Executar solicitação" e em seguida "Outras informações"
    (está opção só estará disponível se existir um questionário vinculado a
    atividade do ticket). Preencher os dados referentes a execução da
    solicitação e clicar em "Salvar".

    !!! warning "ATENÇÃO"

        Apenas componentes simples do Neuro, como os formulários, poderão ser renderizados no Mobile GO. Estes formulários não poderão ter nenhuma lógica de JavaScript vinculada a eles, devem ser similares ao questionário existente no CITSmart                     Experience.


    !!! Abstract "REGRA"

        Não é possível vincular uma IC e base de conhecimento pelo mobile GO.    

4.  Se desejar adicionar algum arquivo clicar na aba "Anexos";

5.  Se desejar adicionar alguma nota, clicar na aba "Notas". Relatar a ocorrência referente ao ticket e a data que a mesma ocorreu.         É possível também registrar o tempo gasto para a solução da ocorrência. É disponibilizado a visualização deste relato pelo               solicitante e o envio do mesmo para o e-mail dele ao selecionar as opções "Visível ao solicitante" e "Enviar ao e-mail". Clicar em       "Salvar".

6.  Clicar em "Finalizar" e completar os dados sobre a conclusão do atendimento.
    Selecionar a situação do atendimento (em andamento, resolvida ou cancelada)
    e o detalhar da mesma;

7.  Clicar em "Coletar Assinatura e Avançar o Fluxo" (ver documento relacionado) ou "Gravar e manter tarefa atual" para
    completar a operação. Serão então automaticamente sincronizadas as
    alterações. Se o aplicativo não encontrar a rede para completar a
    sincronização, será apresentado o ícone “Atualização automática” para
    aguardar o encontro de rede para e então completar a sincronização;

8.  Está disponível a sincronização manual das solicitações assim que o
    aplicativo encontrar uma rede acessível. Para tanto, basta deslizar a tela
    para baixo com o dedo ou clicar no ícone “Atualizar lista”;

9.  Existem filtros que facilitam a localização do ticket necessário, acesse o
    mesmo pela caixa de pesquisa ou clique no ícone “Filtros”.

Relacionado
-----------

[Configurar instância para uso do aplicativo CITSmart GO](/pt-br/citsmart-7/additional-features/mobile-and-field-service/configuration/configure-field-service-application.html)

[Obter assinatura em atendimento de campo](/pt-br/citsmart-7/additional-features/mobile-and-field-service/use/get-signature-in-attendance.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/17/2019 – Larissa Lourenço
