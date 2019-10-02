title: Create ticket via Twitter
Description: CITSmart, in order to expand the service modalities, allows users to register their tickets directly through the social network interface Twitter.

# Create ticket via Twitter
CITSmart, in order to expand the service modalities, allows users to register their tickets directly through the social network interface Twitter.

Before getting started
----------------------

It is necessary to have the integration functionality with Twitter configured in the CITSmart instance besides of having the machine learning functionality (Python environment). Moreover, it is necessary to define the service that will attend to this type of service, as well as contracts and permissions in workflows. 

Procedure 
-------------

1.  Follow CITSmart on Twitter;

2.  Click on "Messages" on Twitter;

3.  Create the ticket with the request you want;

4.  After the ticket is created, the system will answer with a standard feedback including the request number;

    !!! Abstract "NOTE"
        
        Once created the ticket via Twitter, the executor of it will have access to the request through the 
        functionality "Tickets" in the system, following the regular procedure of tickets execution. 
        
5.  When closing the ticket attendance, the Solution-Response will be sent to the user's Twitter as a direct message.

!!! Abstract "IMPORTANT"

    The opening and attendance of tickets via Twitter is only possible if the system follows a Neuro workflow 
    specifically created in order to meet this type of request. Besides, to execute this flow, it is necessary 
    a business process scheduled by Cron expression.  

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/29/2019 – Larissa Lourenço
