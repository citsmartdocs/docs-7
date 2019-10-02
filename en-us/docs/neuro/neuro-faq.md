Title: Neuro FAQ
Description: CITSmart - FAQ

# Neuro Frequently Asked Questions (FAQ)

!!! Question "What is the difference between creating a form using the Form menu and via the Business Object?"

    The creation using the Form menu is 100% manual. If you use the business object menu, you can generate the form from the database. The generated form can be edited in the menu register form.

	How do I create a menu to access my business process?

	The creation the menu for business process, is made in the registration of the business process itself by setting the field "menu".

	It is necessary a previously registered menu with two levels, so it can be linked to this process.

	It is also necessary that after saving the business process with the associated menu, the permissions to the new menu item must be assigned. The assignment of this permission can be accomplished through the menu or the access profile screen.

!!! Question "How do I create "many-to-many" relationships in the business object?"

	To create a "many-to-many" relationship, it is necessary to create a third business object to relate the two objects of the desired business.

	E.g.: Let's create a many-to-many relationship between two objects, **A** and **B**. We will need an object **C** that will relate with **A** and **B**.

	The object **A** will have a one-to-many "relationship" with the object **C**, and object **B** will also have a one-to-many "relationship" with the object **C**.

	The object **C** we will need to have two relationships, one of them "many-to-one," with the object **A** and the other "many-to-one," with the object **B**.

	We can relate a data from object **A** to a lot of data of the object **B**, and the object **B** can do the same with object **A**, through the business object **C**.

!!! Question "I would like to know if every workflow must have a business process?"

	Not every workflow must have or needs a business process. Every Main Workflow needs a business process, however the sub-processes don't require other business processes.

	In addition, this this rule only applies to process integration flows. The service integration flows do not require a related business process.

!!! Question "Is there any alternative to access my workflow tasks opened in a customized menu? I mean, out of task management?"

	You can make your own task list to access the workflow tasks. For a complete tutorial, please check the technical documentation.

!!! Question "Is it possible to create customized components that can be used in the forms creation?"

	You can create your own components that will be used in the form. For a complete tutorial, please check the technical documentation.

!!! Question "Where should I start building an application using the Neuro?"

	It is recommended that the first step to be executed on the Neuro, is to register the application or register a connection to the DB (database), according to the needs of the application.

!!! Question "How does it work the dependency injection in a Neuro form? Which steps must be performed?"

	To inject a dependency , you must register it before. Only CSS and Javascript dependencies types can be injected in a Neuro form.

	Create a new register according to the dependency type. It can be done via menu "Neuro > resources" and upload the dependency.

	To import it on the form, select the tab “page type” that you would like to import and choose the tab "Dependencies".

	Click on the "+ add" icon to add a new dependency, in the field "name" enter the name of your resource dependency and select the corresponding option. For more information about form dependencies, please check the technical documentation.

!!! Question "How do I define the actions that should be available in each workflow task?"

	The actions are registered in the main register flow tabs. To associate an action to a specific task, go to the workflow design, open the element properties, and select the desired actions. After all that is done, save your changes.

!!! Question "How do I delete an element from the workflow?"

	To delete a workflow element, select the element you want to delete, and then press Ctrl + Del.

!!! Question "What do I do when I get this error message "business process not informed"?"

	This error occurs because the business process is not referenced in the controller of the form that starts the business process. To fix this problem, access the business process form, and then insert the following command on the controller "p/process Page": $scope. businessProcessName = ' name_of_the_business_process';

!!! Question "I would like to know, when I register a sub-process, the information in the main process is inherited by the sub-process?"
	
	No, it doesn´t inherit. When you include a new sub-process, BPE or ESI in the main workflow, you must inform the "attributes", the exact name of the sub-process that must be created on the workflow registration.

	All information, such as actions and main workflow status should be replicated in the sub-process registration.

	In short steps, it is recommended to follow the following order:

	1. Register the main workflow;
        2. Register the sub-process;
	3. Include the element of sub-process, making a reference to the sub-process already created.

!!! Question "What is the difference between a process integration workflow and a service integration workflow?"

	The process integration workflow has tasks performed by users, and may also have automated tasks performed by the system.

	The service integration workflow has workflows that were executed, based on system services, such as integrations and conversions, for example.

	There is no problem if a process integration workflow uses a sub-process of the service integration workflow.
