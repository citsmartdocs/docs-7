title: Configurar parametrização - LDAP
Description: Esta configuração de parâmetros ligados à integração com o LDAP ocorre de uma forma implícita usando a funcionalidade Configuração LDAP ou de forma explícita usando a funcionalidade Parâmetros do CITSmart.
# Configurar parametrização - LDAP

Ao contrário dos demais parâmetros do produto, esta configuração de parâmetros
ligados à integração com o LDAP ocorre de uma forma implícita usando a
funcionalidade Configuração LDAP ou de forma explícita usando a
funcionalidade Parâmetros do CITSmart.

Procedimento
----------------

1.  Acessar a funcionalidade através da navegação no menu principal
    Parametrização \> Parâmetros CITSmart;

2.  Definir o valor do parâmetro a ser configurado;

3.  Efetuar a mudança;

4.  Clicar no botão "Gravar";

5.  A lista abaixo apresenta os parâmetros da funcionalidade e a finalidade de
    cada um deles:

|  #  |                                               Nome                                              | Valores possíveis |                                                   Finalidade                                                   |                                                                                                                                             Orientações complementares                                                                                                                                            |
|:---:|:-----------------------------------------------------------------------------------------------:|:-----------------:|:--------------------------------------------------------------------------------------------------------------:|:-----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|  39 | LDAP - ID do perfil de acesso que será setado automaticamente caso o usuário não possua nenhum. |       Ex: 2       |               Informar o número de identificação (ID) do Perfil de Acesso padrão para o usuário.               | Ao cadastrar um usuário e caso não seja informado o perfil de acesso, quando o mesmo realizar login na aplicação, será estabelecido o perfil de acesso (definido no valor do parâmetro). Essa regra vale para os usuários importados do AD. Esse ID do Perfil de Acesso é definido na tela de “Perfil de Acesso”. |
|  45 |                                      LDAP - ID Grupo Padrão                                     |       Ex:123      |       Informar o número de identificação (ID) do grupo padrão, ao qual os usuários do AD serão associados      |                                                                                                                            Esse ID do grupo é definido na tela de "Cadastro de Grupo".                                                                                                                            |
| 409 |                  LDAP - Atributo que representa o superior imediato do usuário                  |     Ex: Maria     | Nome do superior imediato do usuário no LDAP para que se consiga recuperar essa informação pelo AD do cliente. |                                                                                                                           Para poder usar em casos de aprovação de um ticket por exemplo                                                                                                                          |


Tabela 1 - Tabela de parâmetros

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 - Anna Martins
