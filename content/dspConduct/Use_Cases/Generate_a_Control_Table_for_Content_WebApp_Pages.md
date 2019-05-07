+++
title = 'Generate a Control Table for Content WebApp Pages'
solution = 'Master Data Management'
+++

# Generate a Control Table for Content WebApp Pages

A control table is used to store data to be used as the basis when
dspConduct™ builds a Data Control View (DCV) or a Page Control View
(PCV).

A Designer can create a control table for a scenario \> role \> task
combination. The table is created and stored in the Content WebApp’s
database. If the control table already exists, clicking the Create
Control Table icon in the steps below drops the existing table. When the
table is created, control data for all roles in all scenarios that have
this task assigned is added to the table.

Data stored in the control tables are based on the Content WebApp page’s
column settings for control status (Hide, Enable, Disable) set in
dspConduct™. Refer to [Configure Column Status for a Task for a Scenario
Role Combination](Configure_Column_Status_for_a_Scenario_Role_Task.htm)
for more information.

<span style="font-weight: bold;">NOTE:</span> When a table is generated,
it follows the naming convention \[Control table prefix\]\_\[Page View’s
Root Name\]\_\[variant column name\]. The Control Table Prefix for the
task is set on the <span style="font-style: italic;">[Task
Page](../Page_Desc/Task_Page_H.htm)</span> page’s
<span style="font-style: italic;">Vertical</span> View.

The tables are created with ScenarioID, RoleID, and TaskID as the key
fields, along with the column used for defining the task variant.

**NOTE:** When building a list of scenarios \> roles \> tasks to update
when generating control tables, the rules that build the control tables
look for every task that has the same page and then updates the column
information and inserts data for every scenario and role that have any
of those tasks.

<span style="font-weight: bold;">NOTE:</span> If multiple pages use the
same table, dspConduct™ builds different control tables for each page.

<span style="font-weight: bold;">NOTE:</span> Refer to [Create Tables
and Views for Content WebApp Pages
Overview](Create_Tables_and_Views_for_Content_WebApp_Pages_Overview.htm)
for general information.

To create a control table:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Scenarios</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    scenario.

4.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    role.

5.  Click the <span style="font-weight: bold;">Pages</span> icon for a
    scenario \> role \> task combination.

6.  Select one or more page records, and then click the
    <span style="font-weight: bold;">Create Control Table </span>icon in
    the Page toolbar.
    
    **NOTE:** Use discretion when selecting multiple records for
    processing because there can be system limitations on how many
    tables are processed simultaneously.

Continue with [Generate Control Views for Content WebApp
Pages](Generate_Control_Views_for_Content_WebApp_Pages.htm).
