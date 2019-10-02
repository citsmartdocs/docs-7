title: Using Smart Analytcs (BI) to generate reports
Description: Analyze data in your instance where you can elaborate countless possibilities of graphs, panels and tables with measurable data information.
# Using Smart Analytics (BI) to generate reports

According to Wikipedia, Business Inteligence "comprises the strategies and 
technologies used by enterprises for the data analysis of business information. 
BI technologies provide historical, current and predictive views of business 
operations".

CITSmart Analytics is the BI solution for CITSmart data analysis.
With this feature you can create numerous graphs, dashboards and tables with
data information registered in the instance.

Before getting started
----------------

It's necessary to have the BI application installed, configured, and communicable 
with your CITSmart instance.

Procedure
------------

1.  Access the main menu \> Reports \> Smart Analytics \> Smart Analytics;

2.  Select one potion in the tab **Cubes** (default: Change Requests, Releases,
    Tickets);

3.  In the tab **Measures** select a type of measure to use in the report, when
    click on  it, it'll be added to the field **Measure** of the dashboard;


    !!! Abstract "NOTE"

        It's possible to elaborate a new type of measurement, by clicking on the "Add" button and elaborating a new formula.
        
    
1.  In the tab **Dimensions**, it's available the options that will serve as a database
    of the report. Select and drag an option into one of the boxes of measurements and 
    dimensions on the dashboard: Columns, Rows and Filters;

2.  On the right side of the dashboard you can configure the report in several table and chart formats;

3.  To change the position of the measurement units in the tabl/graph, click on the detail button available in each dashboard      measurement box;

4.  To export the report, click on "Export" and select the format (PNG and PDF);

5.  After finish the report, click on “Save query”.



### Units available

|             Dimension           |                                      Objective                                    |
|:-------------------------------:|:---------------------------------------------------------------------------------:|
|             Activity            |            It presents the activities that were created within the instance       |
|               Date              |          It makes available day, month, year, bimester, quarter, semester         |
|          Executor group         |                        Group Code/ID, name of executor group                      |
|           Group Solver          |                           Code/ID, name of solver group                           |
|             Locality            |                        It present the location of requester                       |
|             Priority            |                          It presents the ticket priority                          |
|            Requester            |                         It presents the name of requester                         |
|           Responsible           |                          It presents the name of responsible                      |
|            SLA Status           |                               It presents SLA status                              |
|    Service Level   Agreement    |                              It presents code/ID and SLA                          |
|              Source             |                      It presents the source of the attendance                     |
|            Technical            |                          It presents the technical name                           |
|          Ticket Status          |                     It present the code/ID and ticket status                      |
|              Unity              |                   It presents code/ID and the unit of the requester               |



Related
-----------

[Configure BI solution (Smart Analytics) via Docker](/en-us/citsmart-7/additional-features/smart-analytics/install-bi-docker.html)


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>02/28/2019 – Anna Martins
