Title: Disponibilizar Anuva na interface CITSmart
# Disponibilizar Anuva na interface CITSmart

A Anuva já se integra nativamente ao CITSmart, então é muito fácil adicioná-la ao seu ambiente.

## Procedimento

1. Com acesso de Administrador, acesse a tela de parâmetros do CITSmart
2. Altere o valor do parâmetro “402 Anuva Assistant - External URL” para http://[nome-servidor].anuvaassistant.com
3. Altere o valor do parâmetro “441 Anuva Assistant - Conversation API” para http://[nome-servidor][sigla-idioma].anuvaassistant.com/webhooks/rest/webhook e clique em “Salvar”
4. Altere o valor do parâmetro “442 Anuva Assistant - Parameters API” para http://[nome-servidor][sigla-idioma].anuvaassistant.com/conversations/
5. Configurar o parâmetro 453 "Mensagem default de Fallback da Anuva Assistant", com uma mensagem que a Anuva irá responder sempre que não possuir resposta para aquela pergunta
6. Habilitar parâmetro 423 "Habilitar Anuva Assistant na área interna do sistema", parâmetro que permite que os analistas tenham iteração com a ANUVA
7. Habilitar parâmetro 450 "Habilitar Anuva Assistant na área externa", parâmetro que permite que os usuários finais tenham iteração com ANUVA.    


!!! note "NOTA"

    Para a sigla dos idiomas, use EN (Inglês) e PT (Português-Brasil).
    Se os parâmetros mencionados não estiverem disponíveis, atualizar a versão do CITSmart.


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/07/2019 - Anna Martins
