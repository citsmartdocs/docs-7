Title: Implementar o Acesso Remoto

# Implementar o Acesso Remoto

A funcionalidade de acesso remoto permite que computadores sejam acessados remotamente a partir de sua instância CITSmart. Neste sentido, são utilizados os recursos do protocolo VNC (Virtual Network Computing) por intermédio do Apache Guacamole - Gateway de acesso remoto baseado na web - para tornar esta operação viável. Além de poder acessar remotamente um item de configuração, todas as sessões são gravadas e disponibilizadas junto às informações do IC. Isto garante um melhor controle sobre as ações realizadas, proporcionando um ambiente confiável e auditável.

Esta funcionalidade é um complemento (add-on) à Gerência de Configuração e depende do processo de inventário para tornar o acesso remoto viável a um IC.


## Antes de Começar

Os seguintes requesitos antecedem o uso efetivo desta funcionalidade:

* [x] Ter um processo de inventário definido e funcional utilizando o CITSmart Inventory;
* [x] Ter itens de configuração inventariados;

## Procedimento

1. Instalar o GuaCD utilizando a [documentação oficial][1] ou baixar o container disponibilizado pela CITSmart. Não é necessário 
instalar o guacamole-client, uma vez que o CITSmart utiliza apenas a daemon do Guacamole, ou seja, o GuaCD;

2. Após a instalação, configurar o apontamento de logs;
    
    ```sh
    /usr/local/sbin/guacd -b 0.0.0.0 > /var/log/guacd.log 2>&1
    ```

3. Baixar o binário (.jar) do encoder de vídeo (na central de downloads do portal do parceiro) - que tem a função de compilar os vídeos oriundos das sessões;

4. Copiar o enconder de vídeo para o servidor;

5. Realizar a configuração substituindo as variáveis pelas informações de seu servidor;
    
    ```java
    java -Durl=${CITSMART_PROTOCOL}://${CITSMART_URL}/citsmart -DcontainerIdentifier=${CITSMARTGUACD_ID} -DuserName=citsmart.local\\${CITSMART_LOGIN} -Dpassword=${CITSMART_PASSWORD} -jar /citsmart-guacd-encoder.jar &
    ```
    
6. Definir o diretório para gravação dos vídeos (ex. /mp4);
    
    !!! Abstract "Gravação de video"
    
        Após o encerramento da sessão de acesso remoto, o vídeo gerado 
        entra em uma fila de compilação para então, ser disponilizado na 
        plataforma. O tempo de compilação dependerá do tempo da sessão, 
        além disso, o início da compilação está atrelado à rotina cron 
        definida na conexão de acesso remoto.
        
7. No item de configuração que será acessado remotamente (ex. Computador Windows), instalar um cliente de acesso remoto com suporte ao 
protocolo VNC (Exemplo: [TightVNC][3]) e definir uma senha de acesso. Guardar esta senha pois ela será utilizada no próximo passo.
    
8. Realizar o cadastro de conexões de Acesso Remoto em sua instância [conforme o documento][4].


## O que fazer a seguir

Com o serviço do GuaCD ativo e comunicável, o próximo passo é acessar remotamente o IC configurado.

## Relacionado

[Gerenciamento de Configuração][5]

[Implementar o CITSmart Inventory][6]

[1]:https://guacamole.apache.org/doc/gug/installing-guacamole.html
[3]:https://www.tightvnc.com/
[4]:/pt-br/citsmart-7/processes/configuration/configuration/configure-remote-access.html
[5]:/pt-br/citsmart-7/processes/configuration/overview.html
[6]:https://docs-7.citsmart.com/pt-br/citsmart-7/additional-features/add-ons/inventory.html

