+++
title = 'Build Target Tables'
solution = 'Migration'
+++

# Build Target Tables

Target tables can be built using SQL AutoGen after targets have been
added and configured in Target Design.

<span style="font-weight: bold;">NOTE:</span> The target’s Design Status
must be In Design or Design Finished to perform this task.

<span style="font-weight: bold;">NOTE:</span> Mapping is not required to
create a target table. Once the target is saved in Target Design, the
target table can be built using SQL AutoGen.

<span style="font-weight: bold;">NOTE:</span> Once the table has been
created, the Create Target Table icon on the
<span style="font-style: italic;">Automation</span> page will be
disabled. The Create Target Table icon will be active if the target is
synced with Map.

When a target table is built, the AutoGen process uses the design
specified in Target Design and builds the tt table with all active
fields. The key field(s) indicated on the *[Target
Fields](../../Design/Page_Desc/Target_Fields_H_Target_Design)* page
in Target Design is set as the primary key for the table in the
database. Additional details about target fields that are used when
building the target table display in Target Design on the *Target
Fields* page’s *Vertical* View in the Details section.

<span style="font-weight: bold;">NOTE:</span> A user can create all
target tables, source tables, Update Row source tables, and rules at one
time by clicking the Create All Objects icon on the
<span style="font-style: italic;">[Automation](../Page_Desc/Automation_page)</span>
page.

All objects created using SQL AutoGen are written to the data source
defined for the object in Console (Process Area \> Objects \> Vertical
View \> Data Source ID).

If the target table already exists in the database, it will be dropped
and built again when the user clicks the Create Target Table icon on the
<span style="font-style: italic;">Automation</span> page.

<span style="font-weight: bold;">NOTE:</span> When a target table is
created using AutoGen, a complete view of the target is available on the
<span style="font-style: italic;">Target Fields</span> page in Target
Design. The zSource and zLegacy\* fields are created but are read only
on the <span style="font-style: italic;">Target Fields</span> page.

<span style="font-weight: bold;">NOTE:</span> A System Type must be
defined for a target before the table can be built. If the user did not
import a System Type in Target Design (for example, an Excel file
import, database table import, or manual entry was used for the target
design) an error message displays when the user clicks the Create Target
Table icon. The user must set a System Type before the table can be
created. Add a System Type to a target in Target Design (Design \>
Targets icon \> Vertical View icon for a target \> System Type ID).

<span class="msoIns" style="font-weight: bold;">NOTE:</span> Key fields
are created during field mapping. Key(s) on the target table are created
by using the key(s)from the target system and the zLegacy field.  For
example, the MATNR field identified as the key field in Target Design is
used to create the key field zLegacyMATNR on the target table. The key
field is added to the target table when the table is created during SQL
AutoGen.

To build a target table in AutoGen:

1.  Click the **Automation** tab in the Quick Panel.
2.  Select the object that should contain the target table.
3.  Click the **Create Target Table** icon in the Page toolbar; a
    confirmation message displays.
4.  Click **OK**.

<span style="font-weight: bold;">NOTE:</span> If a table exists in the
database, the Create Target Table icon is disabled until the target is
synced with Map.

**NOTE:** Columns can be appended to all target tables when a table is
created or rebuilt. Refer to [Append Columns to All Target or Source
Tables](../../Design/Use_Cases/Append_Utility_Columns_to_all_Tables)
for more information.
