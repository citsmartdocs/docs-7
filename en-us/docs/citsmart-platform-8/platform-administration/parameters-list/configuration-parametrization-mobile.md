title:Configuration parametrization - mobile
Description: Configure and customize to adequate the scenario about the mobile application usage.
# Configuration parametrization - mobile

The "Mobile" parametrization has the purpose of configure and customize to adequate the scenario about the mobile application usage (for example, CITSmart GO).

Procedure
-------------

1.  Access the functionality through the main menu Parametrization \> Mobile;

2.  Define the parameters value (attributes);

3.  Click on "Save";

4.  The list below presents the "Mobile" parameters and the purpose of each one
    of them:

|  #  |                                                               Name                                                              |   Possible Values   |                                                                                                                             Purpose                                                                                                                             | Additional Guidance |
|:---:|:-------------------------------------------------------------------------------------------------------------------------------:|:-------------------:|:---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:-------------------:|
| 255 |                                 Range of Action/View of attendant in the Mobile - (Default: 30)                                 |                     |                                                     Define the radius of action of an attendant, used in APP mobile. Define the maximum radius of service for requests that are in a "Non-Directed" status.                                                     |    Not applicable   |
| 256 |                        Interval (in minutes) of time for reporting the Attendant position - (Default: 10)                       |                     |                                                                     Define the interval that the Mobile application should report to the server the geographic positioning of the attendant.                                                                    |    Not applicable   |
| 257 |                                    Page size for return in paged REST services (Default: 10)                                    |                     |                                                                                     Define the amount of registries returned in the list of services consumed by the Mobile.                                                                                    |    Not applicable   |
| 258 |                                     Maximum interval of days for consultation (Default: 30)                                     |                     |                                                                                Define maximum query range restriction on the screens, initially used in service force management.                                                                               |    Not applicable   |
| 267 |                                  Page size for return on REST V1 mobile services (Default: 200)                                 |                     |                                                                                                          Set the page size to return in REST services.                                                                                                          |    Not applicable   |
| 272 | Determine whether you will only be notified of requests without responsible in Citsmart Mobile. Values: "Y" or "N" Default: "N" | Y or N (Default: N) | Define which requests can be notified to the user. If the value of the parameter is "Y", only the notifications of requests without current attendant will be displayed. If the value of the parameter is "N", notifications of all requests will be displayed. |    Not applicable   |
| 284 |                           Default contract ID for creating new incidents/requests in Citsmart Mobile.                           |                     |                                                                           Enter the identification number (ID) of the contract to perform the opening of service requests via mobile.                                                                           |    Not applicable   |
| 285 |                        Default service ID for service requests and incidents created in Citsmart Mobile.                        |                     |                                                                      Enter the service identification number (ID) that will be the default for registration of service requests via mobile.                                                                     |    Not applicable   |
| 286 |                         Default source ID for service requests and incidents created in Citsmart Mobile.                        |                     |                                                                                Enter the identification number (ID) of the default origin to open the service request via mobile.                                                                               |    Not applicable   |
| 350 |                                          Enable sending notifications to mobile devices                                         | Y or N (Default: N) |                                                                                   It allows to control whether system notifications will be sent to mobile devices (general).                                                                                   |    Not applicable   |
| 352 |                              Enables sending notifications to mobile devices when creating requests                             | Y or N (Default: N) |                                                                                   It allows to control whether system notifications will be sent to mobile devices (general).                                                                                   |    Not applicable   |
| 353 |                        Enables sending mobile notifications while updating requests reporting close calls                       | Y or N (Default: N) |                                                                                   It allows to control whether system notifications will be sent to mobile devices (general).                                                                                   |    Not applicable   |

Table 1 - Parameters list

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/07/2019 – Anna Martins
