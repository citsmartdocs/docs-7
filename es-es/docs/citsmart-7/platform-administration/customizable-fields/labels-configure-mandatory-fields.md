title: Configurar campos obligatorios
Description: El administrador es responsable de elegir qué campos serán obligatorios para que los usuarios completen.
# Configurar campos obligatorios

Al configurar los campos obligatorios, el administrador elegirá qué campos serán obligatorios para que los usuarios completen al comunicarse con los asistentes. Su propósito es obtener la información necesaria de los solicitantes para resolver la solicitud.

Procedimiento
-------------

1.  Acceder al menú principal Sistema \> 
    Configuración \> Páginas - Configuración de campos;

2.  Se presentarán las páginas con la posibilidad de elección de los campos obligatorios.
    Ellas son: Gestión de Problema y Gestión de Incidentes/Solicitudes.

### Configurar los campos de la funcionalid "Problema"

*Al decidir utilizar campos obligatorios, es posible exigir que cierta información sea
registrado al crear un problema.*

1.  Después de acceder a la página de inicio de la funcionalidad, elija la opción "Problema" y haga clic en "Editar";
     
2.  Seleccione los campos que desea hacer obligatorios. Son:

    |   **Nombre del campo**   | **Obligatorio** |
    |:------------------------:|:--------------:|
    |         Catálago         |      :ballot_box_with_check:                  |
    |   Categoría de Servicio  |       :ballot_box_with_check:                 |
    |          Servicio        |       :ballot_box_with_check:                 |
    |         Teléfono         |          :ballot_box_with_check:              |
    |         Extensión        |        :ballot_box_with_check:                |
    |     Ubicación Física     |      :ballot_box_with_check:                  |
    |        Observación       |           :ballot_box_with_check:             |
    |      Grupo ejecutor      |        :ballot_box_with_check:                |
    |Solucionar/Contornar hasta|    :ballot_box_with_check:                    |

3.  Hacer clic en "Guardar".

### Configurar campos de la funcionalidad "Gestión de Ticket"

*Al decidir utilizar campos obligatorios, es posible exigir que cierta información sea
registrado al crear un incidente/solicitud.*

1.  Después de acceder a la página de inicio de la funcionalidad, elija la opción
    "Gestión de Incidentes/Solicitudes" y hacer clic en "Editar";
    
2.  Seleccione los campos que desea hacer obligatorios. Son:

    | **Nombre del campo** | **Obrigatório** |
    |:--------------------:|:--------------:|
    |       Teléfono       |       :ballot_box_with_check:                 |
    |        E-mail        |          :ballot_box_with_check:              |
    |        Unidad        |           :ballot_box_with_check:             |
    |   Ubicación Física   |       :ballot_box_with_check:                 |
    |    Orígen Contacto   |     :ballot_box_with_check:                   |

    !!! Abstract "ATENCIÓN"
    
        Los parámetros 65 (que identifica el ID de origen de la llamada predeterminada 
        de la solicitud de servicio) y 105 (identifica el ID de origen que se establecerá como
        predeterminado al crear un nuevo incidente) configuran un origen de contacto 
        automáticamente cuando el usuario registra un ticket. Por lo tanto, si el campo
        Origen del contacto" en la pantalla de ticket *no* es obligatorio, pero hay un
        apunte en los parámetros anteriormente citados, el campo se completará automáticamente.
        
3.  Hacer clic en "Guardar".        

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Larissa Lourenço
