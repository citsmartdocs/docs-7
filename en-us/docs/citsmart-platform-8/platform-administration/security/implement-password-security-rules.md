title: Implement password security rules
Description: Configure passwords of system usage, providing a greater level of security with the usage of different characters.
# Implement password security rules

This functionality portrays the configuration of system usage passwords,
providing a higher level of security with the usage of different characters.

!!! Abstract "ATTENTION"

     This security policy is not available for LDAP users.
     

Default rules when enabling Security Policy:

-   Minimum of 8 characters;

-   At least one lower case letter;

-   At least one uppercase letter;

-   At least a number;

-   At least one special character (symbol);

-   The password cannot be the same as the last 3 passwords used;

-   The password expires in 3 months.

Procedure
------------

1.  Access the main menu System \> Settings \> Policy Settings;

2.  Enable the key "Enable password security policy”;

3.  In the field **Passord force** the manager must define the minimum number
    of password characters (minimum value of 8) and it'll cotain requirements of:
    uppercase letter, lower case, numbers and symbols;

4.  Define the number of previous passwords in which the new one cannot be equal,
    in the limiter **The new password cannot be the same as the previous ones**;

5.  For new users, the password change can be defined by clicking on the key
    “Require password change on first login”

6.  In the field **Password expiration** define the time to expire the password;

7.  For users who are already in operation, it's possible to force the password
    change of the new configuration, from the next login, click on the key "Force
    password change at next login for all users"

8.  Click on "Save”.

!!! Abstract "NOTE"

    The System notifies the user 3 days before the expiration of the current password,
    making this alert through a message in a text box that will appear
    once a day when logging in the System. After the password expires,
    the user is automatically sent to the user profile screen with open
    password exchange panel (you can only use the system again if you
    make a password change).

!!! Abstract "NOTE"

    To change the password, the user can reset the password in two different
    ways, see [Register user][1] and [Edit user account][2].


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/31/2019 - Anna Martins

[1]:/en-us/citsmart-7/initial-settings/access-settings/user/users.html
[2]:/en-us/citsmart-7/initial-settings/access-settings/user/user-data.html
