# Build Source Tables

Source tables can be built using SQL AutoGen after targets have been
added and configured in Target Design and a source has been assigned to
a target.

<span style="font-weight: bold;">NOTE:</span> The target associated with
the source must have a Design Status of In Design or Design Finished to
perform this task.

<span style="font-weight: bold;">NOTE:</span> Mapping is not required to
create a source table. If the source fields are in System Types, and the
source is saved in Target Design, the source table can be built using
SQL AutoGen.

<span style="font-weight: bold;">NOTE:</span> Source tables cannot be
built if the target is in a Design Status of Complete or Inactive.

SQL AutoGen:

  - Builds a source table

  - Registers it in Transform

  - Builds the CranPort package to import data from the legacy system
    into the source table
    
    <span style="font-weight: bold;">NOTE:</span> An Assemble Where
    Clause can be added in Map on the
    <span style="font-style: italic;">Target Sources</span> page’s
    vertical view. The Assemble Where Clause is used to filter source
    data when importing or refreshing a target.

  - Creates the delete and insert rule

The source table is created in the data source defined for the object in
Console and is built based on the source database object. It contains
all of the columns from the legacy table, plus zfields used in update
rules and columns needed for check tables.

<span style="font-weight: bold;">NOTE:</span> If Source Active On Build
is enabled on the Parameters page in Console, target sources are
auto-generated with a default status of active in Transform.  If
disabled target sources are auto-generated with a default status of
inactive in Transform.

<span style="font-weight: bold;">NOTE</span>: A user can create all
target tables, source tables, Update Row source tables, and rules at one
time by clicking the Create All Objects icon on the
<span style="font-style: italic;">[Automation](../Page_Desc/Automation_page.htm)</span>
page.

All objects created using SQL AutoGen are written to the data source
defined for the object in Console (Process Area \> Objects \> Vertical
View \> Data Source ID).

The source table name displays in Map on the *Target Sources* page’s
*Vertical* View in the ST Table field.

The source table uses the natural keys from the legacy system, so if no
key fields are defined in the legacy table, no keys are defined in the
source table built by SQL AutoGen. zLegacy key fields must be mapped
manually in Map.

If the source table already exists in the database, it will be dropped
and built again.

<span style="font-weight: bold;">NOTE:</span> To view information about
the source in Map, including field mappings and the source schema, click
Map Source on the Page toolbar of the
<span style="font-style: italic;">Automation SQL Target Source</span>
page.

<span style="font-weight: bold;">NOTE:</span> A source table cannot be
built for a source of {Target Rules}. If the selected source is {Target
Rules}, the Create Source Table icon is disabled.

<span style="font-weight: bold;">NOTE:</span> A System Type must be
defined for a source before the table can be built. If the user did not
import a System Type in Target Design (i.e., an Excel file import,
database table import, or manual entry was used for the target design)
an error message displays when the user clicks the Create Source Table
icon. The user must set a System Type before the table can be created.
Add a System Type to a source in Target Design (Design \> Targets \>
Sources \> System Type ID).

<span style="font-weight: bold;">NOTE:</span> The key field(s) created
on source tables are identical to the key field(s) in the source system.

To build a source table in AutoGen:

1.  Click the **Automation** tab in the Quick Panel.

2.  Click the **Sources** icon for a Target.
    
    **NOTE:** The *[Automation SQL Target
    Source](../Page_Desc/Automation_SQL_Target_Source.htm)* page
    displays behind the *Automation* page and, depending on how the
    user’s view is configured, may be obstructed by the *Automation*
    page itself. In this case, to view the *Automation SQL Target
    Source* page either close the *Automation* page or reduce the size
    of the *Automation* page.

3.  Select the Target that requires a source table to be built.

4.  Click the **Create Source table** icon in the Page toolbar; a
    confirmation message displays.

5.  Click **OK**.

**NOTE:** Columns can be appended to all source tables. Refer to [Append
Utility Columns to All
Tables](../../Design/Use_Cases/Append_Utility_Columns_to_all_Tables.htm)
for more information.
