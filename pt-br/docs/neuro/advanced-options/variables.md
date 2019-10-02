Title: Variáveis
Description: Nesta aba são configuradas as variáveis que serão utilizadas no fluxo desenhado. As variáveis são objetos capazes de reter e representar um valor ou expressão. As variáveis são associadas a "nomes", chamados identificadores, durante o tempo de execução do fluxo.    
# Variáveis 

Nesta aba são configuradas as variáveis que serão utilizadas no fluxo desenhado. As variáveis são objetos capazes de reter e representar um valor ou expressão. As variáveis são associadas a "nomes", chamados identificadores, durante o tempo de execução do fluxo.    

## Como acessar  

1. Acesse a funcionalidade através da navegação no menu Neuro > Gerenciamento > Fluxo de Integração.  

## Pré-condições  

1. Não se aplica. 

## Filtros  

1. O seguinte filtro possibilita ao usuário restringir a participação de itens na listagem padrão da funcionalidade, facilitando a localização dos itens desejados:    

    * Palavra chave    

![Screenshot](images/Variables-fig01.png) 

Figura 1 - Tela de pesquisa  

## Listagem de itens 

1. Os seguintes campos cadastrais estão disponíveis ao usuário para facilitar a identificação dos itens desejados na listagem padrão da funcionalidade: Nome, Descrição, Aplicação do fluxo, Versão e Data de bloqueio.  

![Screenshot](images/Variables-fig02.png)

Figura 2 - Tela de listagem   

## Preenchimento dos campos cadastrais - variáveis     

1. Para adicionar uma variável, selecione a sua aba referente e clique em "Adicionar".    
2. Será apresentada a seguinte tela:    

    ![Screenshot](images/Variables-fig03.png)
    
    Figura 3- Tela de cadastro/edição do workflow, aba de Variáveis  

3. Preencha os campos:    

    * Nome da variável;  
    * Descrição;  
    * Se será armazenada no banco de dados;  
	    * Esta opção irá armazenar o valor da variável internamente, dentro do modelo de dados do Neuro, assim ela irá reter o valor             durante a execução das tarefas   
    * Se é uma variável de retorno;   
	    * Esta opção irá fazer que o Neuro retorne a variável no final da execução do fluxo.    
    * Se é uma lista de valores;  
    * Se é uma variável de entrada na interface do fluxo;  
	    * Esta opção permite que a variável seja “injetada” no processo de negócio vinculado a este fluxo.    
    * Se é uma variável de saída na interface do fluxo;   
	    * Esta opção faz que a variável tenha o valor preenchida quando o processo de negócio vinculado à estre fluxo for executado. 
    * O tipo da variável;  
	    * Se for um objeto Java, informe a classe Java correspondente;   
	    * Se for um objeto de negócio, qual sua aplicação respectiva e qual o nome cadastrado do objeto de negócio;   
    * O valor inicial da variável, se constante ou script.    
	    * Se o valor for uma constante, este nunca será alterado durante a execução do fluxo, independente das operações realizadas               pelo usuário.   

4. Para editar uma variável, selecione a variável desejada, clique em "Editar", faça as alterações necessárias e clique em "Atualizar" para concluir a edição.   

    !!! Abstract "ATENÇÃO"  

        Para salvar suas alterações efetivamente, clique em "Salvar" na barra superior.  

5. Para remover uma variável do fluxo, selecione a variável desejada, clique em "Remover" e confirme a exclusão.  
	

!!! tip "About"
    <b>Updated:</b>17/01/2019 - João Pelles Junior
