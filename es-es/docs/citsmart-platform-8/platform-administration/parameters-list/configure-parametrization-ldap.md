title:  Configurar parametrización – LDAP 
Description: Esta configuración de parámetros conectados a la integración con LDAP 
# Configurar parametrización – LDAP

A diferencia de los demás parámetros del producto, esta configuración de parámetros conectados a la integración con LDAP se produce de forma implícita mediante la funcionalidad de configuración LDAP o de forma explícita mediante la funcionalidad Parámetros de CITSmart.

Procedimiento
-------------

1.  Acceder al menú principal Parametrización \> Parámetros CITSmart;

2.  Definir el valor del parámetro que se va configurar;

3.  Hacer el cambio;

4.  Hacer clic en "Guardar";

5.  La lista siguiente muestra los parámetros de la funcionalidad y el propósito
    de cada uno de ellos:

| **#** |                                            **Nombre**                                            | **Valores posibles** |                                                      **Finalidad**                                                     |                                                                                                                                             **Orientaciones complementarias**                                                                                                                                             |
|:-----:|:------------------------------------------------------------------------------------------------:|:--------------------:|:----------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|   39  | LDAP - ID del perfil de acceso que se establecerá automáticamente si el usuario no tiene ninguno |        Ej.: 2        |              Indicar el número de identificación (ID) del perfil de acceso predeterminado para el usuario              | Al registrar un usuario, y si no se informa el perfil de acceso, cuando el/ella accede a la aplicación, se establecerá el perfil de acceso (definido en el valor del parámetro). Esta regla vale para los usuarios importados del AD. Este identificador de perfil de acceso se define en la pantalla "Perfil de acceso". |
|   45  |                                    LDAP - ID de grupo estándar                                   |        Ej.:123       |        Indicar el número de identificación (ID) del grupo predeterminado al que se asociarán los usuarios del AD       |                                                                                                                             Este ID del grupo se define en la pantalla de "Registro de Grupo".                                                                                                                            |
|  409  |                 LDAP - Atributo que representa el superior inmediato del usuario                 |      Ej.: Maria      | Nombre del superior inmediato del usuario en el LDAP para que se pueda recuperar esa información por el AD del cliente |                                                                                                                             Para poder usar en casos de aprobación de un ticket, por ejemplo.                                                                                                                             |

Tabela 1 - Tabela de parâmetros

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/28/2019 - Larissa Lourenço
