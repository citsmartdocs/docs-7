title: Configure parametrization - LDAP
Description: this configuration of parameters linked to LDAP integration occurs implicitly using the LDAP Configuration feature or explicitly using the CITSmart Params feature.
# Configure parametrization - LDAP

Unlike other product parameters, this configuration of parameters linked to LDAP
integration occurs implicitly using the LDAP Configuration feature or explicitly
using the CITSmart Params feature.

Procedure
-------------

1.  Access the functionality through the main menu Parametrization \> CITSmart
    Parameters;

2.  Define the parameter value to be configured;

3.  Make the change;

4.  Click on "Save";

5.  The list below present the functionality parameters and the purpose of each
    one of them:



|  #  |                                              Name                                             | Possible Values |                                                   Purpose                                                   |                                                                                                                                        Additional Guidance                                                                                                                                        |
|:---:|:---------------------------------------------------------------------------------------------:|:---------------:|:-----------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|
|  39 | LDAP - ID of the access profile that will be set automatically if the user does not have any. |     E.g.: 2     |                              Enter the default Access Profile ID for the user.                              | When registering an user, and if the access profile is not informed, when the user logs into the application, the access profile (defined in the parameter value) will be established. This rule applies to users imported from AD. This Access Profile ID is set in the "Access Profile" screen. |
|  45 |                                    LDAP - Default Group ID.                                   |     E.g.:123    |       Enter the identification number (ID) of the default group, to which AD users will be associated       |                                                                                                                      This group ID is set on the "Group Registration" screen.                                                                                                                     |
| 409 |                LDAP - Attribute representing the immediate superior of the user               |   E.g.: Maria   | Name of the user's immediate superior in LDAP so that this information can be retrieved by the client's AD. |                                                                                                                  To be able to use in cases of approval of a ticket, for example.                                                                                                                 |


Table 1 - Parameters table

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/08/2019 - Anna Martins
