# <span id="Category_H"></span>Category H

[Category V](#Category_V)

<div class="use">

Use this page to:

  - [Create a Category](../Use_Cases/Create_a_Category.htm)
  - [Set Up a Category from IGC™ in
    dspConduct™](../Use_Cases/Set_Up_a_Category_from_IGC_in_dspConduct.htm)

</div>

To access this page, select **dspConduct \>Design** in the *Navigation*
pane.

**NOTE**: If a category was imported from IGC™, data that was entered in
IGC™ cannot be updated from within dspConduct™, and many of the fields
and icons associated with the record are not active for that category.
Refer to [Update Custom Attributes for Governance
Elements](../Use_Cases/Update_Custom_Attributes_for_Governance_Elements.htm)
for more information.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>From IGC</p></td>
<td><p>Displays to indicate that the category was created in IGC™. If no icon displays the category was created in dspConduct™.</p>
<p>This column displays after the IGC™ parameters are configured in Common on initial install. Refer to the <em>BackOffice Associates® Installation and Upgrade Manual</em> for more information.</p>
<p><strong>NOTE</strong>: Data entered in IGC™ cannot be updated from within dspConduct™.</p>
<p><strong>NOTE</strong>: Records that come from IGC™ cannot be deleted.</p>
<p><strong>NOTE</strong>: When importing a category from IGC™, if there is a category in dspConduct™ that has the same name, the IGC™ category is automatically mapped to the dspConduct™ category. If more than one dspConduct™ category has the same name in the database, the IGC™ category is mapped to the category with the earliest Added On date. All Business Processes, Scenarios and Roles coming from the IGC™ will be created as new elements in the matched category. A process Designer can then map dspConduct™ tasks to the IGC™ tasks.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the name of the category .A category is a collection of governance elements and is used for organizational purposes.</p>
<p>The category name cannot be duplicated.</p></td>
</tr>
<tr class="even">
<td><p>DEFAULT WEB APP ID</p></td>
<td><p>Displays the DEFAULT WEB APP ID for the Content WebApp of the selected category.</p>
<p>The field is limited to the applications for which the user has a BOA Tools license and has the ability to change. These applications are not delivered.</p>
<p><strong>NOTE:</strong> A specific Default WebAppID may only be assigned to one category. A validation message is received if a WebApp has already been assigned to another category.</p>
<p><strong>NOTE</strong>: If a category is imported from IGC™, it must have a default WebApp assigned to it or the category is invalid. Refer to <a href="../Use_Cases/Set_Up_a_Category_from_IGC_in_dspConduct.htm">Set Up a Category from IGC™ in dspConduct™</a> for more information. .</p></td>
</tr>
<tr class="odd">
<td><p>WEB APP STATUS</p></td>
<td><p>Indicates whether a category has a WebApp assigned and whether the tasks created in that category in IGC™ have been assigned to pages created in the Content WebApp.</p>
<p>A WebApp must be assigned to a category imported from IGC™.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the description of the category.</p></td>
</tr>
<tr class="odd">
<td><p>IGC Tasks</p></td>
<td><p>Click to open the IGC™ <em><a href="IGC_Task.htm"><em>Task</em></a></em> page to map a dspConduct™ task to an IGC™ task.</p>
<p><strong>NOTE</strong>: This icon is disabled if the category did not come from IGC™.</p>
<p>Refer to <a href="../Use_Cases/Map_a_dspConduct_Task_to_a_Task_Imported_from_IGC.htm#Map_an_IGC_Task_to_An_Existing_dspConduct_Task">Map an IGC™ Task to An Existing dspConduct™ Task</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Tasks</p></td>
<td><p>Click to open the <a href="Task_H.htm">Task</a> page to add tasks at the category level. Refer to <a href="../Use_Cases/Add_a_Task.htm">Add a Task</a> for more information.</p>
<p>The value on the Tasks icon indicates the number (record count) of tasks that have been developed for the selected category. When a category is created, this number is 0 which indicates no tasks have been developed.</p></td>
</tr>
<tr class="odd">
<td><p>Roles</p></td>
<td><p>Click to open the <a href="Role_H_dspConduct.htm">Role</a> page to add roles at the category level. Refer to <a href="../Use_Cases/Add_a_Role.htm">Add a Role in dspConduct™</a> for more information.</p>
<p>The value on the Roles icon indicates the number (record count) of Roles that have been developed for the selected category. Refer to <span class="underline"><span style="color: #548DD4;"><a href="../Use_Cases/Manage_Roles.htm">Manage Roles</a></span></span> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Scenarios</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Scenario_H.htm">Scenario</a></span> page to add a scenario at the category level. Refer to <a href="../Use_Cases/Add_Scenario.htm">Add a Scenario</a> for more information.</p>
<p>The value on the Scenarios icon indicates the number (record count) of scenarios that have been developed for the selected category. When a category is created, this number is 0 which indicates no scenarios have been developed.</p></td>
</tr>
<tr class="odd">
<td><p>Business Processes</p></td>
<td><p>Click to open the <a href="Business_Process_H.htm">Business Process</a> page to add business processes at the category level. Refer to <a href="../Use_Cases/Add_Business_Process.htm">Add a Business Process</a> for more information.</p>
<p>The value on the Business Processes icon indicates the number (record count) of business processes that have been developed for the selected category. When a category is created, this number is 0 which indicates no business processes have been developed.</p></td>
</tr>
</tbody>
</table>

## <span id="Category_V"></span>Category V

[Category H](#Category_H)

This page has the following tabs:

  - [General tab](#General_Tab)
  - [Rules and Actions tab](#Rules_and_Actions_tab)
  - [Metrics tab](#Metrics_Tab)

### <span id="General_Tab"></span>General tab

Field

Description

Name

Displays the name of the category. A category is a collection of
governance elements and is used for organizational purposes.

Default Web App ID

Displays the Content WebApp of the selected category.

The field is limited to the applications for which the user has a BOA
Tools license and has the ability to change. These applications are not
delivered.

**NOTE:** A specific Default WebAppID may only be assigned to one
category.

Request Page Id

Displays the name of the Content WebApp and the name of the page created
in the Content WebApp to enter request data.

The page entered here displays when the user clicks the Content Request
Page icon on the
<span style="font-style: italic;">[Request](Request.htm)</span> page.

If no value is entered, when the user clicks the Content Request Page
icon on the <span style="font-style: italic;">Request</span> page, a
page does not open.

Description

Displays the description of the category.

Owner

Displays the owner of the category. This person(s) is responsible for
the category.They have no approval authority at the category level but
owners at the category level are automatically assigned as owners for
each governance element created in the category.

**NOTE:** The list is limited to those users with an email address in
the DSP®.

**NOTE:** Once the owner is assigned, the child elements will inherit
the category owner as a default if another owner is not assigned.

Comment

Displays additional commentary about the category.

Configuration

Org Unit Types

Click to open the <span style="font-style: italic;">[Category Org Unit
Type](Category_Org_Unit_Type.htm)</span> page to assign org unit types
to a category object.

Request Status Params

Click to open the <span style="font-style: italic;">[Category Request
Status](Category_Request_Status.htm)</span> page. This page lists the
<span id="Request Status dspConduct" class="popUpLink">\>request
statuses</span> and the number of days a request remains within the
request page until being archived.

Workflow Messages

Click to open the <span style="font-style: italic;">[Category Workflow
Message](Category_Workflow_Message.htm)</span> page to create workflow
messages in different languages. Refer to [Create Language-specific
Workflow Messages for a
Category](../Config/Create_Language-specific_Workflow_Messages_for_a_Category.htm)
for more information.

Posting Processes

Click to open the [Category Process](Category_Process.htm) page to set
the allowed Integrate processes for the scenarios in this category.

**NOTE:** The count on the icon represents the number of category
processes registered to the category.

Control Table Prefix

Displays the prefix to the table name when a table is generated for a
scenario \> role \> task combination for the category. When a table is
generated for the control views or required validations, the table name
starts with this configured text.

For example, a user can enter the prefix "ttSRTC\_" and all control
tables for the category are generated with that prefix. Refer to [Create
Tables and Views for Content WebApp
Pages](../Use_Cases/Create_Tables_and_Views_for_Content_WebApp_Pages_Overview.htm)
for more information.

Data-Driven Dependency Conditions

Condition Table Datasource Id

Displays the data source that contains the tables and fields to be
evaluated for conditions. The data source used by the category’s Content
WebApp is used by default.

Conditions

Click to open the
<span style="font-style: italic;">[Conditions](Conditions.htm)</span>
page to identify conditions to be met in the data that determine whether
a scenario or role is available within a business process. Refer to [Add
Data-Driven Dependency Conditions to a
Category](../Use_Cases/Add_Data_Driven_Dependency_Conditions.htm) for
more information.

The count on the icon is the total number of conditions for the selected
category.

### <span id="Rules_and_Actions_tab"></span>Rules and Actions tab

<div class="use">

Use this tab to [Auto-generate Request-related
Objects](../Use_Cases/Auto_Generate_Request_related_Objects.htm).

</div>

Field

Description

Actions

Refresh Column List For All Variants

Click to update the Scenario Role Task Column lists in this category.
Columns that have been added in the Content WebApp are added to the
lists, and columns that have been removed from the Content WebApp are
removed. No columns are updated.

**NOTE:** This option only adds and removes column settings. Existing
settings are not changed.

Rules

Default Value Rules

Click to open the *[Default Value Rules](Default_Value_Rules.htm)* page
to add a default value rule to indicate a default value for a column.

The count on the icon is the total number of Default Value Rules for the
selected category.

Refer [Add a Scenario Level Default Value Rule to a
Category](../Use_Cases/Add_a_Scenario_Level_Default_Value_Rule_to_a_Category.htm)<span style="background: #ffffff;">for
more information.</span>

Review Role Configuration

Audit Datasource Id

Displays the Default WebApp ID audit data source for the category. This
data source must have auditing enabled.

**NOTE:** The Default WebApp ID audit data source is the only valid data
source and may be different than the Default WebApp ID’s data source.

Table Registration

Click to open the [Audit Table
Registration](Audit_Table_Registration.htm) page to configure tables and
columns to be audited for changes to the data in the tables. The Review
role views a list of these changes while reviewing requests.

Purge Aggregate Table

Click to delete all review role audit records from the aggregate table
for the current category.

**NOTE:** Use this option if mistakes were made during configuration
(e.g., a column was incorrectly disabled during the import) and the data
must be imported again.

Default Web App Configuration

Create Default Web App Request Table and Views

Click to open the *[Default Web App Request
Table](Default%20WebApp%20Request%20Table.htm)* page and the *[Default
Web App Request Table
Columns](Default_WebApp_Request_Table_Columns_H.htm)* page to
auto-generate request-related objects in the Content WebApp and the
database.

**NOTE**: This icon is active if those objects have not been built.
After the objects have been built successfully (when the user clicks the
Build Object icon on the *Default Web App Request Table* page), the
Create Default Web App Request Table and Views icon is disabled.

Refer to [Auto-generate Request-related
Objects](../Use_Cases/Auto_Generate_Request_related_Objects.htm) for
more information.

Request Table and Views Creation Log

Click to open the [Request Objects Creation
Log](Request_Objects_Creation_Log.htm) page to view records for the
objects created during the auto-generation process.

Refer to [View the Request Objects Creation
Log](../Use_Cases/Auto_Generate_Request_related_Objects.htm#View_the_Request_Objects_Creation_Log)
for more information.

Create Collect Target Views

Click to open the *[Advanced View
Builder](../../../Platform/Collect/Page_Desc/Advanced_View_Builder_H.htm)*
page in Collect to build views in the Content WebApp database for the
tables in any new dg\* database (or another database that stores
governance system tables).

Refer to [Create Collect Target
Views](../Use_Cases/Auto_Generate_Request_related_Objects.htm#Create_Collect_Target_Views)
for more information.

### <span id="Metrics_Tab"></span>Metrics tab

Field

Description

Duration

Duration Business Process

Click to open the [Business Process Request
Duration](Busniess_Process_Request_Duration.htm) chart.

Duration Scenario

Click to open the [Scenario Request
Duration](Scenario_Request_Duration.htm) chart.

Duration Role

Click to open the [Role Request Duration](Role_Request_Duration.htm)
chart.

SLA Percent On Time

SLA Business Process

Click to open the [SLA Percent On Time by Business
Process](SLA_Percent_OnTime_by_Business_Process.htm) chart.

SLA Scenario

Click to open the [SLA Percent On Time by
Scenario](SLA_Percent_On_Time_by_Scenario.htm) chart.

SLA Role

Click to open the [SLA Percent On Time by
Role](SLA_Percent_On_Time_by_Role.htm) chart.

Predictive

Predictive Business Process

Click to open [Business Process
Predictive](Business_Process_Predict.htm) chart.

Predictive Scenario

Click to open the [Scenario Predictive](Scenario_Predictive.htm) chart.

Predictive Role

Click to open the [Role Predictive](Role_Predictive.htm) chart.

Requests

Active Requests

Click to open the [Active Request for
Category](../Use_Cases/Active_Request_Category.htm) chart to view the
number of requests by
<span id="Request Status dspConduct" class="popUpLink">status</span> in
a category.
