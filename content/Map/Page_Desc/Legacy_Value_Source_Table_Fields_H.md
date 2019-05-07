+++
title = ''
solution = 'Migration'
+++

# <span id="top"></span>Legacy Value (Source Table Fields) H

[Legacy Value (Source Table Fields) V](#LegacyV)

<div class="use">

Use this page when [Value Map Target Fields from Multiple Source
Systems](../Use_Cases/Value_Map_Target_Fields_from_Mulitple_Source_Systems.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Map </span>in the Context
    bar.
3.  Select <span style="font-weight: bold;">Configuration \>Value
    Mapping (Config)</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    check table.
5.  Click <span style="font-weight: bold;">Vertical View</span> for a
    Source.
6.  Click the <span style="font-weight: bold;">Source Tables</span>
    icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SOURCE</p></td>
<td><p>Displays the name of the Source as defined in Target Design.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE TABLE</p></td>
<td><p>Displays the Source table containing the field.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE FIELD</p></td>
<td><p>Displays the Source field containing the value.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays the status of the Source field, such as whether the field is active, if value mapping is complete or if the Source field is not used. The field is used to track when a Mapper incorrectly sets a field mapping with an action of Xref. This status will leave a place holder for other users to review the setting and either activate or inactivate this Source field or table.</p></td>
</tr>
<tr class="even">
<td><p>LEGACY DESCRIPTION TABLE</p></td>
<td><p>Displays the table name that stores the description field of the Source field.  Usually, the value and description are stored in the same table.</p></td>
</tr>
<tr class="odd">
<td><p>LEGACY DESCRIPTION FIELD</p></td>
<td><p>Displays the field name that contains the description of the Source field.</p>
<p>For example, the field State contains a value of GA. The description of the State field would be Georgia, and is stored in the description field.</p></td>
</tr>
<tr class="even">
<td><p>View Values</p></td>
<td><p>Click to open the <em><a href="Legacy_Value_Source_Table_Fields_H.htm">Legacy Value (Source Table Fields)</a></em> page to view all values for the Source table that must be value mapped or removed.</p></td>
</tr>
<tr class="odd">
<td><p>Value Mappings</p></td>
<td><p>Click to open the <em><a href="Value_Mapping_Legacy_to_Target_H.htm">Value Mapping (Legacy to Target)</a></em> page to perform value mapping for the selected Source field.</p></td>
</tr>
<tr class="even">
<td><p>Value Tracking</p></td>
<td><p>Click to open the <em><a href="Source_Value_Tracking.htm">Source Value Tracking</a></em> page to view each Source table that has a field that has been mapped to the selected lookup table.</p>
<p>Refer to <a href="../Use_Cases/View_the_Source_Tables_and_Fields_Mapped_to_a_Lookup_Table.htm">View the Source Tables and Fields Mapped to a Lookup Table</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Remove Values</p></td>
<td><p>Click to remove all unmapped values from the Source table. Mapped values must be removed manually.</p></td>
</tr>
<tr class="even">
<td><p>Refresh</p></td>
<td><p>Click to delete unmapped values and pull new values from the Source.</p></td>
</tr>
</tbody>
</table>

## <span id="LegacyV"></span>Legacy Value (Source Table Fields) V

[Legacy Value (Source Table Fields) H](#top)

<div class="use">

Use this page when [Defining Tables and Fields for Multiple Source
Systems to Use in Value
Mapping](../Use_Cases/Value_Map_Target_Fields_from_Mulitple_Source_Systems.htm).

</div>

Field

Description

Data Source Name

Displays the database name of the Source.

Source

Displays the name of the Source as defined in Target Design.

Check Table

Displays the name of the ERP check table.

Comment

Displays user-entered comments about the selected check table.

Source Table

Displays the Source table containing the field.

**NOTE:** The Source table for the check table for the Rule Xref action
is not automatically set. It must be entered in this field.

Source Field

Displays the Source field containing the value.

**NOTE:** The Source field for the check table for the Rule Xref action
is not automatically set. It must be entered in this field.

Client Field

Displays the name of the field used for filtering on Client
Values.  This field only applies to SAP Sources. For example: MANDT,
CLIENT or MANDANT

Language Field

Displays the name of the language field in the Source table to filter
description updates in one language.  This field only applies to SAP
Sources.

Legacy Description Table

Displays the table name that stores the description field for the Source
field.  Usually, the value and description are stored in the same table.

Legacy Description Field

Displays the field name that contains the description of the Source
field.

For example, the field State contains a value of GA. The description of
the State field would be Georgia, and is stored in the description
field.

Legacy Description Table Key Field

Displays a key field name when the primary key of the Source table does
not match the primary key of the Legacy Description Table.

Legacy Description Language Field

Displays the field in the Source table that stores the description of
the language.

Additional Information

Source Field2

Displays the second Key field name (for Multi-Part Key Source table).

Source Field3

Displays the third Key field name (for Multi-Part Key Source table).

Source Field4

Displays the fourth Key field name (for Multi-Part Key Source table.

Source Field5

Displays the fifth Key field name (for Multi-Part Key Source table).

Description Update SQL

Displays the Override Download SQL if the Source Table is too
complicated for auto-generated SQL commands.

Value Download Where Clause

Displays the where clause to append to the download of values to filter
on a smaller mapping list.
