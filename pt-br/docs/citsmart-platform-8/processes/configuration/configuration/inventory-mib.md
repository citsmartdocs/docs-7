Title: Coletar dados de hardware a partir de MIBs (SNMP)

# Coletar dados de hardware a partir de MIBs (SNMP)

É possível coletar dados de ativos de hardware, utilizando o protocolo SNMP - via coleta de MIBs - e adicionar à informações de um item de configuração no processo de Gerência de Configuração.

## O que fazer antes

- [X] É necessário ter implantada a versão do CITSmart Inventory 1.2.1.9 ou superior (ver [Realizar a instalação][1]);
- [X] No arquivo standalone-full.xml deve ser adicionada a propriedade `snmp.oid.repository.directory` contendo o caminho da pasta onde estarão os arquivos xml com o layout (Ver [Configuração do System Properties][2]);
- [X] Ter um processo de inverário definido via Gerência de Configuração (ver [Implementar o CITSmart Inventory][3]);
- [X] Inventariar o item de configuração, via SNMP, para a coleta de MIBs (ver [Configurar conexão inventory][4]);


## Criar o Modelo

Modelo:

```xml
<SEU-TIPO-ITEM oid-validator="(OID de uma propriedade específica que irá permitir que seja interpretado o resto do arquivo. Caso não retorne valor, o TIPO-ITEM não é criado.)">
                <SUA-CARACTERISTICA>(OID da informação desejada)</SUA-CARACTERISTICA>
                <CARACTERISTICA-EM-HEXA type="hex">(OID da informação que o valor retornado precisa ser convertido de HEXADECIMAL)</CARACTERISTICA-EM-HEXA>
</SEU-TIPO-ITEM>
```

Exemplo:

```xml
<IMPRESSORA oid-validator=".1.3.6.1.2.1.43.5.1.1.16.1">
                <NAME>.1.3.6.1.2.1.43.5.1.1.16.1</NAME>
                <DESCRIPTION type="hex">.1.3.6.1.2.1.43.5.1.1.16.1</DESCRIPTION>
                <QTD-PAGINAS-IMPRESSAS>.1.3.6.1.2.1.43.10.2.1.4.1.1</QTD-PAGINAS-IMPRESSAS>
                <CAPACIDADE-TOTAL-TONER>.1.3.6.1.2.1.43.11.1.1.8.1.1</CAPACIDADE-TOTAL-TONER>
                <CAPACIDADE-ATUAL-TONER>.1.3.6.1.2.1.43.11.1.1.9.1.1</CAPACIDADE-ATUAL-TONER>
</IMPRESSORA>
```

## Implantar o Modelo

Após a criação do modelo é necessário salvá-lo na pasta indicada no parâmetro   `snmp.oid.repository.directory` do servidor de aplicação. Após a implantação do modelo, no momento da execução do inventário a aplicação irá checar os ICs que possuem as MIBs indicadas e automaticamente irá atualizar os ativos com as informações coletadas.


!!! danger "CUIDADO"

    1. Os arquivos de layout podem ter qualquer nome. Todos os arquivos da pasta serão interpretados, portanto só poderão existir arquivos XML dentro dela;
    2. Caso exista mais de um layout, pode ser colocado dentro do mesmo arquivo ou em arquivos diferentes. Só deve-se respeitar o formato de XML;

!!! exemple "LINKS ÚTEIS"

    1. http://www.oidview.com/mibs/ - Repositório contendo milhares de MIB’s separado por fabricantes.
    2. http://ireasoning.com/mibbrowser.shtml - Ferramenta MibBrowser que pode auxiliar na coleta das OID’s.

[1]:/pt-br/citsmart-7/get-started/installation-and-upgrade/perform-installation.html
[2]:/pt-br/citsmart-7/get-started/installation-and-upgrade/perform-installation.html#configuracao-do-system-properties
[3]:/pt-br/citsmart-7/additional-features/add-ons/inventory.html
[4]:/pt-br/citsmart-7/processes/event/configuration/set-inventory-connection.html
