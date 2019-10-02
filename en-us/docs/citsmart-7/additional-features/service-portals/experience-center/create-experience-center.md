title: Creating experience center
Description: This feature provides a variety of actions, such as including, changing, and deleting the Experience Center.
# Creating experience center

Creation is the process of designing and providing the Experience Centers (EC) in CITSmart. In this document, it's presented the interface features that enable the registration, change, deletion, import and export of EC.

## Before getting started

- [X] To create an experience center, it's necessary to have permission in the access profile.

!!! abstract "NOTE"
    
    Some widgets depend on information entered in other features, for example, knowledge, surveys, services, notifications, and others. Therefore, it's necessary to structure this information for possible use within the EC.

## Procedure

1. To access the Experience Center functionality, access the menu **Experience Center** > Experience Center Configuration > **New**.

### Information

2. In the "Information" tab, complete the fields available;

![information Experience Center CITSmart][1]

**1: Change** – icon of Experience Center;

**2: Title** – that will be presented for the user of Experience Center;

**3: Status** – of the Experience Center (“Active” or “Inactive”);

**4: Type** - it's possible to view the options *Main* showing the Experience Center created to be primary, and *Link* showing the ones that were created to be linked to some primary EC;

**5: Description** – text that will follow with the title for the presentation of the Experience Center to the user.

### Permissions

3. On the Permissions tab, define the groups that will be able to view the Experience Center;

![Permission Experience Center CITSmart][2]

### Construction

4. On the Construction tab, it's possible to visually customize the Experience Center, besides the possibility create sections and add Widgets, links and linking other Experience Centers:

#### Visual Customization

5. By using these tools, you can customize the Experience Center view

- **Change logo** – Allows to change the EC logo. Recommended size:

- **Change header** – Allows to change the EC header image. Recommended size:

- **Reset structure** – Allows to set the whole structure as if it were the first access, removing all changes;

- **Grid style** – Allows to change how to visualize the Experience Center,

    - Fixed Width: Keeps the EC fixed at center of screen;

    - Full Width: Leaves the EC completely distributed in the size of your browser;

- **Logo size** – Allows to increase the logo size up to 100% of its original size.

- **Theme color** – Allows to change the color of the drop down menu (using colors in code, e.g.: # 777)

- **Menu icon** – Allows to change the color of menu sections, links, and icons (using colors in code, e.g.: # 777)

!!! warning "ATTENTION"
    
    The "Reset Structure" button is irreversible after saving the change, if you have not *saved*, just press the back button and nothing will be changed.

#### Desing Area

In the design area you can build the content that will be published in the Experience Center.

6. Set the type of navigation (with or without menu);

7. Create sections for the navigation tree (only for navigation with menus); 

8. Add menu item, at end of section, by clicking on "+";

9. Configure the menu content, by clicking on the key icon;

10. Select the type of content (Widget, link or Experience Center);


**Type: Widget**

1. Select the size for the content area, by clicking on "+" and choosing an option;

!!! example "EXAMPLE"

    100%, 50% x 50%, 33,3% x 33,3% x 33,3%, 33,3% x 65,6%, 65,6% x 33,3% e 25% x 25% x 25% x 25%.

2. Select the Widget, by clicking on "=+" and choosing an option;

3. Click on save.

- After selecting a layout, it's possible to choose CITSmart functions as Widgets (See Widgets table);

!!! note "NOTE"

    - Do you want to set this page as home when you first open the experience center? - has the function of making this menu the main page of your Experience Center.
    - Inherit Experience Center Groups - allows to select which groups will be allowed to this menu, the groups that are available for management are the groups that have permission on the “Permissions” tab;

**Type: Link**

1. When selecting the item link, enter a URL to direct the user when they click on the menu item;  

2. Click on save.

**Type: Experience Center**

1. Allows to link another Experience Center (Type: Link) to the main one. Click on the search field and the registered EC will be listed, select one. It's also possible to type the name to find it.

2. Click on save.


#### Positioning of Elements and Widgets

**Cabeçalho fixo**

![header Experience Center CITSmart][3]

 **1: Menu** – with it you can access other Experience Centers to which you have permission;

**2: Logo** – selected by the user for a better EC customization;

**3: Search bar** - perform an universal search that will return Knowledge and Activities that the user can select;

**4: Profile options** – allows you to change the language, edit the profile, logout and access the system

**Experience Center with navigation**

This structure allows the creation of an Experience Center with a left navigation menu tree.

**Experience Center without navigation**

This structure allows the creation of an experience center using only widgets.

**Widgets Available**

|**Name**|**Type**|**Objective**|
|:----------------------:|:-------------:|:--------------------------------:|
|News| General | Displays knowledge of type "News”. |
|Notification| General | Displays Systems notifications. |
|Searches| General |Allows to view active campaigns|
|Youtube| General |Allows to incorporate videos from Youtube|
|Image| General | Enters image |
|Slide Show| General | Displays slide show of type carrossel. |
|Divider| General | Inserts horizontal line on page. |
|Spacer| General | Inserts space between one widget and another. |
|Text| General | Inserts a text with several formats. |
|List| General | Inserts the list of links. |
|Menu| General | Allows to view the menu of CITSmart. |
||||
|Knowledge center| Knowledge| Generates a button that directs to the Knowledge Center|
|Knowledge| Knowledge| Allows to insert existing documents into the knowledge base|
|Favorites| Knowledge| Allows to list all documents classified as favorites in the User's Guide|
|Indicated| Knowledge| Allows to list all documents listed in the User's Guide|
|Liked| Knowledge| Allows to list all documents liked in the User's Guide|
||||
|My services | Requests| Allows to open a ticket through the Experience Center|
|My tickets | Requests| Allows to view the list of tickets opened by the user logged|
||||
|Simple | Simple Agile Management | Allows to view the workspaces of the functionality Simple |
||||
|Smart Chat | Communication | Allows to enter a logo for this submenu |
|Call | Communication | Allows to enter the logo for this submenu |
||||
|My Worksplaces | Smart Decision | Allows to search for reports within the Smart Decisions |
||||
| Experience Center | Experience Center |Allows to enter other experience center|

## What to do next

- In the upper area, click on "Preview" to view the created Experiment Center. After finishing the EC, publish it so that your organization can take full advantage of it.
- Click on "Export" to download the json format Experience Center.


## Related

[Register satisfaction survey](/en-us/citsmart-7/processes/portfolio-and-catalog/configuration/register-satisfaction-survey.html)

[Register a service](/en-us/citsmart-7/processes/portfolio-and-catalog/use/register-a-service.html)

[Create knowledge](/en-us/citsmart-7/processes/knowledge/use/create-knowledge.html)

<i class='fa fa-youtube-play  fa-2x' style='color:#97ce17;vertical-align: middle;'> </i> [Video Library](https://www.youtube.com/playlist?list=PLB5qK2uzf2RPrJlfrg8kcSk7iorkZwCWq)'


!!! tip "About"

    <b>Product/Version:</b> CITSmart | 7.00 &nbsp;&nbsp;
    <b>Updated:</b>01/04/2019 – Larissa Lourenço

[1]:images/creat-experience-center.png
[2]:images/permission-experience-center.png
[3]:images/header-experience-center.png
