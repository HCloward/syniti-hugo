+++
title = 'Target Source Schema H'
solution = 'Migration'
+++

# Target Source Schema H

[Target Source Schema V](#Target_Source_Schema_V)

<div class="use">

Use this page to [Reset Target Source Schema Field
Lengths](../Use_Cases/Reset_Target_Source_Schema_Field_Lengths).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Map </span> in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](Process_Area_Launch_map)* page.
4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.
5.  Click the <span style="font-weight: bold;">Vertical View</span> icon
    for a Target Source.
6.  Click the <span style="font-weight: bold;">Schema Columns</span>
    icon on the *[Target Sources](Target_Sources_H_Map)* page.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Reset</p></td>
<td><p>Click to reset the Target Source schema field lengths if a Target Source was created in Map using System Types, and the System Type tables for a Target Source contained an invalid length for a column.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays order in which the columns display the Source table.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE DATABASE OBJECT ID</p></td>
<td><p>Displays the name of the Source database as defined in Target Design.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD</p></td>
<td><p>Displays field being added to the Source table.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, field is active. Only active fields are created in the Source table.</p></td>
</tr>
<tr class="odd">
<td><p>DATA TYPE</p></td>
<td><p>Displays the data type for the field being created in the Source table.</p></td>
</tr>
<tr class="even">
<td><p>KEY</p></td>
<td><p>If enabled, the field is the primary key on the table.</p>
<p><strong>NOTE:</strong> The key field(s) created on Source tables are identical to the key field(s) in the Source system.</p></td>
</tr>
<tr class="odd">
<td><p>LENGTH</p></td>
<td><p>Displays length of the field within the table.</p></td>
</tr>
<tr class="even">
<td><p>DECIMALS</p></td>
<td><p>Displays number of decimal points allowed by the field type, if the field type is Decimal or Number.</p></td>
</tr>
<tr class="odd">
<td><p>LOCK FIELD</p></td>
<td><p>If checked, the field will not be reset when the Source is reset. This field is used for manually added ZFields or ZLegacy fields that contain concatenated Source fields.</p></td>
</tr>
</tbody>
</table>

## <span id="Target_Source_Schema_V"></span>Target Source Schema V

[Target Source Schema H](Target_Source_Schema_H)

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Source Database Object ID</p></td>
<td><p>Displays the name of the Source database as defined in Target Design</p></td>
</tr>
<tr class="odd">
<td><p>Source Database Field</p></td>
<td><p>Displays field being added to the Source table.</p></td>
</tr>
<tr class="even">
<td><p>Target Table Field</p></td>
<td><p>Displays the Target field being added to the Source Table to be used to capture converted data.<br />
Example: zMEINS will be updated via a Source Rule and then updated into Target Field MEINS.</p></td>
</tr>
<tr class="odd">
<td><p>Data Type</p></td>
<td><p>Displays the data type for the field being created in the Source table.</p></td>
</tr>
<tr class="even">
<td><p>Key</p></td>
<td><p>If checked, the field is the primary key on the table.</p>
<p><strong>NOTE:</strong> The key field(s) created on Source tables are identical to the key field(s) in the Source system.</p></td>
</tr>
<tr class="odd">
<td><p>Length</p></td>
<td><p>Displays length of the field within the table.</p></td>
</tr>
<tr class="even">
<td><p>Decimals</p></td>
<td><p>Displays number of decimal places allowed by the field, if the data type is Decimal or Number.</p></td>
</tr>
<tr class="odd">
<td><p>Default Value</p></td>
<td><p>Displays default value if field is a computed column, for example, zSource.</p></td>
</tr>
<tr class="even">
<td><p>Comment</p></td>
<td><p>Displays a user-entered comment about the Source field.</p></td>
</tr>
<tr class="odd">
<td><p>Target Design Default</p></td>
<td><p>Displays the default value used by the utility columns before rules are processed.<br />
Example: zDuplicateInd will have a default value of 0 (zero).</p></td>
</tr>
</tbody>
</table>
