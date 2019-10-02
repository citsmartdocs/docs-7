title: Configure parametrization - telephony
Description: Allows to define whether to enable the integration of webservices with telephony, to inform the identification number of the request service, among other possible actions in order to configure the use of telephony in CITSmart.
# Configure parametrization - telephony

The "Telephony" parametrization allows to define whether to enable the
integration of webservices with telephony, to inform the identification number
of the request service, among other possible actions in order to configure the
use of telephony in CITSmart.

Procedure
-------------

1.  Access the functionality through the main menu Parametrization \> Telephony;

2.  Define the parameters values (attributes);

3.  Click on "Save";

4.  The list below presents the "Telephony" parameters and the purpose of each
    one of them:

|  #  |                                                               Name                                                               |   Possible Values   |                                                                                     Purpose                                                                                     |                                        Additional Guidance                                        |
|:---:|:--------------------------------------------------------------------------------------------------------------------------------:|:-------------------:|:-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------------------------------------------------------------------------------------:|
| 281 |                        Enable Webservice for integration with Telephony - Values: "Y" or "N" Default: "N"                        | Y or N (Default: N) |                                                         Define whether to enable webservices integration with telephony.                                                        | If the value for the parameter is not set, the value "N" will be automatically set by the system. |
| 282 | Should telephony launch a child request regarding viewing information for an existing request? - Values: "Y" or "N" Default: "N" | Y or N (Default: N) |                   Set whether to enable the automatic launch of a child service request, which is being viewed or executed, by the webservice "view Request".                   | If the value for the parameter is not set, the value "N" will be automatically set by the system. |
| 283 |                                   Service ID of information request about an existing request.                                   |        Y or N       | Enter the identification number (ID) of the service request, which will be used to launch the child request about the information visualization of an already existing request. |                                           Not applicable                                          |

Table 1 - Parameters list

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/09/2019 – Anna Martins
