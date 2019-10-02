title: Manual de uso de la aplicación CITSmart GO
Description: Permitir la realización de llamadas para técnico en campo en modo offline (donde el operador no tiene internet).
# Manual de uso de la aplicación CITSmart GO

El objetivo de la aplicación CITSmart GO es permitir la realización de llamadas
para técnico en campo en modo offline (donde el operador no tiene internet).

Antes de empezar
--------------------

1.  Tener configurado la aplicación en la instancia ITSM;

2.  Instalar la aplicación CITSmart GO en el móvil;

3.  Es necesario delegar tareas al técnico en el sitio CITSmart para que se
    pueda atender en campo en el modo offline.

Procedimiento
-----------------

!!! Abstract "ATENCIÓN"

    Al iniciar sesión en la aplicación CITSmart GO, la primera sincronización puede 
    tardar unos instantes, ya que para funcionar sin conexión tiene que descargar todas 
    las solicitudes y enviar las que han cambiado para que la aplicación funcione 
    correctamente.

1.  Informar los datos para acceder a la aplicación;

2.  Seleccionar y hacer clic en un ticket. Se mostrará una pantalla con los
    datos de la solicitud, incluyendo un mapa del lugar donde se realizará la
    atención;

3.  Hacer clic en "Ejecutar solicitud" y luego "Otras informaciones" (sólo está
    disponible si existe un cuestionario vinculado a la actividad del ticket).
    Completar los datos referentes a la ejecución de la solicitud y hacer clic en
    "Guardar";
    
    !!! Abstract "ATENCIÓN"
    
        Sólo los componentes simples de Neuro, como los formularios, se pueden representar 
        en el Mobile GO. Estos formularios no pueden tener ninguna lógica de JavaScript vinculada 
        a ellos, deben ser similares al cuestionario existente en el CITSmart SM.
        
    !!! Abstract "REGLA"
    
        No es posible vincular un EC a la base de conocimiento por el mobile GO.
    
4.  Si quiera adjuntar un adjunto, haga clic en la pestaña "Adjuntos";

5.  Hacer clic en "Notas" e informe la ocurrencia referente al ticket y la fecha que se la sucedió. Es posible también registrar             el tiempo gastado para la solución de la ocurrencia. Se pone a disposición la visualización de este relato por el solicitante y el       envío del mismo al correo electrónico al seleccionar las opciones "Vísible al solicitante" y "Enviar al correo electrónico". Hacer       clic en "Guardar";

6.  Hacer clic en "Finalizar" y completar los datos sobre la terminación de la
    atención. Seleccionar la situación de la atención (en curso, resuelta o
    cancelada) y los detalles;

7.  Hacer clic en "Recoger firma y Avanzar el Flujo" o "Guardar y mantener la tarea
    actual" para completar la operación. Se sincronizará automáticamente los
    cambios. Si la aplicación no encuentra la red para completar la
    sincronización, aparecerá el icono  para esperar acceder a la red y después
    completar la sincronización;

8.  Está disponible la sincronización manual de las solicitudes tan pronto la
    aplicación encuentre una red accesible. Para ello, simplemente deslice la
    pantalla hacia abajo con el dedo o haga clic en el icono "Actualizar lista";

9.  Hay filtros que facilitan la localización del ticket necesario, se lo acceda
    por el cuadro de búsqueda o haga clic en el icono "Filtros".


Relacionado
-----------

[Configurar instancia para utilizar la aplicación CITSmart GO](/es-es/citsmart-7/additional-features/mobile-and-field-service/configuration/configure-field-service-application.html)

[Obtener signatura en atención de campo](/es-es/citsmart-7/additional-features/mobile-and-field-service/use/get-signature-in-attendance.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 – Anna Martins
