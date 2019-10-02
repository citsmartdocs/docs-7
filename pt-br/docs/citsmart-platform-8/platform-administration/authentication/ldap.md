title: Cadastrar conexões LDAP
Description: Permite gerenciar diretórios, ou seja, acessar bancos de informações sobre os usuários de uma rede por meio de protocolos TCP/IP.

# Cadastrar conexões LDAP

O LDAP (*Lightweight Directory Access Protocol* - Protocolo de acesso aos
diretórios leves) é um protocolo padrão que permite gerenciar diretórios, ou
seja, acessar bancos de informações sobre os usuários de uma rede por meio de
protocolos TCP/IP.

Essa funcionalidade permite cadastrar múltiplas conexões LDAP e definir as
configurações para cada uma delas.

![Autenticação CITSmart LDAP](images/cloud-arch-authentication.png)

Antes de começar
--------------------

É preciso ter cadastrado o horário para agendamento da sincronização automática.

Procedimento
----------------

1.  Acessar o menu principal Parametrização > Configuração LDAP;

2.  Clicar no botão "Novo";

    !!! Abstract "REGRA"

        Todos os campos são igualmente relevantes para viabilizar a conexão com o
        LDAP, enquanto o teste não for bem-sucedido o procedimento de configuração
        não pode ser considerado completado.

3.  Preencher os campos disponibilizados;

    !!! Abstract "REGRA"

        Caso não exista grupos LDAP, preencher o campo “DN Grupo” apenas com um
        asterisco. Isto fará com que o sistema verifique todo o domínio.

4.  É possível vincular novos grupos, para isso clicar no botão "Adicionar" na
    área **Grupos LDAP**;

    !!! Abstract "REGRA"

        Antes de pedir para testar **deve-se** clicar o botão "Gravar" para salvar a
        configuração, caso contrário o teste usará os dados anteriores às alterações
        feitas na tela.

        Quando há um pedido de autenticação na tela de identificação do sistema
        (login e senha) é executado um ciclo de busca da conexão correta com base
        nesta configuração, ou seja, há uma tentativa de autenticação para cada
        domínio aqui cadastrado (isso se houver mais de um).

5.  É possível vincular mapas de campos, para isso clicar no botão "Adicionar"
    na área **Mapeamento de campos**;

6.  Clicar no botão "Gravar".

    !!! Abstract "REGRA"

        O sistema não permite excluir um usuário que tem origem no LDAP.

### LDAP Seguro (LDAPs)

```sh
URL: ldaps://your-host.com:636
```

!!! success "Certificado digital"

    Exportar o certificado público do servidor LDAP e adicionar no repositório de certificados CA de Java de sua instância CITSmart.


Relacionado
-----------

[Cadastrar horário](/pt-br/citsmart-7/processes/event/configuration/register-time.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 - Anna Martins
