title: Configurar campos de obrigatoriedade
Description: É facultado ao administrador a escolha de quais campos o usuário será compelido a preencher
# Configurar campos de obrigatoriedade
Através da configuração dos campos de obrigatoriedade é facultado ao administrador a escolha de quais campos o usuário será compelido a preencher ao contactar os atendentes. A finalidadade desta habilidade é impor ao solicitante a satisfazer as informações imprescindíveis a resolução de sua solicitação.  

Procedimento
------------

1.  Acessar a funcionalidade através da navegação no menu principal Sistema \>
    Configurações \> Páginas - Configuração de campos;

2.  Serão apresentadas as páginas que comportam a escolha de campos obrigatórios.
    São duas: Gerenciamento de Problema e Gerenciamento de
    Incidentes/Requisições.

### Configurar os campos da funcionalidade “Problema”

*Utilizando a opção de utlizar a obrigatoriedade do campo é possível exigir que
determinadas informações sejam registradas ao criar o problema.*

1.  Após acessar a página inicial da funcionalidade, escolher a opção “Problema”
    e clicar no botão “Editar”;

2.  Marcar os campos que deseja tornar obrigatório. São eles:

    |     **Nome do campo**    | **Obrigatório** |
    |:------------------------:|:--------------:|
    |         Catálago         |      :ballot_box_with_check:                  |
    |   Categoria de Serviço   |       :ballot_box_with_check:                 |
    |          Serviço         |       :ballot_box_with_check:                 |
    |         Telefone         |          :ballot_box_with_check:              |
    |           Ramal          |        :ballot_box_with_check:                |
    |     Localidade Física    |      :ballot_box_with_check:                  |
    |        Observação        |           :ballot_box_with_check:             |
    |      Grupo executor      |        :ballot_box_with_check:                |
    | Solucionar/Contornar até |    :ballot_box_with_check:                    |

3.  Clicar no botão “Gravar”.

### Configurar os campos da funcionalidade “Gerenciamento de Ticket"

*Utilizando a opção de utlizar a obrigatoriedade do campo é possível exigir que
determinadas informações sejam registradas ao criar o incidente/requisição.*

1.  Após acessar a página inicial da funcionalidade, escolher a opção
    “Gerenciamento de Incidentes” e clicar no botão “Editar”;

2.  Marcar os campos que deseja tornar obrigatório. São eles:

    | **Nome do campo** | **Obrigatório** |
    |:-----------------:|:--------------:|
    |     Telefone      |       :ballot_box_with_check:                 |
    |       E-mail      |          :ballot_box_with_check:              |
    |      Unidade      |           :ballot_box_with_check:             |
    | Localidade Física |       :ballot_box_with_check:                 |
    | Origem de contato |     :ballot_box_with_check:                   |

    !!! Abstract "ATENÇÃO"

        Os parâmetros 65 (que identifica o ID de origem do chamado padrão da
        solicitação de serviço) e 105 (identifica o ID de origem que será setado
        como padrão ao criar um novo incidente) setam uma origem de contato
        automaticamente quando o usuário cadastrar um ticket. Assim sendo, caso o
        campo “Origem do contato” na tela de ticket *não* for obrigatório, porém,
        existir um apontamento nos parâmetros anteriormente citados, o campo virá
        preenchido automaticamente.  
        
3.  Clicar no botão “Gravar”.

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/18/2019 – Anna Martins
