# Append Utility Columns to All Tables

A Designer can add Utility columns that must be appended to all Target
and/or Source tables.

A Utility field (also called a zField) does not exist in the Target
system, but rules and reports are registered to it in Transform. Fields
of this type should be captured in Target Design but should not be
mapped and will not display in Map. A utility field is added to the
Target table to be used by AutoGen.

If a Target or Source table has already been created, the columns are
appended automatically. The Target or Source table does not need to be
rebuilt.

<span style="font-weight: bold;">NOTE</span>: The zSource  column is
installed with the platform and cannot be deleted.

<span style="font-weight: bold;">NOTE</span>: If a user deletes an
append column from the [Append Utility
Columns](../Page_Desc/Append_Utility_Columns.htm) page, if it has
already been synced with Map, the column still appears on the Target
table. To remove the append column in this case, set the column to
inactive.

<span style="font-weight: bold;">NOTE</span>: If a user deletes a column
from the [Append Utility
Columns](../Page_Desc/Append_Utility_Columns.htm) page that has already
been added to a Target table using SQL AutoGen, that column must be
manually deleted from the Target table.

To append columns to tables in Target Design:

1.  Select **Configuration \> Append Utility Columns** in the
    *Navigation* pane.

2.  Click <span style="font-weight: bold;">Add</span>.
    
    *[View the field descriptions for the Append Utility Columns
    page](../Page_Desc/Append_Utility_Columns.htm)*

3.  Enter the name of the column to append to the table in the
    **COLUMN** field.

4.  Enter a value in the **PRIORITY** field to indicate the order the
    field should be appended to the table.

5.  Enable or disable the **ACTIVE** check box as needed.
    
    <span style="font-weight: bold;">NOTE</span>: The ACTIVE check box
    is enabled by default and indicates that the column will be appended
    to the  Target or Source table as indicated.

6.  Enable the **KEY** check box if the  column should be appended to
    the table as a key column.

7.  Select the column’s data type, such as NVARCHAR or DECIMAL, from the
    **DATA TYPE** list box.

8.  Enter the maximum number of characters that can be stored in the
    field in the **LENGTH** field.

9.  Enter the number of decimal places allowed in the field in the
    **DECIMALS** field.
    
    <span style="font-weight: bold;">NOTE</span>: If the data type for
    the column is DECIMAL, this field is required.

10. Select a default value to use for the column in the **DEFAULT
    VALUE** list box.
    
    <span style="font-weight: bold;">NOTE</span>: Default values are
    added on the *[Utility Field
    Defaults](../Page_Desc/Utility_Field_Defaults.htm)* page. Refer to
    [Add Utility Field Defaults](Add_Utility_Field_Defaults.htm) for
    more information.

11. Enable or disable the **TARGET APPEND** check box as needed.
    
    <span style="font-weight: bold;">NOTE</span>: The
    <span style="font-weight: bold;">TARGET APPEND</span> check box is
    checked by default and indicates that the column will be appended to
    all Target tables.

12. Enable or disable the **SOURCE APPEND** check box as needed.
    
    <span style="font-weight: bold;">NOTE</span>: The
    <span style="font-weight: bold;">SOURCE APPEND</span> check box is
    checked by default and indicates that the column will be appended to
    all Source  tables.

13. Click **Save**.
