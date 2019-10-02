title: Configurar conexão Inventory
Description: Tem como objetivo cadastrar todas as propriedades referentes à conexão do CITSmart Inventory, de acordo com o IP e porta onde está instalado o Jboss do CITSmart Inventory.
# Configurar conexão Inventory

Esta funcionalidade tem como objetivo cadastrar todas as propriedades referentes
à conexão do CITSmart Inventory, de acordo com o IP e porta onde está instalado
o Jboss do CITSmart Inventory.

Antes de começar
--------------------

A configuração da funcionalidade requer um servidor com aplicação Inventory
funcional e comunicável com o ITSM.

Procedimento
----------------

1.  Acessar a funcionalidade através da navegação no menu principal Processos \>
    Gerência de Evento \> Conexões \> Inventory;

2.  Na área **Dados da Conexão**, preencher os campos;

3.  Selecionando o tipo de conexão *Inventory*, no campo "Ignorar máquinas já
    inventariadas" (no caso de máquinas inventariadas é possível definir quantos
    dias essa máquina ficará sem novo inventário e por isso seu Status será
    colocado como Ignorado até que se passe o total de dias parametrizado) serão
    abertas duas caixas que se referem a Período e Formato do período, marcar a
    opção que melhor se encaixe e gravar as configurações;

    ![inventory integracao](images/conexao-inventory.jpg)

       Figura 1 -Integração CITSmart inventory


4.  Se o tipo de conexão escolhida for o OCS Inventory será apresentado o campo de configuração do mesmo para ser informado o repositório de XML, conforme ilustrado abaixo. Além disso, existem alguns *pré-requisitos* muito relevantes que devem ser observados:

    ![ocs](images/conexao-inventory-2.jpg)
   
    Figura 2 -Integração CITSmart inventory - OCS inventory


     -   Após instalar o OCS Inventory, ele não vem como padrão qualquer tipo de
         integração com outro sistema, para isso no menu Inventory files precisa
         atribuir GENERATE_OCS_FILES = ON, OCS_FILES_FORMAT = XML e especificar o
         caminho onde irão ser guardados os arquivos XML em OCS_FILES_PATH

    -   O local especificado para a geração dos arquivos XML é algo muito
        estratégico:

        -   Caso o servidor OCS seja o mesmo servidor do Inventory, trata-se do
            menor risco pois a pasta provavelmente estará acessível para leitura;

        -   Caso o servidor OCS **NÃO** seja o mesmo servidor do Inventory, deve-se
            optar por uma dessas duas opções:

            -   o OCS Inventory deve ter permissão para gravar no servidor do
                Inventory;

            -   o Inventory deve ter permissão (compartilhamento) no servidor OCS
                Inventory.

5.  A aplicação de Inventário realiza a captura dos dados por meio da porta do
    Agente SNMP (161) e/ou pelo Agente de Captura (porta 7103 desenvolvido pela
    CITSmart Corporation, em .Net). Inicialmente, o Inventory realiza um comando
    "ping" para verificar se a máquina está ativa. Se conseguir realizar o
    comando, tentar acessar a porta SNMP do item de configuração. Se o acesso à
    porta não for obtido com sucesso, o Inventory tenta realizar o acesso
    através do agente de captura, clicar no botão "Testar Conexão";

6.  Clicar no botão "Gravar e Aplicar Configurações".

Relacionado
-------

[Cadastrar gerente Inventory](/pt-br/citsmart-7/processes/event/configuration/register-inventory-manager.html)



!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/15/2019 - Anna Martins
