Title: Disponer Anuva en la interfaz CITSmart
# Disponer Anuva en la interfaz CITSmart

Anuva ya se integra nativamente al CITSmart, entonces es muy fácil añadirla a su entorno.

## Procedimiento

1. Con acceso de administrador, acceda a la pantalla de parámetros del CITSmart;
2. Cambiar el valor del parámetro “402 Anuva Assistant - External URL” para http://[nombre-servidor].anuvaassistant.com
3. Cambiar el valor del parámetro “441 Anuva Assistant - Conversation API” para http://[nombre-servidor][sigla-idioma].anuvaassistant.com/webhooks/rest/webhook y hacer clic en "Guardar"
4. Cambiar el valor del parámetro “442 Anuva Assistant - Parameters API” para http://[nombre-servidor][sigla-idioma].anuvaassistant.com/conversations/
5. Configurar el parámetro 453 "Mensaje predeterminada de Fallback de la Anuva Assistant", con un mensaje que Anuva responderá cuando no tenga respuesta a esa pregunta.
6. Habilitar el parámetro 423 "Habilitar Anuva Assistant en el área interna del sistema", un parámetro que permite a los analistas iterar con ANUVA
7. Habilitar el parámetro 450 "Habilitar Anuva Assistant en el área externa del sistema", parámetro que permite a los usuarios finales iterar con ANUVA.    

!!! note "NOTA"
    
    Para la abreviatura de los idiomas, utilice EN (Inglés) y PT (Portugués-Brasil).
    Si estos parámetros no están disponibles, actualice su versión de CITSmart.
   
 
!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>04/07/2019 - Anna Martins
