title: Notificar via email ticket delegado
Description: Permite implementar a forma de envio de email de um ticket delegado, assim os tickets delegados terão um modelo de email próprio a ser enviado ao técnico.
# Notificar via email ticket delegado

Este documento permite implementar a forma de envio de email de um ticket
delegado, assim os tickets delegados terão um modelo de email próprio a ser
enviado ao técnico.

Antes de começar
--------------------

Um modelo de email deverá ter sido cadastrado previamente e que as chaves a
serem usadas em seu corpo de texto deverão ser as seguintes:

```html
${IDSOLICITACAOSERVICO}

${SERVICO}

${SOLICITANTE}

${DESCRICAO}
```

Procedimento
----------------

1.  Acessar a funcionalidade através do menu Processos \> Gerência de Portfólio
    e Catálogo \> Portfólio;

2.  Escolher o portfólio, clicar em "Avançar";

3.  Escolher o serviço e clicar em "Avançar";

4.  Clicar na guia *Contratos*;

5.  Selecionar o contrato e clicar em "Avançar";

6.  Clicar na guia *Requisições* e clicar em "Editar";

7.  Escolher a atividade;

8.  No campo **Modelo de e-mail Delegação** escolher pelo modelo de e-mail
    cadastrado previamente;

9.  Clicar no botão "Gravar";

10.  Na tela de parametrização ativar os parâmetros 438 (informar modelo de email
    de delegação) e o 439 (opção “SIM”);

11.  Na tela de cadastro de grupo, no campo “Colaboradores”, marcar o checkbox
    “Email” das pessoas que irão receber o email daquele grupo.


O que fazer a seguir
--------------------

Acessar o ticket desejado e efetuar a delegação.


Relacionado
-------

[Delegar um ticket](/pt-br/citsmart-7/processes/tickets/use/delegate-ticket.html)

[Configurar modelo de email](/pt-br/citsmart-7/platform-administration/email-settings/email-templates-configure-email-template.html)

[Cadastrar um grupo](/pt-br/citsmart-7/initial-settings/access-settings/user/register-groups.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RN9wA1DbVHEot2QD2gW8_jq)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/16/2019 – Anna Martins
