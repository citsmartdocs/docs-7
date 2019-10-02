title: Registrar usuario
Description: Ofrece acciones diversas, como, incluir, cambiar y borrar un usuario.
# Registrar usuario

Para que el colaborador acceda al sistema, es necesario crear un usuario. Al registrarse, es posible que los datos del usuario (login y contraseña) se envíen al correo electrónico del colaborador. Para hacer esto, configure el parámetro 455 que indica la plantilla de correo electrónico (ID) creada para este propósito. La plantilla de correo electrónico debe contener las claves $ {LOGIN} y $ {NUEVACONTRASEÑA}.

Esta funcionalidad ofrece acciones diversas, como, incluir, cambiar y borrar un
usuario.

!!! warning "ATENCIÓN"

    El envío de login y contraseña al registrar un nuevo usuario no incluye los 
    usuarios importados a través de AD o LDAP.

## Antes de empezar

Para registrar un usuario, es necesario:

- [X] Registrar el Colaborador;

- [X] Tener al menos un Perfil de Acceso;

Para enviar el Login y Contraseña al correo electrónico del Colaborador:

- [X] Configurar el parámetro 33 e ingresar correctamente la URL de la instancia;

- [X] Configurar el parámetro 455 con la ID de la plantilla de correo electrónico creada para enviar los datos de acceso;

!!! note "EJEMPLO"
    
    Modelo basico: "Estimado usuario, siguen los datos de acceso. Nombre de usuario: $ {LOGIN} y contraseña: $ {NUEVACONTRASEÑA}"

## Procedimiento

1.  Acceder al menú principal Registros Generales \> Gestión de Personal \> Usurio;

2.  Completar los campos disponibles;

3.  Hacer clic en "Guardar".

!!! info "INFORMACIÓN"
    
    El sistema verifica si hay una plantilla de correo electrónico para el nuevo colaborador que tiene la clave de contraseña para enviar por correo electrónico. El administrador del sistema registra o cambia el inicio de sesión y la contraseña de un colaborador en la pantalla del usuario. El sistema verifica si: el sistema usa la política de contraseña y si el usuario es LDAP o no. El sistema le permite ingresar una nueva contraseña. Al guardar, el sistema envía los nuevos datos por correo electrónico al colaborador.
    
Relacionado
-----------

[Registrar colaborador](/es-es/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Crear perfil de acceso](/es-es/citsmart-7/initial-settings/access-settings/profile/create-profile-access.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 – Anna Martins

