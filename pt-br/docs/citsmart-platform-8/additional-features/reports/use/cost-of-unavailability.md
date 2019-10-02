title: Relatório do custo de indisponibilidade do serviço
Description: Verificar o relatório que demonstra o custo por hora de indisponibilidade de um serviço.
# Relatório do custo de indisponibilidade do serviço

Este documento tem por objetivo verificar o relatório que demonstra o custo
por hora de indisponibilidade de um serviço, onde:

 +   Tempo Disponível: tempo (dentro da jornada de trabalho) que os incidentes do
    serviço ficaram disponíveis no período;

 +   Tempo Indisponibilidade: tempo em horas (dentro da jornada de trabalho) que
    os incidentes do serviço ficaram indisponíveis no período;

 +   Número de quedas: quantidade de incidentes do serviço;

 +   MTBSI = Tempo disponivel / Nºde quedas;

 +   MTBF = (Tempo disponivel - Tempo Indisponibilidade) / Nº de Quedas;

 +   MTRS = Tempo Indisponibilidade / Nº de quedas.

Antes de começar
--------------------

No porfólio de serviços um serviço deverá ter o atributo **Incidente** com o
campo "Causa indisponibilidade" setado igual a "SIM".

No atributo **Contrato** do serviço escolhido, o incidente deverá está
vinculado, assim como definir o Custo de Indisponibilidade, o Acordo de
Disponibilidade e também vincular o Calendário.

O relatório disponibilizado via anexo deverá ser importado no Gerador de
Relatório Smart.

Procedimento
----------------

*Passo 1*

1.  Acessar Relatórios \> Relatórios Smart \> Gerador de Relatórios Smart;

2.  Clicar em no botão "Importar";

3.  Selecionar o arquivo disponibilizado (anexo) e clicar em "Abrir";

4.  Na página de listagem de relatórios, clicar no botão "Editar" do relatório
    importado;

5.  Selecionar a opção *N/A* no campo **Módulo(s) onde será exibido** e definir
    o(s) grupo(s);

6.  Clicar no botão "Gravar".

*Passo 2*

1.  Acessar o menu principal Processos \> Gerência de Portfólio e Catálogo \>
    Porfólio;

2.  Escolher o portfólio desejado e clicar em "Avançar";

3.  Escolher o serviço desejado e clicar em "Avançar";

4.  Clicar no atributo **Incidentes**, em seguida no botão "Novo Incidente" (o
    campo "Tipo de Demanda" deverá ser Incidente, assim como o campo "Causa
    Indisponibilidade" deverá ser "SIM");

5.  Clicar em "Gravar";

6.  Clicar no botão "Vincular Incidente" e vincular o incidente criado
    anteriormente.

*Passo 3*

1.  Clicar no atributo **Contratos** do serviço;

2.  Selecionar o contrato desejado e clicar em "Avançar";

3.  Clicar no atributo **Incidentes** do contrato e em seguida no botão
    "Vincular Incidente";

4.  Preencher os campos disponibilizados adicionando também o incidente criado
    anteriormente;

5.  Clicar em "Gravar";

6.  Clicar no atributo **Custo de Indisponibilidade**, definir o valor e clicar
    em "Gravar";

7.  Clicar no atributo **Acordo de Disponibilidade**, clicar no botão "Vincular
    Acordo de Disponibilidade e definir um SLA;

8.  Clicar no atributo **Calendário**, clicar no botão "Vincular Calendário" e
    definir um calendário.

O que fazer a seguir
--------------------

Acessar o painel gerencial no Smart Portal, adicionar o relatório importado
previamente, definir as datas e checar o relatório.

O relatório também poderá ser visualizado em Relatórios Smart.


Relacionado
-----------

[Cadastrar um serviço](/pt-br/citsmart-7/processes/portfolio-and-catalog/use/register-a-service.html)

[Configurar atributos do serviço](/pt-br/citsmart-7/processes/portfolio-and-catalog/use/configure-services-attributes.html)

[Configurar atributos do contrato do serviço](/pt-br/citsmart-7/processes/portfolio-and-catalog/use/service-contract-attributes.html)

[Criar portfólio](/pt-br/citsmart-7/processes/portfolio-and-catalog/use/create-the-portfolio.html)

[Acordo de nível de serviço](/pt-br/citsmart-7/processes/service-level/use/service-level-agreement.html)

[Personalizar o painel gerencial (Smart Decision)](/pt-br/citsmart-7/additional-features/reports/create/dashboard-customize-management-panel-smart-decision.html)

[Emitir relatório utilizando Smart Report](/pt-br/citsmart-7/additional-features/reports/create/smart-reports/configuration/create-smart-report.html)

[Construir e manter relatórios Smart - V.8.0](/pt-br/citsmart-7/additional-features/reports/create/smart-reports/configuration/build-maintain-smart-report.html)


Anexo
-----
[Download-Confiabilidade][1]

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 – Anna Martins

[1]:/pt-br/citsmart-7/additional-features/reports/use/images/confiabilidade.citreport
