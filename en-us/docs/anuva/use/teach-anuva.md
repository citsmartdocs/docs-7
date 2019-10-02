title: How to teach Anuva
# How to teach Anuva

Anuva learns from the dialogues added to its knowledge base. These dialogues are structured in **Interests** (possible phrases used in user interaction) and **Abilities** (possible chatbot responses to user interactions). 

Since Anuva works reactively to user interactions, in order to form dialogues we need to group interests and abilities in pairs. Contexts will be used only when, during the dialog, it is necessary to store some information that the user refers to for use in another point of the conversation.

It is up to the chatbot administrator to provide this data to the system, structuring the possible dialogues and to carry out the training of the set. The training should be scheduled through the Anuva interface, and at the end of the training, your Anuva will be updated automatically.

Procedure
------------

1.	Access the menu “Dialogues”;

2.	Click on "New" and select one of the options: Simple (only an Interest-Ability interaction) or Complex (when joining multiple simple dialogues);

3.	Inform the Theme related to the Dialogue, this will help you to categorize them, later. A new theme can be registered in the "Theme" menu;

4.	In the **Interests** section, complete the phrases related to the user Interest and click on "Save";

5.	In the **Abilities** section, complete the fields on the screen, paying attention to the ability type:

	   - Standard: it will be used to represent abilities that are answered through a predefined text response. Several                  predefined answer phrases can always be assigned to answer the same question;

	   - Customized: it will be used when, in order to respond to a user's interest, Anuva needs to seek information on                  another system. Access the document “How Anuva can interact with other systems” to understand how to use this type of            ability;

	   - Button: it will be used whenever it is necessary to limit user responses to a particular Anuva interaction. When                using this option, Anuva will respond to user interaction by displaying buttons. A button is defined by its Name and              Value. In the name field, the button that will appear for the user is defined. In the value field, it is defined to              Anuva how it should interpret the user's interest by clicking on the button;

	   - Image: it can be used when you want to respond to the user using text and image. The image associated with the                  response will be displayed in the chat window.


6. Click on "Save".

!!! Abstract "NOTE"

    - Complex dialogues help Anuva to be more assertive in a conversation that is long, use it to guide it 
      to how to respond in those situations;
    
    - Anuva's understanding is made by approximation, so the more phrases you add to the interest, the more 
      precise it will be in understanding the user's interaction. Remembering that the user does not have to 
      type the exact phrase that was added to the interest, since Anuva works with Artificial Intelligence;
                
    - Remember to add at least one dialog with fallback ability. It will be used when your Anuva cannot understand 
      the user's interest or understand with an accuracy of less than 20%. You can view the accuracy of each interaction 
      in the menu Analytics > List conversations.
 
 
Related
--------
 
[How to train Anuva](/en-us/anuva/use/trainning-anuva.html)
 
 

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/07/2019 - Anna Martins
    
