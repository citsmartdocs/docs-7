Title: Cómo interactuar Anuva con otras interfaces
# Cómo interactuar Anuva con otras interfaces

Para que Anuva interactúe con otros sistemas, es necesario agregar en el diálogo una habilidad personalizada.

La consulta se realiza a través de una API Rest, la cual necesita ser puesta a disposición por el sistema que detenta la información de interés del usuario. Ej.: buscar información sobre el estado de un ticket, creación de tickets, generación de boletos en el sistema.

Procedimiento
-----------

1. Acceder al menú "Diálogos" y hacer clic en Nuevo;

2. Completar la información de la sección **Interés**;

3. En la sección **Habilidad**, seleccionar el tipo *Personalizado*;

4. Completar la información de la sección API, incluido el ejemplo del cuerpo y de la respuesta;

5. Si es necesario, introduzca el encabezado;

6. En la sección Respuestas, son dos opciones de acción:

    a) Respuestas en memoria: En este caso, el valor devuelto por la API se asocia al atributo seleccionado;
 
    b) Respuestas en texto: devuelve un mensaje de texto al usuario.
  
  
!!! Abstract "NOTA"

    La integración necesita ser homologada por la CITSmart, siendo así que después de 
    configurar esta habilidad es necesario abrir un ticket para que la hagamos la 
    homologación de la integración.
    
    
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/07/2019 - Anna Martins
   
