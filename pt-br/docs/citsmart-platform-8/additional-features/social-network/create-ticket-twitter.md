title: Criar ticket pelo Twitter
Description: O CITSmart, com intuito de ampliar as modalidades de atendimento, possibilita que os usuários possam registrar seus tickets diretamente pela interface da rede social Twitter.

# Criar ticket pelo Twitter
O CITSmart, com intuito de ampliar as modalidades de atendimento, possibilita que os usuários possam registrar seus tickets diretamente pela interface da rede social Twitter.

Antes de começar
----------------

É necessário ter a funcionalidade de integração com o Twitter configurada na instância CITSmart e ter a funcionalidade de machine learning (ambiente com Python). Além disso, é preciso definir o serviço que atenderá à esta modalidade de atendimento, bem como contratos e permissões em fluxos de trabalho. 

Procedimento 
-------------

1.  É necessário seguir a página CITSmart no Twitter;  

2.  Clicar no ícone “Mensagem” nesta página;

3.  Elaborar o ticket com a solicitação desejada;

4.  Logo após de criado o ticket, o sistema responderá com um feedback padrão incluindo o número da solicitação;

    !!! Abstract "ATENÇÃO"
        
        Criado o ticket pelo Twitter, o executor dele terá acesso a solicitação por meio da funcionalidade “Tickets” 
        no sistema, seguindo o procedimento regular de execução dos tickets. 
        
5.  Encerrado o atendimento do ticket, sua Solução-Resposta será publicada no twitter do usuário, como mensagem direta.

!!! Abstract "IMPORTANTE"

    A abertura e atendimento de tickets pelo Twitter só é possível se o sistema seguir um formulário (workflow) 
    Neuro criado especificamente com o intuito de atender este tipo de solicitação e este fluxo para ser executado,
    necessitará de um processo de negócio agendado por expressão Cron.  

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/29/2019 – Larissa Lourenço
