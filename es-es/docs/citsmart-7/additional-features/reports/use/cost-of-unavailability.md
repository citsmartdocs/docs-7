title: Informe del custo de indisponibilidad del servicio
Description: Verificar el informe que demuestra el costo por hora de indisponibilidad de un servicio.
# Informe del custo de indisponibilidad del servicio


Este documento tiene por objetivo verificar el informe que demuestra el costo
por hora de indisponibilidad de un servicio, donde:

-   Tiempo Disponible: tiempo (dentro de la jornada de trabajo) que los
    incidentes del servicio quedará disponible en el período;

-   Tiempo Indisponibilidad: tiempo en horas (dentro de la jornada de trabajo)
    que los incidentes del servicio quedarán indisponibles en el período;

-   Número de caídas: cantidad de incidentes del servicio;

-   MTBSI = Tiempo disponible / Nºde caídas;

-   MTBF = (Tiempo disponible - Tiempo Indisponibilidad) / Nº de Caídas;

-   MTRS = Tiempo Indisponibilidad / Nº de caídas.

Antes de empezar
--------------------

En el portafolio de servicios, un servicio deberá tener el
atributo **Incidente** con el campo "Causa indisponibilidad" establecido igual a
"SÍ".

En el atributo **Contrato** del servicio elegido, el incidente deberá estar
vinculado, así como definir el Costo de Indisponibilidad, el Acuerdo de
Disponibilidad y también vincular el Calendario.

El informe, disponible a través de los datos adjuntos, se debe importar en el
Generador de informes Smart.

Procedimiento
-----------------

*Paso 1*

1.  Acceder el menú Informes \> Informes Smart \> Generador de Informes Smart;

2.  Hacer clic en "Importar";

3.  Seleccionar el archivo disponible (adjunto) y hacer clic en "Abrir";

4.  En la página de lista de informes, hacer clic en "Editar" del informe
    importado;

5.  Seleccionar la opción *N/A* en el campo Módulo (s) donde se
    visualizará y definir el(los) grupo(s);

6.  Hacer clic en "Guardar".

*Paso 2*

1.  Acceder al menú principal Procesos \> Gestión de Portafolio y Catálogo \>
    Portafolio;

2.  Elegir un portafolio y hacer clic en "Avanzar";

3.  Elegir un servicio y hacer clic en "Avanzar";

4.  Hacer clic en el atributo **Incidentes**, después en "Nuevo Incidente" (el
    campo "Tipo de Demanda" deberá ser Incidente, así como el campo "Causa
    Indisponibilidad" deberá ser "SI");

5.  Hacer clic en "Guardar";

6.  Hacer clic en "Vincular Incidente" y vincular el incidente creado
    anteriormente.

*Paso 3*

1.  Hacer clic en el atributo **Contratos** del servicio;

2.  Seleccionar un contrato y hacer clic en "Avanzar";

3.  Hacer clic en el atributo** Incidentes** del contrato y después en "Vincular
    Incidente";

4.  Completar los campos disponibles, agregando también el incidente creado
    anteriormente;

5.  Hacer clic en "Guardar";

6.  Hacer clic en el atributo **Custo de Indisponibilidad**, definir el valor y
    hacer clic en "Guardar";

7.  Hacer clic en el atributo **Acuerdo de Disponibilidad**, hacer clic en
    "Vincular Acuerdo de Disponibilidad y definir un SLA;

8.  Hacer clic en el atributo **Calendario**, hacer clic en "Vincular
    Calendário" y definir un calendário.

Lo que hacer después
------------

Acceder al panel de administración en el Smart Portal, agregar el informe
importado previamente, definir las fechas y comprobar el informe.

El informe también se puede ver en Informes Smart.



Relacionado
-----------

[Registrar servicio](/es-es/citsmart-7/processes/portfolio-and-catalog/use/register-a-service.html)

[Configurar atributos del servicio](/es-es/citsmart-7/processes/portfolio-and-catalog/use/configure-services-attributes.html)

[Configurar atributos del contrato de servicio](/es-es/citsmart-7/processes/portfolio-and-catalog/use/service-contract-attributes.html)

[Crear portafolio](/es-es/citsmart-7/processes/portfolio-and-catalog/use/create-the-portfolio.html)

[Acuerdo de Nivel de Servicio](/es-es/citsmart-7/processes/service-level/use/service-level-agreement.html)

[Personalizar el panel gerencial (Smart Decision)](/es-es/citsmart-7/additional-features/reports/create/dashboard-customize-management-panel-smart-decision.html)

[Emitir informe utilizando Smart Report](/es-es/citsmart-7/additional-features/reports/create/smart-reports/configuration/create-smart-report.html)

[Construir y mantener informes Smart - V.8.0](/es-es/citsmart-7/additional-features/reports/create/smart-reports/configuration/build-maintain-smart-report.html)


Adjunto
-----
[Download-Confiabilidad][1]

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Anna Martins

[1]:/es-es/citsmart-7/additional-features/reports/use/images/confiabilidade.citreport
