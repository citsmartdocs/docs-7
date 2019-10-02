Description: Release Notes CITSmart Versão 7.0.0.0 de 01/03/2019

# Versão 7.0.0.0
_01/03/2019_

## Correções

### Gerenciamento de Ticket

As funcionalidades de Sub-Solicitação e Solicitação Relacionada sofreram uma reestruturação que proporciona maior conformidade à suas atribuições, o foco dessa correção foi aproximar a funcionalidade daquilo que realmente é a sua proposta.

Para mais informações, veja [Relacionar um Ticket][1] e [Cadastrar um sub-ticket][2]

### Webservices

A sincronização para criação de novas Atividades sofreu uma alteração em sua regra de negócio, isso porque não é possível criar uma atividade que não tenha vínculo com Serviço de Negócio e Portfólio. Portanto, o webservice designado para criação irá abrir um ticket com os parâmetros passados na configuração inicial do serviço.

A funcionalidade de criar um novo usuário, quando estiver habilitado a sincronização de dados permanece consistente.

### Fluxo

Tratativa para barrar edição de expressões nativas e expressões de mesmo nome.

## Novas Funcionalidades e Melhorias

### Acesso Rápido

O acesso rápido permite que o usuário encontre os principais processos por meio de ícones que auxiliam na fixação e visualização de forma eficiente.

**O usuário visualiza somente os ícones dos processos que o mesmo possui acesso com exceção dos ícones Simple, Portal do Conhecimento, Centro de Experiência e Guia de Usuário.**

### Configuração de notificação por e-mail de ticket delegado

Criamos a possibilidade de configuração de notificação por e-mail na funcionalidade de delegação do ticket
Para mais informações, veja [Notificação via e-mail de ticket delegado][3]

### Configuração de Notificação por e-mail de ticket reclassificado

Criamos a possibilidade de configuração de notificação por e-mail na funcionalidade de reclassificação do ticket
Para mais informações, veja [Notificação via e-mail de ticket reclassificado][4]

### Gerência de  Mudança

A versão 7.0.0.0 do CITSmart sofreu melhorias no processo de gerenciamento de mudanças, trazendo o mundo ágil para gerenciar as atividades que deverão ocorrer durante o escopo da mudança.

**Nota:** Essa funcionalidade substitui os parâmetros de fluxos padrões para utilização do processo de mudança, portanto, é necessária a alteração para essa configuração.


Para mais informações, veja [Gerência de Mudança][5]

### Gerência de Problema

Na versão 7.0.0.0 do CITSmart o processo de gerenciamento de problema permite adicionar atividades para auxiliar no gerenciamento das equipes durante o diagnóstico da causa raiz.

**Nota:** Essa funcionalidade substitui os parâmetros de fluxos padrões para utilização do processo de problema, portanto, é necessária a alteração para essa configuração.


Para mais informações, veja [Gerência de Problema][6]

### Configuração de uso para Gerência de  Liberação

O processo de liberação ganha mais força no planejamento, testes e homologação permitindo designação das atividades e gerenciamento à vista.

**Nota:** Essa funcionalidade substitui os parâmetros de fluxos padrões para utilização do processo de liberação, portanto, é necessária a alteração para essa configuração.


Para mais informações, veja [Gerência de Liberação][7]

### Revisão de Comentários

Na versão 7.0.0.0 o CITSmart permite avaliação e publicação dos comentários escritos sobre um conhecimento.

Para mais informações, veja [Revisão de Comentário][8]

### Acesso à base de conhecimento de usuários externo

Inovamos  a forma de acesso à base de conhecimento para usuários que não possuem login de acesso à ferramenta CITSmart.

Na versão 7.0.0.0 conhecimentos com permissão de visualização poderão ser acessados pela comunidade em geral, basta possuir o link de acesso.


Para mais informações, veja Configurar acesso externo ao [Portal de Conhecimento][9]

### Gerência de Item de Configuração

Aprimoramos a experiência do usuário trazendo em destaque um dashboard que apresenta a quantidade de itens de configuração, por grupo, tipo e aglutinados nos processos de Incidente, Mudança e Liberação, deixando à vista possíveis IC’s que passarão por alteração ou envolvidos em algum incidente.

Para mais informações, veja [Gerenciamento de Item de Configuração][10]

### Regra de Escalonamento

Simplificamos o uso das regras de escalonamento dos tickets, com poucos passos será possível implementar a regra que antes contava com inúmeras configurações.

**Nota**: Essa funcionalidade substitui o uso de diversos parâmetros de escalonamento, portanto, é necessária a alteração para o uso efetivo das regras de escalonamento.


Para mais informações, veja [Criar regra de escalonamento][11]

### Aprovação de Ticket

Na versão 7.0.0.0 do CITSmart incluímos a aprovação de tickets através de novo ícone direto na lista de atendimento, não será necessário abrir o ticket para realizar o atendimento, apresentamos as informações disponíveis e as opções configuradas para aceite ou recusa do chamado.

Essa funcionalidade está disponível no Mobile SM e no Portal de Serviços.

Para mais informações, veja [Aprovar um ticket][12]

### Atualização automática da lista de ticket

Permitimos que a função de atualização automática da lista de ticket seja habilitada para atualizar a lista automaticamente de tempos em tempos.

Para mais informações, veja [Atualização Automática da Lista de Ticket][13]

### Ocorrência

O aprimoramento do cadastro de ocorrência permite que o solicitante ou técnico seja notificado via e-mail. Além da permissão de incluir tempo de execução da atividade e manter o sigilo da informação cadastrada, para que somente os técnicos permitidos a vejam.

Para mais informações, veja [Cadastrar ocorrência em Ticket][14]

### Simple - Gestão Ágil e a vista

O Simple foi criado com o intuito de trazer o conceito de gestão ágil à ferramenta.
De forma independente ou aglutinada em uma das soluções de Problema, Mudança e Liberação, o Simple permite reutilização de Sprints, compartilhamento de recursos, envio de atividades à outras Sprints e gestão à vista.

Para mais informações, veja [Simple][15]

### Área do cliente

Proporcionamos uma área específica para melhorar a experiência de uso. Nessa área será permitido a apresentação de serviços, informações, relatórios que mais se aproximam com o uso do dia a dia do cliente.

Para mais informações, veja [Centro de Experiência][16]

### Business Intelligence

A partir da versão 7.0.0.0 disponibilizamos alguns relatórios quantitativos dos principais processos contidos no CITSmart através de nossa nova plataforma BI.

Para mais informações, veja [Business Intelligence][17]

### Auditoria

Reformulamos a auditoria do sistema para aumentar a agilidade e confiabilidade do recurso de pesquisa de auditoria.

Para mais informações, veja [Auditoria do Sistema][18]

### Política de Segurança de Senha

Aprimoramos o quesito de segurança da informação, implantado formas de segurança de senhas para usuários internos.

Para mais informações, veja [Política de Segurança de Senha][19]

### Mobilidade

Entregamos um novo aplicativo que de forma robusta permitirá o atendimento a campo de técnicos que momentaneamente estão sem conexão à internet.

A experiência de mobilidade vai além com os recursos de assinatura e notas.

Para mais informações, veja [Manual de utilização do aplicativo CITSmart GO][20]

Ainda no contexto de mobilidade e não menos robusta, aprimoramos o aplicativo Mobile SM, que possui dentre outros usos a capacidade de assinatura, aprovação e notas.

Para mais informações, veja [Manual de utilização do aplicativo mobile CITSmart Experience][21]

### Neuro

A partir da versão 1.2.3.0 do Neuro é possível criar automaticamente um questionário do CITSmart a partir do cadastro de objeto de negócio do Neuro. A ideia dessa inovação é facilitar a extração de respostas de questionários do CITSmart e formar relatórios de forma simples com o auxílio do Smart Report.


### Fluxo

O pacote de fluxos entregues para os processos de Problema, Mudança e Liberação foram simplificados, os produtos foram remodelados para estarem aderentes às possibilidades que o fluxo oferece.

__Caso o cliente não queira utilizar os novos fluxos, a última versão 7.1.0 continuará funcionando perfeitamente.__


[1]:/pt-br/citsmart-7/processes/tickets/use/register-ticket-related.html
[2]:/pt-br/citsmart-7/processes/tickets/use/create-and-view-sub-request.html
[3]:/pt-br/citsmart-7/processes/tickets/configuration/notification-delegated-email-ticket.html
[4]:/pt-br/citsmart-7/processes/portfolio-and-catalog/configuration/send-email-reclassified-ticket.html
[5]:/pt-br/citsmart-7/processes/change/overview.html
[6]:/pt-br/citsmart-7/processes/problem/overview.html
[7]:/pt-br/citsmart-7/processes/release/overview.html
[8]:/pt-br/citsmart-7/processes/knowledge/use/review-reviews.html
[9]:/pt-br/citsmart-7/processes/knowledge/configuration/configure-external-access-knowledge-portal.html
[10]:/pt-br/citsmart-7/processes/configuration/overview.html
[11]:/pt-br/citsmart-7/processes/tickets/use/create-escalation-rule.html
[12]:/pt-br/citsmart-7/processes/tickets/use/approve-a-ticket.html
[13]:/pt-br/citsmart-7/processes/tickets/use/desktop-of-service-desk.html
[14]:/pt-br/citsmart-7/processes/tickets/use/register-ticket-occurrences.html
[15]:/pt-br/citsmart-7/additional-features/project-management/simple-agile-management/simple-agile-management.html
[16]:/pt-br/citsmart-7/processes/knowledge/use/create-experience-center.html
[17]:/pt-br/citsmart-7/additional-features/smart-analytics/use-bi-solution.html
[18]:/pt-br/citsmart-7/platform-administration/logs-and-auditing/system-audit.html
[19]:/pt-br/citsmart-7/platform-administration/security/implement-password-security-rules.html
[20]:/pt-br/citsmart-7/additional-features/mobile-and-field-service/apps/citsmart-field-service-manual.html
[21]:/pt-br/citsmart-7/additional-features/mobile-and-field-service/apps/citsmart-app.html
