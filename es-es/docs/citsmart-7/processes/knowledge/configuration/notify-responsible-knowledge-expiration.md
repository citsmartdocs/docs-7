title: Notificar responsable por la expiración del conocimiento
Description: Configurar la notificación por correo electrónico para avisar al responsable (creador y publicador) acerca de la expiración de los conocimientos.
# Notificar responsable por la expiración del conocimiento


Este conocimiento tiene por objetivo configurar la notificación por correo
electrónico para avisar al responsable (creador y publicador) acerca de la
expiración de los conocimientos.

Antes de empezar
--------------------

Es necesario tener al menos un conocimiento registrado en la base de
conocimiento.

Procedimiento
-----------------

1.  Configurar el parámetro 78 con la cantidad de días anteriores a la
    expiración del conocimiento del cual desea notificar al responsable del
    conocimiento;

2.  Crear una rutina de procesamiento batch de notificación:

    -   Acceder al menú principal Sistema \> Procesamiento Batch y hacer clic en
        "Nuevo";

    -   Definir la descripción de la rutina, seleccionar el tipo "Clase Java" y
        establecer la situación como "Activo";

    -   Seleccionar la programación como "Diario" e indicar el horario en que se
        procesará la rutina;

    -   En la area "Contenido" copiar el guión abajo:

        -   br.com.centralit.citcorpore.quartz.job.VerificaValidadeBaseConhecimento

    -   Hacer clic en "Guardar".

3.  Si lo desea, puede personalizar la plantilla de correo electrónico. Sólo
    tienes que acceder a la funcionalidad a través del menú principal Sistema \>
    Configuración \> Modelo de e-mail, seleccionar la plantilla de correo
    electrónico con ID = "7" y realizar el cambio deseado.



Relacionado
----------
[Configurar parametrización - conocimiento](/es-es/citsmart-7/platform-administration/parameters-list/configure-parametrization-knowledge.html)

[Crear conocimiento](/es-es/citsmart-7/processes/knowledge/use/create-knowledge.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROzG1nEl9sfg_Y3Hy6spefP)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/24/2019 - Anna Martins
