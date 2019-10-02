title: Registering user
Description: This feature provides a variety of actions, such as including, changing, and deleting an user. 
# Registering user

In order for the employee to access the system, it's necessary to create a user. By registering it, it's possible that user's data (login and password) are sent to the email of employee. To do this, set parameter 455 indicating the email template (ID) created for this purpose. The email template should contain the keys ${LOGIN} and $ {NEWPASSWORD}.

This feature provides a variety of actions, such as including, changing, and deleting an user.

!!! warning "ATTENTION"

    The sending of login and password, when registering the new user, doesn't include users 
    imported via AD or LDAP.

## Before getting started

To register an user, it's necessary to:

- [X] Register the Employee;

- [X] Have at least an Access Profile;

To send the Login and Password to the Employee's email:

- [X] Configuring parameter 33 and correctly indicating the instance's URL;

- [X] Configuring parameter 455 with the email template ID created to send the access data;

!!! note "EXAMPLE"

    Basic template: "Dear user, here's the access data. Username: ${LOGIN} and Password: ${NEWPASSWORD}"

## Procedure

1.  Access the main menu General Registration \> Personnel Management \> User;

2.  Complete the fields available;

3.  Click on "Save".

!!! info "INFORMATION"

    The system checks if there is an email template for the new employee that has the password key to send via email. The system manager registers or changes an employee login and password on the user screen. The system checks whether: the system uses the password policy and whether the user is LDAP or not. The system allows to enter a new password. After saving, the system sends by email the new data to the employee.


Related
-----------

[Register employee](/en-us/citsmart-7/initial-settings/access-settings/user/register-employee.html)

[Create profile access](/en-us/citsmart-7/initial-settings/access-settings/profile/create-profile-access.html)

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/10/2019 – Larissa Lourenço

