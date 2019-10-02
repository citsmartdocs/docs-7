title: Criar um grupo
Description: Permite o cadastro de grupos e o vínculo deles com usuários, um perfil, contratos e e-mails para notificação.


# Criar um Grupo

Um grupo é um conjunto de um ou mais colaboradores que tem os mesmos objetivos relacionados as suas funções.

Os dois usos mais comuns para os grupos criados são:


1.  Gestão da segurança/sigilo de acessos a vários tipos de cadastros (ex.: pastas da base de conhecimento, portfólios de serviços, etc.).

2.  Programação de notificação automática com base em alguma situação/evento específico;



Esta funcionalidade permite o cadastro de grupos e o vínculo deles com usuários, um perfil, contratos e e-mails para notificação.

Esta funcionalidade disponibiliza ações diversas, tais como, incluir, alterar e excluir um grupo.

## Antes de começar

Para cadastrar um grupo é necessário o cadastro prévio do perfil de acesso e do colaborador.

## Procedimento

1.  Acessar a funcionalidade através da navegação no menu principal Acesso e Permissão > Grupo;

2.  Clicar em "Novo";

3.  Preencher os campos disponibilizados;

    - **Informações básicas**

    |Campo|Descrição|
    |-|-|
    |Nome *	|[Nome do Grupo]|
    |Sigla *	|[NG]|
    |ID Grupo|[01] - Gerado automaticamente|
    |Líder|[Nome do Líder] - Usado para identificar o gestor do grupo|
    |Perfil de Acesso *	|[Perfil] - Perfil de acesso herdado|
    |Grupo de Service Desk|[Sim/Não] - Se o grupo faz atendimento (=SIM), caso contrário o grupo não aparecerá na lista de grupos para direcionamento/delegação de tickets|
    |Solicitante do Chat|[Sim/não] - Se os integrantes do grupo podem abrir tickets via chat|
    |Comitê Consultivo de Mudanças|[Sim/Não] - Se o grupo faz parte de um CCM (Gerência de Mudança)|
    |Suspensão/Reativação |Parâmetro para permitir a suspensão/reativação de tickets independentemente das permissões no fluxo de trabalho (reativar/suspender)|
    |Notificações de e-mail Obrigatórias (Abertura, Andamento e Encerramento)|Caso habilitado, torna o envio de e-mail - oriundo das diversas ações dos fluxos - obrigatório (não configurável pelo atendente). Ao deixar desabilitado, o atendente poderá configurar as opções de envio de e-mail.|
    |Descrição |Detalhes para ajudar na identificação do grupo|

    - **Contratos:** Acordos que o grupo terá acesso (para registrar um serviço, realizar um atendimento etc.).

    - **Permissões nos Fluxos de trabalho**

    |Ação```*```| Descrição|
	  |-|-|
	  |Criar|Permissão para registrar um ticket/atividade|
	  |Executar|Permissão para executar um ticket/atividade|
    |Delegar|Permissão para delegar um ticket/atividade|
	  |Suspender|Permissão para suspender um ticket/atividade|
    |Reativar|Permissão para reativar um ticket/atividade|
    |Alterar SLA|Permissão para alterar a SLA de um ticket/atividade|
	  |Reabrir|Permissão para reabrir um ticket/atividade|
    |Cancelar|Permissão para cancelar um ticket/atividade|
    |Reclassificar|Permissão para reclassificar um ticket/atividade|

    ```*```Selecionar apenas as permissões específicas para o contexto de atuação.

    - **Colaboradores (usuários do sistema):** membros do grupo.
    - **E-mail:** endereços de e-mail que receberão as notificações originadas em um fluxo de trabalho. Esta opção é bastante útil quando é necessário tornar uma pessoa "informada" das interações do grupo sem que ela participe no mesmo.

4.  Definir as configurações que sejam necessárias;
5.  Clicar em "Gravar".


!!! Abstract "REGRA"

    A exclusão de grupo depende de não existir portfólios, colaboradores e
    contratos vinculados ao mesmo.


Relacionado
-----------

[Cadastrar um colaborador](/pt-br/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Criar perfil de acesso](/pt-br/citsmart-7/initial-settings/access-settings/profile/create-profile-access.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 – Anna Martins
