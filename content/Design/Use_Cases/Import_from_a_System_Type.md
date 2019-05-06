# Import From a System Type

The design of a Target can be imported from a System Type, which
contains generic information about external systems (for example, Target
and Legacy) used for a data migration. Refer to [System
Types](../../../Platform/Common/Use_Cases/System_Types_Overview.htm) for
more information about adding and configuring System Types.

**NOTE:**On the *Targets* page, **Import Fields** is available in Target
Design to import one Target at a time. A user must enter the **SYSTEM
TYPE ID** and the **TARGET SYSTEM TABLE NAME**and click the **Import
Fields** icon.

Target Import is also allowed (one or more Targets) from database tables
or from an Excel file (using a template provided). Refer to [Import a
Target Design from a Database](Import_from_a_Database.htm) or [Import a
Target Design from an Excel](Import_from_an_Excel_File.htm) file for
more information.

When importing from a System Type, the user selects the table in the
System Type to import. After a successful import, the table displays on
the *[Targets](../Page_Desc/Targets_H_Design.htm)* page in Target
Design, with the proper prefix appended to the front of the table name.
When a user selects the Target on the *Targets* page, the fields in the
Target table display on the *Target Fields* page.

After a table is imported, the Key fields on the table are assigned a
criticality of High and a required level of Technical Required. For
non-key fields, the criticality is set to Medium and the required level
is set to Conditional.

<span style="font-weight: bold;">NOTE</span>: If a System Type does not
have tables, an error displays on import, and the System Type cannot be
imported. The count on the Tables icon on the
<span style="font-style: italic;">Target Object Import: System
Types</span> page is 0. If a table in a System Type does not have
fields, the table will be imported, but will have no fields in Target
Design. The Fields icon on the <span style="font-style: italic;">System
Type Import</span> page displays 0.

**NOTE**: A System Type cannot be imported if no tables have been
registered for the System Type in Common. Refer to [Add System Tables
and
Fields](../../../Platform/Common/Use_Cases/Add_System_Tables_and_Fields.htm)
for more information.

To import a System Type in Target Design:

1.  Click **Target Import** in the *Navigation* pane.

2.  Click the **System Types Import** icon for an OBJECT ID in the
    parent pane.
    
    <span style="text-indent: -.25in;font-weight: bold;">NOTE:</span> If
    a System Type has been previously imported into Target Design the
    System Type can only be re-imported if the Target's Design Status is
    In Design. On the *Targets* page, if a Target is selected with a
    Design Status of Design Finished, Completed or Inactive, the Target
    Import icon is disabled.

3.  Click the **Import** icon for a SYSTEM TYPE in the child pane.

4.  Click the **IMPORT** check box to include a table in the import.
    
    <span style="font-weight: bold;">NOTE:</span> If an imported field
    is a Key field, the Verify Post Load check box is checked for the
    field by default on import.
    
    **NOTE**: Import can be checked for multiple tables at once. To
    select a contiguous range of records, hold down the **Shift** key
    and select the first and last records in the range. To select a
    non-contiguous range of records, hold down the **Ctrl** key and
    select each record. Click the **Mark for Import** icon. To exclude
    multiple tables from import, repeat these steps but click the
    **Clear Import Flag** icon.

5.  Click the **Execute Import** icon in the Page toolbar; a
    confirmation message displays.

6.  Click **OK**.

During the import, new records are added to the tables, fields, and
lookup tables. If the records have been added into the Target
previously, updates are applied to existing tables, fields and lookup
tables.

**NOTE**: If a Source was added in Target Design during a System Type
import, and the System Type tables for a Source contained an invalid
length for a column, use the Reset functionality to update a Source
table with the column’s correct length. Refer to [Reset Target Source
Schema Field
Lengths](../../Map/Use_Cases/Reset_Target_Source_Schema_Field_Lengths.htm)
for more information.
