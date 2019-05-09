+++
title = 'Build an Update Row Source Table'
solution = 'Migration'
+++

# Build an Update Row Source Table

Update Row source tables can be built using SQL AutoGen after targets
have been added and configured in Target Design and an Add Row source
has been assigned to a target.

**NOTE:** The target associated with the source must have a Design
Status of In Design or Design Finished to perform this task.

**NOTE:** Mapping is not required to create a source table. If the
source fields are in System Types, and the source is saved in Target
Design, the source table can be built using SQL AutoGen.

**NOTE:** Source tables cannot be built if the target is in a Design
Status of Complete or Inactive.

SQL AutoGen:

  - Builds a source table

  - Registers it in Transform

  - Builds the CranPort package to import data from the legacy system
    into the source table
    
    <span style="font-weight: bold;">NOTE:</span> An Assemble Where
    Clause can be added in Map to on the *Target Source* page’s vertical
    view. The Assemble Where Clause is used to filter source data when
    importing or refreshing a target.

  - Creates the delete and insert rule

The Update Row source table is created in the data source defined for
the object in Console and is built based on the source database object.
It contains all of the columns from the legacy table, plus zfields used
in update rules and columns needed for check tables.

<span style="font-weight: bold;">NOTE:</span> A user can create all
target tables, source tables, Update Row source tables, and rules at one
time by clicking the Create All Objects icon on the
<span style="font-style: italic;">[Automation](../Page_Desc/Automation_page)</span>
page.

All objects created using SQL AutoGen are written to the data source
defined for the object in Console (Process Area \> Objects \> Vertical
View \> Data Source ID).

The source table name displays in Map on the
<span style="font-style: italic;">[*Target Sources* (Update
Row)](../../Map/Page_Desc/Target_Sources_Update_Row)</span> page’s
*Vertical* View in the ST Table field.

The source table uses the natural keys from the legacy system, so if no
key fields are defined in the legacy table, no keys are defined in the
source table built by SQL AutoGen. zLegacy key fields must be mapped
manually in Map.

If the source table already exists in the database, it will be dropped
and built again.

**NOTE:** A System Type must be defined for a source before the table
can be built. If the user did not import a System Type in Target Design
(for example, an Excel file import, database table import, or manual
entry was used for the target design) an error message displays when the
user clicks the Create Source Table icon. The user must set a System
Type before the table can be created. Add a System Type to a source in
Target Design (Design \> Targets \> Sources \> System Type ID).

To build an Update Row source table in AutoGen:

1.  Click the **Automation** tab in the Quick Panel.

2.  Click the **Sources** icon for a Target.
    
    **NOTE:** The *Automation SQL Target Source* page displays behind
    the *[Automation](../Page_Desc/Automation_page)* page and,
    depending on how the user’s view is configured, may be obstructed by
    the *Automation* page itself.  In this case, to view the
    *[Automation SQL Target
    Source](../Page_Desc/Automation_SQL_Target_Source)* page either
    close the *Automation* page or reduce the size of the *Automation*
    page.

3.  Select the source on the
    <span style="font-style: italic;">[Automation SQL Target
    Source](../Page_Desc/Automation_SQL_Target_Source)</span> page
    in the Parent pane.

4.  Select the Update Row source on the
    <span style="font-style: italic;">[Automation SQL Target Source
    (Update
    Row)](../Page_Desc/Automation_SQL_Target_Source_Update_Row)</span>
    page in the Child pane.

5.  Click the **Create Source table** icon in the Page toolbar; a
    confirmation message displays.

6.  Click **OK**.

<span style="font-weight: bold;">NOTE:</span> Columns can be appended to
all source tables. Refer to [Append Utility Columns to All
Tables](../../Design/Use_Cases/Append_Utility_Columns_to_all_Tables)
for more information.
