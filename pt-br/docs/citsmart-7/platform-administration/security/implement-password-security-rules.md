title: Implementar regras de segurança de senha
Description: Configuração de senhas de uso do sistema, disponibilizando maior nível de segurança com uso de diferentes caracteres.
# Implementar regras de segurança de senha

Esta funcionalidade retrata a configuração de senhas de uso do sistema,
disponibilizando maior nível de segurança com uso de diferentes caracteres.

!!! Abstract "ATENÇÃO"

    Esta política de segurança não está disponível para usuários LDAP.
     

Regras default ao habilitar a Política de Segurança:

-   Tamanho mínimo de 8 caracteres;

-   No mínimo uma letra minúscula;

-   No mínimo uma letra maiúscula;

-   No mínimo um número;

-   No mínimo um caracter especial (símbolo)

-   A senha não pode ser igual às últimas 3 utilizadas;

-   A senha expira em 3 meses

Procedimento
------------

1.  Acessar o menu principal Sistema \> Configurações \> Política de Segurança;

2.  Habilitar a chave “Habilitar política de senha”;

3.  No campo **Força da senha** o administrador deverá definir o número mínimo
    de caracteres da senha (valor mínimo de 8) e se a mesma conterá exigências
    de:letras maiúsculas, minúsculas, números e símbolos;

4.  Definir a quantidade de senhas anteriores na qual a nova não poderá ser
    igual, no limitador **A nova senha não pode ser igual às anteriores**;

5.  Para novos usuários a troca de senha poderá ser definida ao clicar na chave
    “Exigir a troca de senha no primeiro login”

6.  No campo **Duração da senha** definir o tempo de expiração da senha;

7.  Para usuários que já estejam em operação é possível forçar a troca de senha
    da nova configuração, a partir do próximo login, clicar na chave “Forçar
    troca de senha no próximo login para todos os usuários”;

8.  Clicar em “Salvar”.

!!! Abstract "NOTA"

    O Sistema notifica o usuário 3 dias antes da expiração da senha atual,
    fazendo este alerta através de mensangem em caixa de texto que surgirá uma
    vez ao dia ao realizar o login no sistema. Depois que a senha estiver
    expirada, o usuário é redirecionado automaticamente para a tela de perfil de
    usuário com painel de troca de senha aberto (somente poderá utilizar o
    sistema novamente se realizar a troca de senha).

!!! Abstract "NOTA"

    Para alterar a senha o usuário pode redefinir a senha por dois caminhos
    diferentes, ver [Cadastrar usuário][1] e [Editar informação da conta][2].


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/31/2019 - Anna Martins

[1]:/pt-br/citsmart-7/initial-settings/access-settings/user/users.html
[2]:/pt-br/citsmart-7/initial-settings/access-settings/user/user-data.html
