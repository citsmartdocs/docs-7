Title: Flujo de integración de servicios  
Description: Los flujos de integración de servicios, como el propio nombre dice, involucra workflows ejecutados en base a servicios del sistema, como integraciones y conversiones, por ejemplo.   


# Flujo de integración de servicios   

Los flujos de integración de servicios, como el propio nombre dice, involucra workflows ejecutados en base a servicios del sistema, como integraciones y conversiones, por ejemplo.   

## Cómo acceder    

1- Acceda a la funcionalidad a través del menú Neuro > Administración > Flujo de integración.     

## Condiciones previas    

1- No se aplica.   

## Filtros  

1- El siguiente filtro permite al usuario restringir la participación de elementos en el listado estándar de la funcionalidad, facilitando la localización de los elementos deseados:   

- Palabra clave  

![Screenshot](images/Service-Integration-Flow-fig01.png)

Figura 1 - Pantalla de búsqueda    

## Lista de elementos    

1- Los siguientes campos catastrales están disponibles para el usuario para facilitar la identificación de los elementos deseados en el listado estándar de la funcionalidad: Nombre, Descripción, Aplicación del flujo, Versión y Fecha de bloqueo.   

![Screenshot](images/Service-Integration-Flow-fig02.png)   
Figura 2 - Pantalla de lista     

## Completar campos catastrales - Datos del flujo   

A través de esta pestaña, se definen las informaciones básicas del flujo que será dibujado.   

1- Para añadir un nuevo flujo, haga clic en Registrar > Flujo de servicios de integración, como se muestra en la figura siguiente:   

![Screenshot](images/Service-Integration-Flow-fig03.png)

Figura 3 - Pantalla de registro   

2- Para registrar un nuevo dato del flujo, haga clic en "Agregar".   
3- Se presentará la siguiente pantalla:    

![Screenshot](images/Service-Integration-Flow-fig04.png)

Figura 4 - Pantalla de registro/edición del workflow, pestaña de Datos del Flujo    

4- Introduzca un nombre para el flujo, una descripción, que formulario comenzará el flujo (en su caso), y si persiste o no la ejecución del flujo. Si el campo "Persiste la ejecución del flujo" se marca, el Neuro persistirá en la base de datos de toda instancia de la ejecución de este flujo.    

5- El campo de versión se incrementa automáticamente por el sistema cada vez que se crea una nueva versión del workflow.    

## Variables  

En esta pestaña se configuran las variables que se utilizarán en el flujo dibujado. Las variables son objetos capaces de retener y representar un valor o una expresión. Las variables se asocian a "nombres", llamados identificadores, durante el tiempo de ejecución del flujo.  

1- Para agregar una variable, seleccione la pestaña correspondiente y haga clic en "Agregar".  
2- Se mostrará la siguiente pantalla:    

![Screenshot](images/Service-Integration-Flow-fig05.png) 

Figura 5 - Pantalla de registro/edición del workflow, pestaña de Variables     

3- Completar los campos:    

- Nombre de la variable;

- Descripción;

- Se almacenará en la base de datos;  

     * Esta opción almacenará el valor de la variable internamente dentro del modelo de datos de Neuro, por lo que conservará el valor
     durante la ejecución de las tareas  

- Si es una variable de retorno;  

     * Esta opción hará que Neuro devuelve la variable al final de la ejecución del flujo.  

- Si es una lista de valores;

- Si es una variable de entrada en la interfaz de flujo;  

     * Esta opción permite que la variable sea "inyectada" en el proceso de negocio vinculado a este flujo.  

- Si es una variable de salida en la interfaz de flujo;  

     * Esta opción hace que la variable tenga el valor completado cuando se ejecuta el proceso de negocio vinculado al flujo.  

- El tipo de la variable;  

    * Si es un objeto Java, introduzca la clase correspondiente de Java; 
	
    * Si es un objeto de negocio, informe cuál es su aplicación respectiva y cuál es el nombre registrado del objeto de negocio;  

- El valor inicial de la variable, si constante o script.  

    * Si el valor es una constante, éste nunca cambiará durante la ejecución del flujo, independientemente de las operaciones realizadas
    por el usuario.  

4- Para editar una variable, seleccione la variable deseada, haga clic en Editar, realice los cambios necesarios y haga clic en
Actualizar para completar la edición.  

5- Para eliminar una variable de flujo, seleccione la variable deseada, haga clic en Eliminar y confirme la eliminación.    

!!! Abstract "ATENCIÓN"  

    Para guardar efectivamente los cambios, haga clic en Guardar en la barra superior.  

## Acciones  

Por medio de este menú, es posible registrar las acciones que serán ejecutadas en el workflow.   

Las acciones se basan en scripts programados en el lenguaje Rhino.   

1- Para agregar una acción, seleccione su ficha correspondiente y haga clic en "Agregar".   
2- Se mostrará la siguiente pantalla:  

![Screenshot](images/Service-Integration-Flow-fig06.png) 

Figura 6 - Pantalla de registro/edición del workflow, pestaña de Acciones   

3- Completar los campos:   

- Un identificador para la acción;    
- El nombre literal para la misma;   
- El script que se ejecutará cuando se acciona la acción.    

4- Para editar una acción, seleccione la acción deseada, haga clic en "Editar", realice los cambios necesarios y haga clic en "Actualizar" para completar la edición.  

5- Para eliminar una acción, seleccionéla, haga clic en Eliminar y confirme la eliminación.   

!!! Abstract "ATENCIÓN"  

    Para guardar efectivamente los cambios, haga clic en Guardar en la barra superior.

## Diagrama  

El diagrama de un flujo de servicios no tiene los mismos componentes de "Tarea" de un flujo de proceso. No es posible utilizar aquí los componentes de "Tarea humana" y "Sub proceso workflow".  

Para un proceso de negocio, poseemos más las secciones de componentes:   

- Conectores: componentes utilizados para la ejecución de operaciones relacionadas con la base de datos.  
- Componentes: componentes variados para la ejecución de diversas tareas.  
- Transformadores: componentes para la conversión de tipos de variables.  
- CITSmart ITSM: componentes utilizados para la integración con un sistema CITSmart ITSM externo.   

Los demás componentes presentes en la paleta se asemejan a los componentes de un "Flujo de proceso". Más información sobre la funcionalidad y el uso de cada uno de los componentes se pueden encontrar en el desarrollo de aplicaciones.    

1- Para diseñar el diagrama, elija la pestaña refente al mismo.  
2- Se presentará la siguiente pantalla:  

![Screenshot](images/Service-Integration-Flow-fig07.png)

Figura 7 - Pantalla de registro/edición del workflow, pestaña de Diagrama  


!!! tip "About"
    <b>Updated:</b>17/01/2019 - João Pelles Junior
