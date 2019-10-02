Title: Configurar notificación sonora
Description: Configuración de una alarma sonora para señalar al asistente la llegada de un nuevo ticket

# Configurar notificación sonora

Esta función permite la configuración de una alarma sonora para señalar al asistente la llegada de un nuevo ticket en su cola de ticket.

## Antes de empezar

* [x] Tenga al menos un flujo de trabajo definido en su entorno CITSmart;
* [x] Es esencial tener las condiciones mínimas para la reproducción de audio en su ordenador;

## Procedimiento

### Crear plantilla de notificación

1. Acceder al menú principal Sistema > Notificaciones > Plantilla de Notificación;
2. Hacer clic en "Nuevo" para crear una nueva plantilla;
3. Informar los datos de notificación, hacer clic en "Notificación Sonora" e importar el archivo de audio;
4. Guardar las informaciones.

### Insertar elemento "Notificación" en el flujo

1. Acceder al menú principal Workflow > Diseño de flujo;
2. Seleccionar y editar un flujo;
3. En la pestaña "Diagrama", haga clic en el elemento "Extensiones", haga clic y mantenga presionado el elemento "Notificación" y
arrástrelo al área de dibujo;
4. Haga doble clic en el icono "Notificación", y después en la pestaña "Configuración";
5. En el campo "Plantilla de notificación", seleccione la plantilla para la notificación;
6. Guardar los cambios en el flujo;

## Lo que hacer después

Listo, de ahora en adelante será posible identificar nuevos tickets mediante la notificación sonora.

!!! warning "ATENCIÓN"

    Incluso, si el usuario recibe varias notificaciones al mismo tiempo, la alarma sonora solo se activará una vez.

## Relacionado

[Registrar plantilla de notificación][1]

[Crear flujo de trabajo][2]


[1]:/es-es/citsmart-7/additional-features/communication-and-notification/notification/configuration/template-create.html

[2]:/es-es/citsmart-7/workflow/use/create-flow.html
