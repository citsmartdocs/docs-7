title: Processamento Batch
Description: Tem o objetivo de registrar o processamento batch, que poderá ser utilizado em outras rotinas do sistema.
# Processamento Batch

Esta funcionalidade tem o objetivo de registrar a utilização de processamento batch, que
poderá ser utilizado em outras rotinas do sistema.

Rotinas como:

   - Verificação de e-mail
   
   - Verificação da hora do servidor
   
   - Distribuição automática de Tickets com balanceamento carga de trabalho
   
## Antes de Começar

O processamento Batch do CITSmart utiliza o Quartz para o agendamento e processamento de rotinas de sistema. Sendo assim, antes de utilizar qualquer rotina batch é necessário [configurar o Quartz][3].

Procedimento
----------------

1.  Acessar a funcionalidade através da navegação no menu principal Sistema \>
    Processamento Batch;

2.  Clicar no botão "Novo";

3.  Preencher os campos disponibilizados (descrição, tipo [classe Java,
    RhinoScript, SQL]; situação; expressão cron que define o horário de execução
    da rotina e o conteúdo da rotina, onde será descrito o contexto da rotina a
    ser executada na ferramenta);
    
    Exemplo de conteúdo "Classe Java":
    
    ```java
    br.com.centralit.citcorpore.quartz.job.JobConfiguracaoAberturaAutomaticaViaEmail
    ```

4.  Clicar em "Gravar".

Rotinas Batch
-----------------

-   Retornar horário do Servidor

    -   Tipo: RhinoScript
    -   Conteúdo:
    
        [Baixar Script][2]

-   Realizar leitura de e-mail

    -   Tipo: Classe Java
    -   Conteúdo:
    
   ```java
   br.com.centralit.citcorpore.quartz.job.JobConfiguracaoAberturaAutomaticaViaEmail
   ```


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 – Anna Martins


[1]:/pt-br/citsmart-7/platform-administration/configuring-automatic-actions/images/verify-email.txt
[2]:/pt-br/citsmart-7/platform-administration/configuring-automatic-actions/images/server-time.txt
[3]:/pt-br/citsmart-7/get-started/installation-and-upgrade/perform-installation.html#configuracao-do-quartz
