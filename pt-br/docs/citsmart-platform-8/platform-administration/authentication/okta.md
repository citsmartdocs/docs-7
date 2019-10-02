title: Configurar o Okta no CITSmart
Description: O Okta conecta qualquer usuário com qualquer aplicativo em qualquer dispoitivo. Este documento explica a forma ideial de conectar esta solução ao CITSmart.
# Configurar o Okta no CITSmart

Este método de autenticação permite que se utilize os recursos do Okta para autenticar usuários da organização em uma instância CITSmart. Este documento explica os passos da configuração deste método. Para saber mais sobre o Okta acesse [okta.com][1].

Antes de começar
--------------------

A configuração desta solução é um processo de diversas fases. A primeira fase é a criação de uma conta Okta.

Procedimento
----------------

*1º Passo: Criar uma conta Okta:*

1. Acessar o site:  https://www.okta.com;

2. Clicar em "Try Okta" e em seguida "Sign up today";

3. Informar os dados essenciais (e-mail, nome e sobrenome);

    ![Criar conta okta](images/okta.img1.png)

4. Apertar o botão "Get Started" para concluir a operação. Em seguida, verificar o e-mail cadastrado (que enviará um link de acesso), acessar a conta com a senha temporária enviada e alterar a mesma para maior segurança dos dados;

![Verificar e-mail](images/okta.img2.png)

*2º Passo: Criar a aplicação CITSmart dentro do Okta:*

1. Após concluído a etapa anterior, conectar-se ao Okta com a conta recém criada;

2. Clicar na aba "Applications e em seguida no botão "Add Application";

    ![Criar aplicação](images/okta.img3.png)

3. Apertar em "Create New App";

    ![Criar App](images/okta.img4.png)

4. Marcar a opção "SAML 2.0" e depois clicar no botão "Create";

    ![Opção SAML 2.0](images/okta.img5.png)

5. No campo "App name", adcionar o nome da aplicação e logo após, é necessário clicar no botão "Next";

    ![Nomear Aplicativo](images/okta.img6.png)

6. Configurar o caminho da aplicação e depois clicar no botão Next;

    ![Configurar caminho](images/okta.img7.png)

    !!! Abstract "ATENÇÃO"
    
        No campo "Single sign on URL" e "Audience URI (SP Entity ID)" deverá ser incluído os endereços de URL no qual a                 aplicação CITSmart será executada.

7. Marcar as opções "I'm an Okta customer adding an internal app" e "This is an internal app that we have created". Logo em seguida, clicar no botão "Finish".

    ![Marcar as opções](images/okta.img8.png)

*3º Passo: Atribuir usuários a aplicação CITSmart do Okta:*

1. Concluído o passo anterior, é necessário clicar na aba "Applications > Applications" e em seguida em "Assign Applications" e optar pelo filtro chamado "People";

    ![Atribuição de usuários](images/okta.img9.png)

2. Em seguida, é possível escolher o usuário que terá a permissão de acessar a aplicação que está sendo criada. Clicar então no botão "Assign" e posteriormente para finalizar, clicar em  "Done";

    ![Escolhendo o usuário](images/okta.img10.png)

*4º Passo: Incluir informações necessárias no CITSmart configurado no Okta:*

1. Será necessário configurar alguns dados no diretório do WildFly. Acessar o diretório, abrir a pasta "/standalone/configuration" e alterar o arquivo "citsmart.cfg".

    ![Diretório Wildfly](images/okta.img11.png)

2. Acessado o arquivo, é preciso incluir estas informações no arquivo "citsmart.cfg":
       
      a) Na linha *SAML2_HOST* e *SAML2_PORT* incluir o endereço e porta da aplicação CITSmart;
       
      b)  Na linha *SAML2_METADATA* incluir os metadados SAML do Okta. Este dado pode ser obtido seguindo as seguintes instruções:
 
      * Acessar a aplicação CITSmart no Okta, clicar na aba "Applications > Applications" e em seguida na opção "Sign On". Ao apertar a opção "Identity Provider metadata", será disponibilizado uma nova aba os metadados, copiar a URL do browser e inserir na propriedade *SAML2_METADATA* ;
        
    ![Sign On](images/okta.img12.png)

     c) Na linha *OKTA_URL*, incluir a URL principal da conta Okta.
   
     d) Na linha *OKTA_TOKEN*, incluir o token para acesso via API. Para obter este token, atenda estes passos:
   
   - Acessar a aplicação CITSmart no Okta, selecionar no menu a opção "Security > API" e em seguida clicar no botão "Create Token". Nomear o token e apertar o botão "Create Token". Será então apresentado o valor do token que deverá ser copiado na linha citado acima.
   
    ![Token](images/okta.img13.png)

     e) Na linha *OKTA_DOMAIN_ALIAS*, incluir o domínio dos usuários provinientes do Okta.
  
*5º Passo: Sincronizar usuário do Okta no CITSmart:*

1. Dentro do CITSmart, acessar o menu "Okta Config" e cadastrar uma nova configuração ao clicar no botão "Novo";

    ![Okta Confg](images/okta.img14.png)

2. Preencher os campos com as informações necessárias:

    ![Campos Okta Confg](images/okta.img15.png)

    * **Descrição:** introduzir uma definição desta nova configuração Okta;
     
    * **Alias:** incluir o domínio do usuário que será gravado na base. Exemplo: okta\administrador@citsmart.com;
     
    * **URL de domínio:** deverá incluir o mesmo valor (URL) que foi inserida na linha *OKTA_URL* no arquivo "citsmart.cfg"; 
     
    * **Token API:** incluir o mesmo valor do token inserido na linha *OKTA_TOKEN* no arquivo "citsmart.cfg";
      
    * **Grupo:** inserir o ID do grupo no qual o usuário sincronizado e gravado pertencerá no CITSmart;
     
    * **Perfil de Acesso:** inserir o ID do perfil no qual o usuário sincronizado e gravado pertencerá no CITSmart;
     
    * **ID da aplicação:** incluir o ID da aplicação. Esta informação pode ser recuperada na URL do Okta, conforme a figura abaixo:
     
      ![ID da URL](images/okta.img16.png)

3. Clicar no botão "Salvar" e em seguida "Sicronizar usuários" para efetuar a operação.

*6º Passo: Configurar o Logout:*

 1. Como o Okta não possui tela de logout, no parâmetro 377 do CITSmart podemos inserir algum endereço de página para redirecionar o usuário ao final da sessão;
 
 2. Configurar o link para logout também no endereço (**Admin > Settings > Customization > Sign-Out-Page)** , em seguida marcar a opção "Usar a custom sign-out page". Então, deve-se inserir a URL (https://localhost:8443/citsmart/saml/logout) com as devidas adaptações (host e porta), conforme a imagem abaixo:
 
 ![Logout](images/okta.img19.png)

!!!Abstract "NOTA"   
  
    Ao fazer o *logout* do CITSmart não deve ser realizado o *logout* do Okta, pois o usuário pode ter outras aplicações na sessão do Okta. Em contrapartida, se fizer o *logout* do Okta, a sessão do usuário no CITSmart será removida.
       
O que fazer a seguir
----------------------

Concluída a integração do Okta com o CITSmart, alguns parâmetros do CITSmart podem ser configurados para melhor personalizar esta integração:

 -  O parâmetro 445 (Nome do grupo Administrador no Okta) permite escolher o grupo administrador na solução Okta. Se o usuário pertencer a este grupo escolhido, terá o perfil de acesso definido como administrador. Caso o mesmo não tenha um perfil definido, o sistema atribuirá o parâmetro 39 e caso este usuário já tenha um perfil definido no CITSmart, este se manterá.
 
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>05/30/2019 – Larissa Lourenço

[1]: https://www.okta.com/
