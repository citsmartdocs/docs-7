title: Cadastrar usuário
Description: Disponibiliza ações diversas, tais como, incluir, alterar e excluir um usuário.

# Cadastrar usuário

Para que o colaborador possa acessar o sistema é necessário criar um usuário. Ao registrá-lo é possível que os dados do usuário (login e senha) sejam enviados para o e-mail do colaborador. Para isso, configure o parâmetro 455 indicando o template de e-mail (ID) criado para esta finalidade. No template de e-mail devem constar as chaves ${LOGIN} e ${NOVASENHA}.

Esta funcionalidade disponibiliza ações diversas, tais como, incluir, alterar e
excluir um usuário.

!!! warning "ATENÇÃO"
    O envio de login e senha ao cadastrar novo usuário não engloba usuários importados via AD ou LDAP.

## Antes de começar

Para cadastrar um usuário é necessário:

- [X] Registrar o Colaborador;

- [X] Possuir no mínimo um Perfil de Acesso;

Para enviar o Login e a Senha do usuário para o e-mail do Colaborador:

- [X] Configurar o parâmetro 33 e indicar corretamente a URL da instância;

- [X] Configurar o parâmetro 455 com o ID do modelo de e-mail criado para enviar os dados de acesso;

!!! note "EXEMPLO"
    Modelo básico: "Prezado usuário, seguem dados de acesso. Usuário: ${LOGIN} e Senha: ${NOVASENHA}"

## Procedimento

1.  Acessar a funcionalidade através da navegação no menu principal Cadastros
    Gerais \> Gerência de Pessoal \> Usuário;

2.  Preencher os campos disponibilizados;

3.  Clicar em "Gravar".

!!! info "INFORMAÇÃO"
    O sistema verifica se existe um template de e-mail para novo colaborador que possua a chave de senha para envio via e-mail. O administrador do sistema cadastra ou altera um login e senha de um colaborador na tela de usuário. O sistema verifica se: o sistema utiliza a política de senha e o se usuário é LDAP ou não. O sistema permite a entrada de uma nova senha. Ao gravar o sistema envia por e-mail os novos dados ao colaborador.

## Relacionado

[Cadastrar um colaborador](/pt-br/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Criar perfil de acesso](/pt-br/citsmart-7/initial-settings/access-settings/profile/create-profile-access.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 – Anna Martins

