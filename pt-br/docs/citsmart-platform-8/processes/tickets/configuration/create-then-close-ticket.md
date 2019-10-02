title: Como criar e, em seguida, encerrar um ticket
Description: Para atividades que não exigem um SLA, onde o atendente deseja apenas formalizar a requisição e execução da atividade, é possível configurar para que ocorra a criação e encerramento do ticket ao mesmo tempo.
# Como criar e, em seguida, encerrar um ticket

Para atividades que não exigem um SLA, onde o atendente deseja apenas formalizar
a requisição e execução da atividade, é possível configurar para que ocorra a
criação e encerramento do ticket ao mesmo tempo.

Procedimento
----------------

1.  É possível definir o fluxo de criação e encerramento do ticket de duas
    formas distintas:

    - **1° Modo - Importar o fluxo**: é possível importar o fluxo com o script já
      cadastrado. Basta realizar download do anexo "Fluxo JSON" e acessar a
      funcionalidade do fluxo (Workflow \> Desenho de Fluxo), clicar no botão
      "Novo", logo em seguida apertar o botão "Importar" e selecionar a opção "JSON".
      Realizar o upload do anexo e clicar em "Importar". Em seguida, para verificar o
      script, clicar na aba "Diagrama" e no ícone tarefa, e depois, apertar a aba
      "Ação de entrada";

    - **2° Modo - Copiar o script:** já para copiar apenas o script, copiar o conteúdo
      do anexo "Script" e acessar a funcionalidade do fluxo (Workflow \> Desenho de de
      Fluxo), clicar no botão "Novo" e preencher os campos necessários. Depois,
      clicar na aba **Diagrama**, desenhar o fluxo referente a criação e encerramento
      de uma tarefa, selecionar e clicar sob a esta tarefa (pequena caixa cinza ao
      lado da tarefa) e na aba "Ação de entrada". É necessário copiar o RhinoScript no
      construtor de expressões, clicar no botão "Construir expressões" e selecionar a
      expressão do cadastro.

!!! Abstract "ATENÇÃO"

    Não foram implementados controles para informações de captura pois o tempo
    de atendimento e fechamento do ticket é muito curto, caso seja necessário
    fazer o mesmo, será preciso implementar o registro das informações nas
    tabelas de captura.

Anexo
------
[Download-Fluxo JSON][1]

[Download-script][2]


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RN9wA1DbVHEot2QD2gW8_jq)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/16/2019 – Anna Martins


[1]:/pt-br/citsmart-7/processes/tickets/images/fluxo-JSON.json
[2]:/pt-br/citsmart-7/processes/tickets/images/script.zip
