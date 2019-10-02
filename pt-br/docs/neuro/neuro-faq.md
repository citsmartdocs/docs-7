Title: FAQ (Neuro)
Description: CITSmart - FAQ

# FAQ (Neuro)

!!! Question "Qual a diferença entre criar um formulário através do menu Formulário e através do menu Objeto de negócio?"

    A criação através do menu de Formulário ocorre de forma 100% manual. Através do menu de objeto de negócio, é possível gerar o formulário a partir do modelo do banco de dados. O formulário gerado poderá ser editado no menu de cadastro de formulário.

	Como eu crio um menu para acessar o meu processo de negócio?

	A criação do menu para processo de negócio é feita no próprio cadastro de processo de negócio, definindo o campo "Menu associado".

	É necessário que esteja previamente cadastrado um menu com dois níveis para que ele possa ser vinculado a este processo de negócio.

	Também é necessário que, após salvo o processo de negócio com menu associado, seja atribuído permissão para o item de menu novo. A atribuição de permissão pode ser realizada através da tela de Menu ou da tela de Perfil de Acesso.

!!! Question "Como eu crio relacionamentos "muitos para muitos" no objeto de negócio?"

	Para criar um relacionamento "Muitos para muitos", é necessário criar um objeto de negócio terceiro para relacionar os dois objetos de negócio desejados.

	Ex: Vamos criar um relacionamento "muitos para muitos" entre dois objetos, A e B. Para isso, iremos necessitar de um objeto C que irá relacionar os dois.

	O objeto A terá um relacionamento "um para muitos" com o objeto C, e o objeto B também terá um relacionamento "um para muitos" com o objeto C.

	Dentro de nosso objeto C deve de ter dois relacionamentos, um deles "muitos para um" com o objeto A e o outro "muitos para um" com o objeto B.

	Assim, pode-se relacionar um dado do objeto A a vários dados do objeto B, e um dado do objeto B a vários dados do objeto A, através do objeto de negócio C, tendo efetivamente um relacionamento "muitos para muitos"

!!! Question "Todo workflow precisa ter um processo de negócio relacionado?"

	Nem todo workflow precisa ter um processo de negócio relacionado. Pode-se dizer que todo workflow principal precisa de um processo de negócio, porém os subprocessos não necessitam de outros processos de negócio para eles.   
	
	Além disso, essa regra se aplica apenas a fluxos de integração de processos, visto que os fluxos de integração de serviço não precisam de processo de negócio relacionado.

!!! Question "Existe alguma alternativa para que eu acesse as minhas tarefas do workflow abertas em um menu customizado, ou seja, fora do Gerenciamento de tarefas?"

	É possível fazer sua própria listagem de tarefas para acessar as tarefas do workflow. Para um tutorial completo, vide a documentação técnica.  

!!! Question "É possível criar componentes customizados que possam ser utilizados na criação de formulários?"

	É possível criar seus próprios componentes para serem utilizados no formulário. Para um tutorial completo, vide a documentação técnica.

!!! Question "Por onde devo começar a construção de uma aplicação utilizando o Neuro?"

	Recomenda-se que o primeiro passo a ser executado no Neuro seja o cadastro da aplicação ou o cadastro de uma conexão de banco de dados, de acordo com a necessidade da aplicação.  

!!! Question "Como funciona a injeção de dependências próprias dentro de um formulário no Neuro? Quais passos devem ser executados?"

	Para injetar uma dependência própria, é necessário cadastrá-la antes. As dependências que podem ser injetadas dentro de um formulário Neuro são somente do tipo CSS e Javascript.

	Criar um cadastro novo de acordo com o tipo da sua dependência através do menu "Neuro > Recursos" e fazer o upload da dependência.

	Para importá-la no formulário, selecionar a aba do tipo da página que deseja importar e escolher a aba "Dependências". 

	Clicar no ícone de "+ Adicionar" para incluir uma dependência nova, no campo "Nome" digitar o nome cadastrado do recurso da sua dependência e selecionar a opção correspondente. Para mais informações à respeito de dependências de formulário, vide a documentação técnica.

!!! Question "Como defino as ações que devem estar disponíveis em cada tarefa do workflow?"

	As ações são cadastradas nas abas principais do cadastro do fluxo. Para associar uma ação a uma tarefa específica, ir para o desenho do workflow, abra as propriedades daquele elemento, selecionar as ações desejadas e salvar as alterações.

!!! Question "Como deleto um elemento do workflow?"

	Para deletar um elemento do workflow, selecionar o elemento que deseja deletar e pressionar Ctrl + Del.

!!! Question "O que faço quando ocorrer o erro "Processo de negócio não informado"?"

	Este erro ocorre porque o processo de negócio não está referenciado no controller do formulário que inicia o processo de negócio. Para corrigir este problema, acessar o formulário referente ao processo de negócio, e inserir o seguinte comando no controller da "Página p/ processo": $scope.businessProcessName = 'nome_do_processo_de_negocio';

!!! Question "Quando eu cadastro um subprocesso, as informações do processo principal são herdadas pelo subprocesso?"

	Não. Ao incluir um novo subprocesso, seja do tipo ESI ou do tipo BPE em um workflow principal, deverá, informar na aba "Atributos", o nome exato do subprocesso que deverá ser criado manualmente no cadastro do workflow.

	Todas as informações, como ações e estados do fluxo principal deverão ser replicados no cadastro do subprocesso.

	Resumindo em passos, recomenda-se seguir a seguinte ordem:

	1. Cadastrar o fluxo principal;
	2. Cadastrar o subprocesso;
	3. Incluir o elemento de subprocesso, referenciando o subprocesso já criado.

!!! Question "Qual a diferença entre um fluxo de integração de processos e um fluxo de integração de serviços?"

	Os fluxos de integração de processos são workflows que possuem tarefas executadas por usuários, podendo também possuir tarefas automáticas executadas pelo sistema.

	Os fluxos de integração de serviços, como o próprio nome diz, envolvem workflows executados com base em serviços de sistema, como integrações e conversões, por exemplo.

	Nada impede que um fluxo de integração de processos utilize um subprocesso de integração de serviços, por exemplo.
	
