title: Notify responsible for the knowledge expiration
Description: Configure the e-mail notification to notify the responsible (creator and publisher) about the expiration of knowledge.
# Notify responsible for the knowledge expiration

This knowledge is intended to configure the e-mail notification to notify the
responsible (creator and publisher) about the expiration of knowledge.

Before getting started
--------------------------

It's necessary to have at least one knowledge registered in the knowledge base.

Procedure
-------------

1.  Configure the parameter 78 with the amount of the days previous to the
    knowledge expiration, which is intended to notify the responsible for the
    knowledge;

2.  Create a routine for the batch processing notification:

    -   Access the functionality through the main menu System \> Batch
        Processing and click on "New";

    -   Define the routine description, select the type "Java Class" and put the
        situation as "Active";

    -   Select the appointment as "Daily" and indicate the time in with will be
        processed the routine;

    -   In the area "Content", copy the script below:

        -   br.com.centralit.citcorpore.quartz.job.VerificaValidadeBaseConhecimento

    -   Click on "Save".

3.  If you want, it's possible to customize the email template. Just access the
    functionality through the main menu System \> Settings \> Email template,
    select the email template with ID = "7" and make the change.

Related
-------

[Configure parametrization - knowledge](/en-us/citsmart-7/platform-administration/parameters-list/configure-parametrization-knowledge.html)

[Create knowledge](/en-us/citsmart-7/processes/knowledge/use/create-knowledge.html)


<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2ROOaL7DsS86sLx4ilNgruEc)'

!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/04/2019 - Anna Martins
