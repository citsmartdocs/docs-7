title: Configure parametrization - work order
Description: Allows to define the calculation formula of the work order gloss, enable custom signatures in the Work Orders report, within other viable actions.
# Configure parametrization - work order

Work order is a document that will give the permission to the relative execution
of a service. The "Work order" parametrization allows to define the calculation
formula of the work order gloss, enable custom signatures in the Work Orders
report, within other viable actions.

Procedure
-------------

1.  Access the functionality through the main menu Parametrization \> Work Order
    (WO);

2.  Define the parameters value (attributes);

3.  Click on "Save";

4.  The list below presents the "Work order" parameters and the purpose of each
    one of them:

|  #  |                                      Name                                      |   Possible Values   |                                                                                                                                                                              Purpose                                                                                                                                                                             |                                                                Additional Guidance                                                               |
|:---:|:------------------------------------------------------------------------------:|:-------------------:|:----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------:|:------------------------------------------------------------------------------------------------------------------------------------------------:|
|  51 |                         WO GLOSS FORMULA - Default Code                        |                     |                                                                                                                                 Define the Work Order Calculation formula. By default the formula is already defined in the tool.                                                                                                                                |                                                                  Not applicable                                                                  |
| 130 | It allows Work Order listing with retroactive date (Eg: Y or N - Default: 'N') | Y or N (Default: N) |                                                                                                                                           Define whether to allow the listing of a Work Order with a retroactive date.                                                                                                                                           |                               If you do not enter the parameter value, the system default value will be used: "N".                               |
| 229 |               Reset Activity Formulas (Eg: Y or N - Default: 'Y')              | Y or N (Default: Y) | Change the formula structure of the activities already registered to the new structure that is configurable from the WO Formula screen. When reporting the default value of "Y", the system will execute the activity formula reset routine at the time JBoss restarts on a CITSmart system update, and assigns "N" to this parameter at the time it's finished. | Once the "Y" value has been entered, the contract activity formula, not yet configured, will be in accordance with the new WO Formula structure. |
| 243 |              Allow custom subscriptions in the Work Orders report              |                     |                                                    Enable signatures to be used for printing the Work Order reports. When the parameter is enabled (value = Y), the system displays a field in the Work Order form, and you can choose which signature frame configuration to use when printing your reports.                                                    |                        When enabled, it forces the user to define and configure one more field before saving a Work Order.                       |

Table 1 - Parameters list

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/09/2019 – Anna Martins
