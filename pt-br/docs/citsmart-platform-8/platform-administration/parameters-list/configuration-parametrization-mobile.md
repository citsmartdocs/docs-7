title: Configurar parametrização - mobile
Description: Possui a finalidade de configuração, customização para adequação de cenário no que tange a utilização dos aplicativos mobile (como por exemplo, o CITSmart GO)
# Configurar parametrização - mobile

A parametrização de "Mobile" possui a finalidade de configuração, customização
para adequação de cenário no que tange a utilização dos aplicativos mobile (como
por exemplo, o CITSmart GO).

Procedimento
----------------

1.  Acessar a funcionalidade através da navegação no menu principal
    Parametrização \> Mobile;

2.  Definir os valores dos parâmetros (atributos);

3.  Clicar no botão "Gravar" para efetuar a operação;

4.  A lista abaixo representa os parâmetros do "Mobile" e a finalidade de cada
    um deles:

| #   | Nome                                                                                                                     | Valores possíveis   | Finalidade                                                                                                                                                                                                                                                                                             | Orientações complementares |
|-----|--------------------------------------------------------------------------------------------------------------------------|---------------------|--------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|----------------------------|
| 255 | Raio de Ação/Visualização do atendente no Mobile - (Default: 30)                                                         |                     | Definir o raio de ação de um atendente, utilizado no APP mobile. Definir o raio máximo de atendimento de solicitações que estejam com situação “Não Direcionada”.                                                                                                                                      | Não se aplica              |
| 256 | Intervalo (em minutos) de tempo para reporte de posição do Atendente - (Default: 10)                                     |                     | Definir o intervalo que o aplicativo Mobile deve reportar ao servidor o posicionamento geográfico do atendente.                                                                                                                                                                                        | Não se aplica              |
| 257 | Tamanho de página para retorno nos serviços REST paginados (Default: 10)                                                 |                     | Definir a quantidade de registros retornado em serviços de listagem consumidos pelo Mobile.                                                                                                                                                                                                            | Não se aplica              |
| 258 | Intervalo máximo de dias para consulta (Default: 30)                                                                     |                     | Definir restrição de intervalo máximo de consulta nas telas, inicialmente utilizadas na gestão da força de atendimento.                                                                                                                                                                                | Não se aplica              |
| 267 | Tamanho de página para retorno nos serviços REST V1 mobile (Default: 200)                                                |                     | Definir o tamanho da página para retorno nos serviços REST.                                                                                                                                                                                                                                            | Não se aplica              |
| 272 | Determina se serão notificados somente solicitações sem responsável no CITSmart Mobile. Valores: "S" ou "N" Default: "N" | S ou N (Default: N) | Definir quais solicitações poderão ser notificadas ao usuário. Caso o valor do parâmetro seja “S”, serão apresentadas somente as notificações de solicitações sem responsável atual pelo atendimento. Caso o valor do parâmetro seja “N”, serão apresentadas as notificações de todas as solicitações. | Não se aplica              |
| 284 | ID do contrato padrão para a criação de novos incidentes/requisições no CITSmart Mobile.                                 |                     | Informar o número de identificação (ID) do contrato para realizar a abertura de solicitações de serviço via mobile.                                                                                                                                                                                    | Não se aplica              |
| 285 | ID do serviço padrão para solicitações de serviços e incidentes criados no CITSmart Mobile.                              |                     | Informar o número de identificação (ID) do serviço que será padrão para registro de solicitações de serviços via mobile.                                                                                                                                                                               | Não se aplica              |
| 286 | ID de origem padrão para as solicitações de serviço e incidentes criados no CITSmart Mobile.                             |                     | Informar o número de identificação (ID) da origem padrão para abertura de solicitação de serviço via mobile.                                                                                                                                                                                           | Não se aplica              |
| 350 | Habilita o envio de notificações para celulares                                                                          | S ou N (Default: N) | Permite controlar se as notificações do sistema serão enviadas para dispositivos móveis (gerais).                                                                                                                                                                                                      | Não se aplica              |
| 352 | Habilita o envio de notificações para celulares durante a criação de solicitações                                        | S ou N (Default: N) | Permite controlar se as notificações do sistema serão enviadas para dispositivos móveis (gerais).                                                                                                                                                                                                      | Não se aplica              |
| 353 | Habilita o envio de notificações para celulares durante a atualização de solicitações informando atendimentos próximos   | S ou N (Default: N) | Permite controlar se as notificações do sistema serão enviadas para dispositivos móveis (gerais).                                                                                                                                                                                                      | Não se aplica              |

Tabela 1 - Lista de parâmetros


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 – Anna Martins
