title: Configurar parametrização - telefonia
Description: Permite definir se ativa a integração dos webservices com a telefonia.
# Configurar parametrização - telefonia

A parametrização da "Telefonia permite definir se ativa a integração dos
webservices com a telefonia, informar o número de identificação do serviço de
requisição, dentre outras ações possíveis afim de configurar o uso da telefonia
no CITSmart.

Procedimento
------------

1.  Acessar a funcionalidade através da navegação no menu principal
    Parametrização \> Telefonia;

2.  Definir os valores dos parâmetros (atributos);

3.  Clicar no botão "Gravar" para efetuar a operação;

4.  A lista abaixo representa os parâmetros da "Telefonia" e a finalidade de
    cada um deles:

|  #  |                                                                            Nome                                                                            |  Valores possíveis  |                                                                                            Finalidade                                                                                            |                                            Orientações complementares                                           |
|:---:|:----------------------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:---------------------------------------------------------------------------------------------------------------:|
| 281 |                                     Ativar WebService de integração com a Telefonia - Valores: "S" ou "N" Default: "N"                                     | S ou N (Default: N) |                                                                  Definir se ativa a integração dos webservices com a telefonia.                                                                  | Caso não seja definido o valor para o parâmetro, será definido pelo sistema automaticamente o valor: “N” (Não). |
| 282 | A telefonia deve lançar uma solicitação filha, referente à visualização de informações de uma solicitação já existente? - Valores: "S" ou "N" Default: "N" | S ou N (Default: N) |                Definir se ativa o lançamento automático de uma solicitação de serviço filha, da que está sendo visualizada ou executada, pelo webservice “visualizarSolicitacao”.                | Caso não seja definido o valor para o parâmetro, será definido pelo sistema automaticamente o valor: “N” (Não). |
| 283 |                                       ID do serviço de requisição de informações sobre uma solicitação já existente.                                       |        S ou N       | Informar o número de identificação (ID) do serviço de requisição, o qual será utilizado para lançar a solicitação filha referente à visualização de informações de uma solicitação já existente. |                                                  Não se aplica                                                  |

Tabela 1 - Lista de parâmetros


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 – Anna Martins
