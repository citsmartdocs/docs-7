Title: Como interagir Anuva com outras interfaces
# Como interagir Anuva com outras interfaces

Para que a Anuva interaja com outros sistemas, é necessário adicionar no diálogo, uma habilidade personalizada.

A consulta é feita através de uma API Rest, a qual precisa ser disponibilizada pelo sistema detentor das informações 
de interesse do usuário. Ex: buscar informações sobre o status de um ticket, criação de tickets, geração de boletos no sistema.

Procedimento
-----------

1. Acessar o menu principal “Diálogos” e clicar em “Novo”;

2. Preencher as informações da seção **Interesse**;

3. Na seção **Habilidade**, selecionar o tipo *Personalizado*;

4. Preencher as informações da Seção API, incluindo o exemplo do corpo e da resposta;

5. Caso seja necessário, informe o cabeçalho;

6. Na seção Respostas, são duas opções de ação da assistente:

    a) Respostas em memória: o valor retornado pela API é associado ao atributo selecionado;
 
    b) Respostas em texto: retorna uma mensagem em texto para o usuário.
  
  
!!! Abstract "NOTA"

    A integração precisa ser homologada pela CITSmart, sendo assim que após configurar
    esta habilidade é preciso abrir um ticket para que se faça a homologação da integração.
    
    
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/07/2019 - Anna Martins
   
