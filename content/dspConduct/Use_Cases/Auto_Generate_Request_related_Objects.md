+++
title = 'Auto-generate Request-related Objects'
solution = 'Master Data Management'
+++

# Auto-generate Request-related Objects

A Designer can auto-generate a *Request* page and request-related
objects (tables, views and stored procedures) in a Content WebApp and
database if the objects don’t already exist. Once these objects have
been built, users can create and submit a request to dspConduct™ and the
Content WebApp can send data to dspConduct™.

The *Request* page can be customized to meet a client’s business needs,
though the default table and page column definitions meet most
requirements.

**NOTE**: While users can develop their own custom pages, posting pages,
processes, or requests statuses, all custom code must be maintained by
the Designer.

**NOTE**: Auto-generating a *Request* page is an advanced feature. To
use it, a Designer must be familiar with:

  - Working with tables, view, and stored procedures in SQL
  - Working in the DSP to create data sources and WebApps
  - Creating a category in dspConduct™
  - Working with page columns in the DSP®

This section contains the following topics:

  - [Build the Request-related
    Objects](#Build_the_Request-related_Objects)
  - [View the Request Objects Creation
    Log](#View_the_Request_Objects_Creation_Log)
  - [Create Collect Target
Views](#Create_Collect_Target_Views)

## <span id="Build_the_Request-related_Objects"></span>Build the Request-related Objects

A Designer can auto-generate a *Request* page and request-related
objects (tables, views and stored procedures) in a Content WebApp and
database if those objects do not exist. Once these objects have been
built, users can create and submit a request to dspConduct™ and the
Content WebApp can send data to dspConduct™.

**NOTE**: Objects can be built once. After the objects have been built
successfully, there is no method for building them again from within
dspConduct™ or the DSP®. If objects must be rebuilt, they must be
manually updated in the database.

Before performing this task, these prerequisites must have been met:

  - An empty database that will be used for the Content WebApp must
    exist.
  - A data source that uses that database must be registered in the
    DSP®.
  - A WebApp that uses that data source must be added in the DSP®.

Once the prerequisites exist, create a dspConduct™ Category that uses
the WebApp as its Default Web App.

To build the request-related objects:

1.  Click **Vertical View** for the Category.

2.  Click the **Rules and Actions** tab.

3.  Click the **Create Default Web App Request Table and Views** icon.
    
    **NOTE**: The pages that display allow the user to create the
    request-related objects in the WebApp and the database, and this
    icon is active if those objects have not been built. After the
    objects have been built successfully, the Create Default Web App
    Request Table and Views icon is disabled and these pages can no
    longer be accessed.
    
    **NOTE**: These pages display the default ttRequest table and page
    column definitions that will be used when building the objects.
    These default settings can be used to meet most business needs, and
    it is recommended that they not be updated. A user can choose to
    customize or add page column before the request-related objects are
    auto-generated, but all custom code must be maintained by the
    Designer. Refer to the field descriptions for the *[Default Web App
    Request Table
    Columns](../Page_Desc/Default_WebApp_Request_Table_Columns_H)*
    page for information about the type of data to enter in this field
    if needed.
    
    **NOTE**: The auto-generation process creates table columns and page
    columns that are not associated with columns in the underlying
    table. A column is a page column only when the value in the COLUMN
    ORDER field is 0.

4.  Click **Build Objects** in the Page toolbar on the *[Default WebApp
    Request Table](../Page_Desc/Default%20WebApp%20Request%20Table)*
    page to auto-generate the tables, views and stored procedures.

The tables ttRequest, ttRequestOrgUnit1, ttRequestOrgUnit2 and
ttRequestOrgUnit3 are created, along with the following
objects.

|                                                                         |                                                                                                                                                                                      |
| ----------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Object                                                                  | Description                                                                                                                                                                          |
| webDefaultWebAppRequestTable\_BuildObjects\_ztParamIns                  | Creates table ztParam in Content WebApp's database if it doesn't exist already.                                                                                                      |
| webDefaultWebAppRequestTable\_BuildObjects\_DGEViewsIns                 | Creates views in Content WebApp's database; views provide access to DGE tables.                                                                                                      |
| webDefaultWebAppRequestTable\_BuildObjects\_DGEListViewsIns             | Creates views in Content WebApp's database used as List views on Request page.                                                                                                       |
| webDefaultWebAppRequestTable\_BuildObjects\_CreateTablesIns             | Determines if Request-related tables exist in the Content WebApp's database and calls the logic to create them if they don't exist.                                                  |
| webDefaultWebAppRequestTable\_BuildObjects\_ttRequestTriggerIns         | Creates trigger on table ttRequest in the Content WebApp's database if it doesn't exist.                                                                                             |
| webDefaultWebAppRequestTable\_BuildObjects\_OnValidateSubmitViewsIns    | Creates views in the Content WebApp's database used by the Request OnValidate stored procedures and the Submit procedures.                                                           |
| webDefaultWebAppRequestTable\_BuildObjects\_OnValidateProceduresIns     | Creates stored procedures in the Content WebApp's database used by the Request OnValidate event. Also creates stored procedures used by the Request OrgUnit page's OnValidate event. |
| webDefaultWebAppRequestTable\_BuildObjects\_SubmitProceduresIns         | Creates stored procedures in the Content WebApp's database used by the Request Submit event.                                                                                         |
| webDefaultWebAppRequestTable\_BuildObjects\_PageViewsIns                | Creates Request-related page views in the Content WebApp's database.                                                                                                                 |
| webDefaultWebAppRequestTable\_BuildObjects\_CreatePagesIns              | Creates Request-related pages and page events in the Content WebApp.                                                                                                                 |
| webDefaultWebAppRequestTable\_BuildObjects\_RegisterEventRulesIns       | Registers specific procedures to the Request-related pages' events.                                                                                                                  |
| webDefaultWebAppRequestTable\_BuildObjects\_UpdatePagePropertiesUpd     | Registers DCV, PCV to the Request-related pages. Sets Insert, Update, and Support Delete properties.                                                                                 |
| webDefaultWebAppRequestTable\_BuildObjects\_UpdateRequestBuildStatusUpd | Set BuildStatus to true for Request-related ttTable records.                                                                                                                         |
| webDefaultWebAppRequestTable\_BuildObjects\_DefaultViewsCreatedUpd      | After all the Request-related objects have been created, updates ttCategory DefaultWebAppViewsCreated bit to 1.                                                                      |

The following pages are created in the Content WebApp:

  - **\[WebApp name\]** – A static landing page for the Content WebApp
    that displays when the user clicks the WebApp name in the
    *Navigation* pane.
  - **Reports** – A page listing links to custom reports to be developed
    on site.
  - **Request** – A page used by users to enter request data and submit
    it to dspConduct™, created based on the table and page column
    definitions on the *[Default WebApp Request
    Table](../Page_Desc/Default%20WebApp%20Request%20Table)* page
    and the *[Default WebApp Request Table
    Columns](../Page_Desc/Default_WebApp_Request_Table_Columns_H)*
    page.
  - **Request Details** – A page that displays a visual representation
    of an active request’s process through the workflow, including which
    roles have been completed for the request.
  - **Request Org Unit 1 – 3** – If Org Unit Types have been defined for
    the Category, the Organization Unit pages are used to enter Org Unit
    values in addition to values entered on the main Request
page.

## <span id="View_the_Request_Objects_Creation_Log"></span>View the Request Objects Creation Log

This log displays all the log records that are written when the stored
procedures registered to Build Objects execute as the Request-related
objects are created.

There are two ways to access the log.

To access the log at any time:

1.  Click **Design** in the Navigation pane.
2.  Click **Vertical View** for a category.
3.  Click the **Rules and Actions** tab.
4.  Click the **Request Table and Views Creation Log** icon.

The log can also be accessed on the *[Default WebApp Request
Table](../Page_Desc/Default%20WebApp%20Request%20Table)* page by
clicking Creation Log in the Page toolbar. However it is only accessible
on that page until objects are built. Once objects are built and the
user navigates away from the *Default WebApp Request Table* page, that
page is no longer accessible.

**NOTE**: Records remain in the log unless they are manually removed.

**NOTE**: If a Category is deleted, the log records associated with that
Category are also
deleted.

## <span id="Create_Collect_Target_Views"></span>Create Collect Target Views

Tthe Content WebApp must include views that reference the governance
system tables stored in the dg\* database (or another database that
stores the tables). These views are not created when request-related
objects are auto-generated, but can be created automatically using
Collect’s Advanced View Builder feature.

**NOTE**: Using this feature drops and recreates any existing views that
point to these tables created by the Advanced View Builder. Any
modifications that have been made to the views in the Content WebApp
database will be lost every time Build View executes.

To create the target views:

1.  Click **dspConduct \> Design \> Vertical View** for a category.

2.  Click the **Rules and Actions** tab.

3.  Click the **Create Collect Target Views** icon; a confirmation
    message displays.

4.  Click **Ok**.

5.  Select an option from the **DATABASE FOR TABLES** list box.
    
    **NOTE**: This database stores the tables for the governance system.

6.  Click **Save**.

7.  Click the **Build Views** icon on the Page toolbar.

When the process completes, views for all of the tables in dgSAP (or the
selected database) exist in the Content WebApp database.
