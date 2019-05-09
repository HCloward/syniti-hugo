+++
title = 'System Types Table Fields H'
solution = 'Platform'
+++

# System Types Table Fields H

[System Types Table Fields V](#SystemTypesV)

<div class="use">

Use this page to:

  - [Add Fields to Tables](../Use_Cases/Add_Fields_to_Tables)
  - [Add a Lookup Table
    Manually](../Use_Cases/Add_a%20Lookup%20Table%20Manually.)

</div>

To access this page:

1.  Select **Common \> System Types** in the *Navigation* pane.
2.  Click the **Tables** icon for a System Type.
3.  Click the **Fields** icon for a Table Name.

**NOTE:** Excel Integration has been enabled on this page. Refer to [Use
Excel Integration](../../Excel_Int/Use_Excel_Integration) for more
information.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>FIELD ORDER</p></td>
<td><p>Displays order of field within the system table.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD</p></td>
<td><p>Displays name of field within the system table.</p>
<p><strong>NOTE:</strong> The validation will fail if the field name is not unique.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays brief description of the field.</p></td>
</tr>
<tr class="odd">
<td><p>KEY FIELD</p></td>
<td><p>If enabled, the field is the key on the table.</p></td>
</tr>
<tr class="even">
<td><p>DATA TYPE</p></td>
<td><p>Displays data type for the field, for example, int or nvarchar.</p></td>
</tr>
<tr class="odd">
<td><p>LENGTH</p></td>
<td><p>Displays number of characters permitted by the field.</p></td>
</tr>
<tr class="even">
<td><p>LOOKUP TABLE</p></td>
<td><p>Click the link on the name of the lookup table to open the <em><a href="System_Types_Table_Lookup">System Types Table Lookup</a></em> page to view or edit the fields in the lookup table.</p></td>
</tr>
<tr class="odd">
<td><p>Static Value List</p></td>
<td><p>Click to open the <em><a href="System_Types_Table_Statics">System Types Table Statics</a></em> page to add a static value for the field.</p></td>
</tr>
<tr class="even">
<td><p>DSP SUPPLIED</p></td>
<td><p>If enabled, this content is installed with the platform and cannot be edited.</p>
<p>If disabled, the content was added by a user or process.</p>
<p><strong>NOTE:</strong> This is a display-only check box. It cannot be updated.</p></td>
</tr>
</tbody>
</table>

## <span id="SystemTypesV"></span>System Types Table Fields V

[System Types Table Fields H](#top)

<div class="use">

Use this page to [Add Fields to
Tables](../Use_Cases/Add_Fields_to_Tables).

</div>

This page has the following tabs:

  - [General](#General_Tab)
  - [Documentation](#Documentation_Tab)

### <span id="General_Tab"></span>General tab

Field

Description

Field Data

Field Order

Displays order of field within system table.

Field

Displays name of field within system table.

Description

Displays brief description of field.

Key Field

If enabled, field is the key on the table.

Field Details

Data Type

Displays data type for field, for example, int or nvarchar.

Length

Displays number of characters permitted by field.

Decimals

Displays the number of decimal places allowed in numeric fields that
allow for decimals.

Field Format

Displays the format of the field used to validate the data in this field
during Data Services AutoGen and Construct Data entry. Values are Date,
Time, Decimal and Checkbox.

For example, the Date Format for a target is set at YYYYDDMM.

This value will be loaded into Target Design's [Target
Fields](../../../Migration/Design/Page_Desc/Target_Fields_H_Target_Design)
page.

Active For Mapping Default

If enabled, the table field is marked Active when the table is used in
the mapping process by Map. If disabled, the table field is made
inactive until manually activated. The default value for this check box
is enabled for manually entered fields and disabled for system-imported
fields.

Rule Field

If enabled, the field is marked as Rule Only. A Rule Only field is part
of the table creation process, but is excluded from being moved between
the Source Table to the Source Table in the Object database, or between
the Source Table in the Object database to the Target Table in the
Object database.

### <span id="Documentation_Tab"></span>Documentation tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Application Screen</p></td>
<td><p>Displays the name of the screen in the ERP system that contains the field.</p></td>
</tr>
<tr class="odd">
<td><p>Help Text</p></td>
<td><p>Displays helpful information about the field. For System Types delivered with the DSP®, this field is imported directly from the System Type help documentation.</p></td>
</tr>
<tr class="even">
<td><p>Comment</p></td>
<td><p>Displays a user-entered comment about the target field.</p>
<p>This field is for documentation purposes only.</p></td>
</tr>
<tr class="odd">
<td><p>Instructions</p></td>
<td><p>Displays instructions about how to use the field in mapping or other functions.</p>
<p>This field is for documentation purposes only.</p></td>
</tr>
</tbody>
</table>
