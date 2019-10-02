Title: Implementar o CITSmart Inventory

# Implementar o CITSmart Inventory

O CITSmart Inventory é um componente da Plataforma CITSmart que permite coletar, registrar e gerenciar informações de ativos de T.I. Ele possibilita gerenciar o ciclo de vida dos itens de configuração de sua organização a partir do processo de Gerenciamento de Configuração.

![Arquitetura EVM e INV](images/cloud-arch-inv-evm.png)

Antes de começar
------------

O CITSmart Inventory trabalha em conjunto com o [Monitor de Eventos CITSmart - EVM][1], pois este serve como um orquestrador de dados. Portanto, para utilizar o Inventory, deve-se primeiro configurar o EVM.


## Procedimento

1. [Instalar][2] o servidor de aplicação Wildfly;
2. Fazer download do pacote WAR do componente Inventory;  
3. Descompactar os arquivos;  
4. Copiar o pacote para a pasta de implantação do servidor de aplicativos Wildfly (ex. /deployments);  
5. Configurar as [Propriedades do Sistema][3] com os dados da instância CITSmart.

## O que fazer depois  

Para testar o Inventory, [configurar][4] as conexões na instância CITSmart.

## Relacionado

[Implementar o CITSmart Event Monitor][5]

[Gerenciamento de Configuração e Ativo][6]


[1]:/pt-br/citsmart-7/additional-features/add-ons/event-monitor.html
[2]:/pt-br/citsmart-7/get-started/installation-and-upgrade/perform-installation.html
[3]:/pt-br/citsmart-7/get-started/installation-and-upgrade/perform-installation.html#configuracao-do-system-properties
[4]:/pt-br/citsmart-7/processes/event/configuration/set-inventory-connection.html
[5]:/pt-br/citsmart-7/additional-features/add-ons/event-monitor.html
[6]:/pt-br/citsmart-7/processes/configuration/overview.html



!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/22/2019 - João Pelles  
	
