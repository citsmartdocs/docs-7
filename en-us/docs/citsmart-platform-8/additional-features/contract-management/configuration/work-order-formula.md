title: Register work order (WO) formula
Description:Is intended to register the client formulas to configure "how" will be the calculation of the total cost value of the contract service activity.
# Register work order (WO) formula

This functionality is intended to register the client formulas to configure "how" will be the calculation of the total cost value of the contract service activity.

Procedure
-------------

1.  Access the functionality through the main menu Integrated Management \>
    Contract Management \> WO Formula;

2.  In the tab "**Formula Registration**", it's necessary to complete the field
    necessary. When informing the formula options, remember that the purpose of
    each variable available to describe the formula:

    |   **Variable**  | **Description** |                                                                  **Purpose**                                                                  |
    |:---------------:|:---------------:|:----------------------------------------------------------------------------------------------  -----------------------------------------------:|
    |      vValor     |      Value      |                           Allows the user to enter a value that will be used to calculate the value of the activity                           |
    |    vDiasUteis   |   Working days  | Allows the return of the number of business days between the start date and the end date of the service order based on the contract schedule. |
    |  vDiasCorridos  |   Running days  |                                  Amount of days between the start date and the end date of the service order.                                 |
    | vNumeroUsuarios | Number of users |                                         Allows you to return the number of active users on the system.                                        |
    |  vComplexidade  |    Complexity   |       Based on the complexity chosen by the user, the system will return its corresponding value entered on the contract record screen.       |

3.  After describe the formula, click on "View Formula". This button represents
    the validation of the formula and where the calculation process is
    presented, transforming the formula text into a mathematical expression and
    returning its calculated result, after clicking on "Simulate". Remember that
    it's possible to use the "{}" keys to delimit a text that you wish to
    include in the formula, where it will not influence the calculation of the
    value of the activity;

4.  Click on "Save". But, before save the formula, the system should validate
    the syntax and only allow the saving if is correct.

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROEeoHh3EbsZJxjr9hJSLIV)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/07/2019 – Larissa Lourenço
