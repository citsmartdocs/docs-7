title: Configure service to change password
Description: Changing the user password is one of the possibilities allowed by the system.  
# Configure service to change password

The alternative to change users password is one of the possibilities released by the system. To configure this option, it's necessary to follow the procedures described here.

!!! Abstract "NOTE"

    This option is only available for manual account authentication.

Before getting started
----------------

It's necessary to first have a functional e-mail service (SMTP), since the sending of the password is done via e-mail.

Procedure
------------

*1st Step: Create an email template for changing the password*

1.  Access the main menu System \> Settings \> Email Template;

2.  Create an email template to change the password;

    !!! Abstract "NOTE"

        In order for the user to receive the new access information, it's necessary to use, in the e-mail message, the key                      ‘${NOVASENHA}’ (for example, the key about the "New password”). In addition, you can also send the user login using the key              ‘${LOGIN}’ (for example, the key about the“Login”). 
        

*2nd Step: Set the parameter about the service to change the password*

1.  Access the main menu Parametrization \> CITSmart Parameters;

2.  Edit and save parameter 116 by assigning the numeric value of the ID generated for the newly created e-mail template;

What to do next
------------------

To test the service to change the password, access the login page, click on "Forgot your password?", enter a local user login and click on "Save".

## Related

[Create E-mail Template][1]

[Configure E-mail Account][2]

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/21/2019 – Larissa Lourenço

[1]:/en-us/citsmart-7/platform-administration/email-settings/email-templates-configure-email-template.html
[2]:/en-us/citsmart-7/platform-administration/email-settings/configuration.html
