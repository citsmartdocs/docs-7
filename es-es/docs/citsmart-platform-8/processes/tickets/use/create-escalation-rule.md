title: Crear regla de escalonamento
Description: Esta funcionalidad permite crear reglas de escalonamento. 
# Crear regla de escalonamento

Esta funcionalidad permite crear reglas de escalonamiento para proporcionar una perspectiva de impacto a la empresa al gestionar las atenciones de los tickets (y sus eventuales solicitudes e incidentes), dentro de un tiempo hábil preestablecido. Al crear reglas para la notificación del responsable, cuando el ticket está en nivel crítico de ruptura de su SLA, es posible evitarlo a través de acciones preventivas y escalonar esta atención a otros grupos ejecutores, y respetar así, su tiempo de atención.

Antes de empezar
----------------

Para crear las reglas de escalonamiento, es necesario configurar el parámetro
190 con el valor "S", y registrar previamente los contratos, empleados, grupos,
los portafolios de servicios y la acción automática del tipo escalonamiento.

En el archivo **citsmart.cfg**, debe configurar la propiedad
**START_MONITORA_INCIDENTES** informando el parámetro TRUE (sólo el
administrador del sistema operativo del servidor de la aplicación realiza este
ajuste).

Procedimiento
-------------

1.  Acceder a la funcionalidad por el menú principal Procesos ITIL \> Gestión de
    Requerimiento e Incidente \> Reglas de escalamiento;

2.  Haga clic en "Nuevo";

3.  Informar los datos generales de la Regla de Escalonamiento (Título,
    situación, el solicitante, el grupo ejecutor de la atención, el portafolio y
    contrato a ser vinculado a la regla y el impacto y urgencia de la atención
    del ticket);

4.  Informar los datos específicos de la Regla de Escalonamiento:

| **Campo** |                                                       **Objetivo**                                                      |
|:---------:|:-----------------------------------------------------------------------------------------------------------------------:|
|   Tiempo  |                               Informar el plazo de escalonamiento/notificación del ticket                               |
|  Formato  |         Indicar si la regla se refiere a minutos (tiempo de la regla) o porcentual (referente al tiempo del SLA)        |
| Condición | Seleccionar el marco del escalonamiento/notificación (si esto ocurrirá antes o después de la ruptura del plazo elegido) |
|   Fecha   |     Seleccionar la fecha de referencia de la regla (la fecha de creación, de la última ocurrencia o su fecha límite)    |
|   Acción  |                                  Vincular el tipo de acción automática a la nueva regla                                 |

Relacionado
-----------

[Crear portafolio](/es-es/citsmart-7/processes/portfolio-and-catalog/use/create-the-portfolio.html)

[Registrar grupo](/es-es/citsmart-7/initial-settings/access-settings/user/register-groups.html)

[Registrar colaborador](/es-es/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Registrar contrato](/es-es/citsmart-7/additional-features/contract-management/use/register-contract.html)

[Registrar acción automatica de escalonamiento](/es-es/citsmart-7/additional-features/automation-of-operation/configuration/register-escation-automatic-action.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROfIFL9F-3s-gomHNzudBEy)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/25/2019 - Larissa Lourenço
