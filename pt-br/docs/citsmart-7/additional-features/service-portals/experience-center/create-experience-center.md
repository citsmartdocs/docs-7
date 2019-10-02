Title: Criar Centro de experiência
Description: Esta funcionalidade disponibiliza ações diversas, tais como, incluir, alterar e excluir o Centro de Experiência customizado.

# Criar Centro de Experiência

A criação é o processo de concepção e disponibilização de Centros de Experiência (CE's) no CITSmart. Neste documento, são apresentados os recursos de interface que viabilizam o registro, alteração, exclusão, importação e exportação de CE’s.

## Antes de começar

- [X] Para criar um centro de experiência é necessário possuir permissão no perfil de acesso.

!!! abstract "Nota"

    Alguns widgets dependem de informações cadastradas em outras funcionalidades, por exemplo, conhecimentos, pesquisas (surveys), serviços, notificações e entre outros. Neste sentido, é necessário estruturar estas informações para eventual utilização no CE.

## Procedimento

1. Para acessar a funcionalidade do Centro de Experiência, acesse o menu **Centro de Experiência** > Configuração de Centro de Experiência > **Novo**.

### Informações

2. Na guia Informações, preencher os campos disponibilizados;

![information Experience Center CITSmart][1]

**1: Alterar** – ícone do Centro de Experiência;

**2: Título** – que será apresentado para o usuário do Centro de
Experiência;

**3: Situação** – que o Centro de Experiência se encontra (“Ativo” ou “Inativo”);

**4: Tipo** - é possível visualizar as opções *Principal* que mostra os Centros de Experiências criados para serem principais, e *Vínculo* que mostra os que foram criados para serem vinculados à algum CE principal;

**5: Descrição** – texto que seguirá com o título para apresentação do Centro de Experiência para o usuário.

### Permissões

3. Na guia Permissões, definir os grupos que poderão visualizar o Centro de Experiência;

![Permission Experience Center CITSmart][2]

### Construção

4. Na guia Construção, é possível personalizar visualmente o Centro de Experiência, além de poder criar seções e adicionar Widgets, links
e vincular outros Centros de Experiência:

#### Personalização Visual

5. Utilizando essas ferramentas você pode customizar a visão do Centro de Experiência

- **Alterar logo** – Permite alterar a logo do CE. Tamanho recomendado:

- **Alterar cabeçalho** – Permite alterar a imagem do cabeçalho do CE. Tamanho recomendado:

- **Reiniciar estrutura** – Permite deixar a toda estrutura como se fosse o primeiro acesso, removendo todas alterações;

- **Estilo da grid** – Permite alterar a forma de visualizar o Centro de experiência,

    - Largura fixa: Mantém o CE fixo no centro da tela;

    - Largura completa: Deixa o CE completamente distribuído no tamanho
do seu navegador;

- **Tamanho da logo** – Permite aumentar o tamanho da logo em até 100% o seu tamanho original.

- **Cor do tema** – Permite alterar a cor do menu retrátil (utilizando cores em código, Ex: #777)

- **Ícone do menu** – Permite alterar a cor das seções, dos links e dos ícones do menu (utilizando cores em código, Ex: #777)

!!! warning "ATENÇÃO"

    O botão “Reiniciar estrutura” é irreversível após salvar a alteração, caso não tenha *salvado* basta apertar o botão voltar que nada será alterado.

#### Área de Desenho

Na Área de desenho você pode construir o conteúdo que será publicado no Centro de Experiência.

6. Defina tipos de navegação (com menu ou sem menu);

7. Criar seções para a árvore de navegação (apenas para navegação com menus);

8. Adicionar item de menu, no final da seção clicar em "+";

9. Configurar o conteúdo do menu, clicar no ícone de chave;

10. Selecionar tipo de conteúdo (Widget, link ou Centro de Experiência);


**Tipo: Widget**

1. Selecionar o tamanho para área de conteúdo, clicar em "+" e escolher uma opção;

!!! example "EXEMPLO"
    100%, 50% x 50%, 33,3% x 33,3% x 33,3%, 33,3% x 65,6%, 65,6% x 33,3% e 25% x 25% x 25% x 25%.

2. Selecione o Widget, clicar em "=+" e escolher uma opção;

3. Clicar em gravar para salvar as alterações.

- Após selecionar o layout desejado, é possível escolher funções do CITSmart em forma de Widgets (Ver tabela de Widgets);

!!! note "NOTA"
    - Deseja definir está página como inicial ao abrir o centro de experiência pela primeira vez? - tem a função de transformar esse menu na página principal do seu Centro de Experiência.
    - Herdar os grupos do Centro de Experiência - permite selecionar quais os grupos que terão permissão a esse menu, os grupos que estão disponíveis para gerenciamento são os grupos que tiveram permissão na guia “Permissões”;

**Tipo: Link**

1. Ao selecionar o item link insira uma URL para direcionar o usuário quando o mesmo clicar no item de menu;  

2. Clicar em gravar para salvar as alterações.

**Tipo: Centro de Experiência**

1. Permite que seja vinculado outro Centro de Experiência (Tipo: Vínculo) ao principal. Clique no campo pesquisa e serão listados os CE´s cadastrados, selecione um. Também é possível digitar o nome para localizá-lo.

2. Clicar em gravar para salvar as alterações.


#### Posicionamento dos Elementos e Widgets

**Cabeçalho fixo**

![header Experience Center CITSmart][3]

 **1: Menu** – com ele é possível acessar outros Centros de experiência a qual você possui permissão;

**2: Logo** – selecionada pelo usuário para melhor personalização do CE;

**3: Barra de pesquisa** - realizar uma pesquisa universal que retornará Conhecimentos e Atividades que o usuário pode selecionar;

**4: Opções da conta** – permite alterar o idioma, editar o perfil, realizar o logout e acessar o sistema

**Centro de Experiência com navegação**

Esta estrutura permite a criação de um Centro de Experiência com uma árvore menu de navegação à esquerda.

**Centro de Experiência sem navegação**

Esta estrutura permite a criação de um centro de experiência utilizando somente widgets.

**Widgets Disponíveis**

|**Nome**|**Tipo**|**Objetivo**|
|:----------------------:|:-------------:|:--------------------------------:|
|Notícias| Geral | Exibir conhecimentos do tipo “Notícia”. |
|Notificação| Geral | Exibir as notificações do Sistema. |
|Pesquisas| Geral |Permite visualizar campanhas ativas|
|Youtube| Geral |Permite incorporar vídeos do Youtube|
|Imagem| Geral | Inserir imagem |
|Slide Show| Geral | Exibir Slide show do tipo carrossel. |
|Divisor| Geral | Inserir linha horizontal na página. |
|Espaçador| Geral | Inserir espaço entre um widget e outro. |
|Texto| Geral | Inserir Texto com diversas formatações. |
|Lista| Geral | Inserir lista de links. |
|Menu| Geral | Permite visualizar menu do CITSmart. |
||||
|Centro de conhecimento| Conhecimento| Gera um botão que direciona para o Centro de Conhecimento|
|Conhecimento| Conhecimento| Permite inserir documentos já existentes na base de conhecimento|
|Favoritos| Conhecimento| Permite listar todos os documentos classificados como favorito no Guia do usuário|
|Indicados| Conhecimento| Permite listar todos os documentos indicados no Guia do usuário|
|Curtidos| Conhecimento| Permite listar todos os documentos curtidos no Guia do usuário|
||||
|Meus serviços | Solicitações| Permite abrir um ticket pelo Centro de Experiência|
|Meus tickets | Solicitações| Permite visualizar a listagem de tickets abertos pelo usuário logado|
||||
|Simple | Simple-Gestão Ágil | Permite visualizar worksplaces da funcionalidade Simple |
||||
|Smart Chat | Comunicação | Permite inserir logo para este submenu |
|Ligue | Comunicação | Permite inserir logo para este submenu |
||||
|Meus Worksplaces | Decisão Smart | Permite buscar relatórios que se encontram dentro do Decisões Smart |
||||
| Centro de Experiência | Centro de Experiência |Permite inserir outro centro de experiência|

## O que fazer a seguir

- Na área superior, clique em "Prévia" para visualizar o Centro de Experência criado. Após finalizar o CE, publique-o para que sua organização possa usufruir de todos os recursos.


## Relacionado

[Criar conhecimento](/pt-br/citsmart-7/processes/knowledge/use/create knowledge.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RPwkqhQwYU_EpvvGd29tSTA)

About
Product/Version: CTISmart | 8.0.2.0 Updated: 25/09/2019 – Brunno Roosevelt Sturm Dias

[1]:images/creat-experience-center.png
[2]:images/permission-experiece-center.png
[3]:images/header-experience-center.png
