title: Cómo enseñar la Anuva
# Cómo enseñar la Anuva

Anuva aprende a partir de los diálogos añadidos a su base de conocimiento. Estos diálogos se estructuran en Intereses (posibles frases utilizadas en la interacción del usuario) y Habilidades (posibles respuestas del chatbot a las interacciones del usuario).

Como Anuva funciona de forma reactiva a las interacciones del usuario, para formar diálogos necesitamos agrupar intereses y habilidades en pares. Los contextos se utilizarán sólo cuando, durante el diálogo, es necesario almacenar alguna información citada por el usuario para utilizar en otro punto de la conversación.

Es responsabilidad del administrador del chatbot, proporcionar estos datos al sistema, estructurando los posibles diálogos y para que sea realizado el entrenamiento del conjunto. El entrenamiento debe ser programado por la interfaz de Anuva, y al final del entrenamiento, su Anuva será actualizada automáticamente.

Procedimiento
------------

1. Acceder al menú “Diálogos”;

2. Haga clic en "Nuevo" y seleccione una de las opciones Simple (sólo una interacción Interes-Habilidad) o Complejo (cuando se unen varios diálogos simples);

3. Informar el Tema relacionado al Diálogo, esto te ayudará a categorizarlos posteriormente. Un nuevo tema puede ser registrado en el menú "Tema";

4. En la sección Intereses, completar las frases relacionadas con el Interés del usuario y hacer clic en "Guardar";

5. En la sección Habilidades, completar los campos de la pantalla, atentándose al tipo de la habilidad:

    - Estándar: se utilizará para representar las habilidades que se responden a través de una respuesta de texto predefinida. Se pueden 
    asignar varias frases predefinidas de respuestas siempre para responder a la misma pregunta;

    - Personalizada: se utilizará cuando, para responder a un interés del usuario, Anuva necesita buscar información en otro sistema.
    Acceda a la documentación "Cómo Anuva puede interactuar con otros sistemas" para entender cómo utilizar este tipo de habilidad.

    - Botón: Se utilizará siempre que sea necesario limitar las respuestas del usuario a una determinada interacción de Anuva. Al 
    utilizar esta opción, Anuva responderá a la interacción del usuario mostrando botones. Un botón se define por su nombre y valor. En
    el campo nombre, se establece el botón que aparecerá para el usuario. En el campo valor, se establece en Anuva cómo debe interpretar
    el interés del usuario al hacer clic en el botón;
 
    - Imagen: Puede utilizarse cuando desee responder al usuario utilizando texto e imagen. La imagen asociada a la respuesta aparecerá
    en la ventana de chat.

6. Hacer clic en "Guardar".

!!! Abstract "NOTA"

    - Diálogos complejos ayudan a Anuva a ser más asertiva en una conversación que es larga, úsela para orientarla 
    a cómo responder en esas situaciones;
    
    - La comprensión de Anuva es hecha por aproximación, siendo así, cuanto más frases usted añadir al Interés, 
    más precisa ella será en el entendimiento de la interacción del usuario. Recordando que el usuario no necesita 
    escribir la frase exacta que fue agregada al interés, pues Anuva trabaja con Inteligencia Artificial;
                
    - Recuerde de añadir al menos un diálogo con habilidad de fallback. Se utilizará cuando su Anuva no pueda entender 
    el interés del usuario o entender con una exactitud inferior al 20%. Puede ver la exactitud de cada interacción en 
    el menú Analytics > Listar conversaciones.
 
 
Relacionado
--------
 
[Cómo entrenar su Anuva](/es-es/anuva/use/trainning-anuva.html)
 
 

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/07/2019 - Anna Martins
    
