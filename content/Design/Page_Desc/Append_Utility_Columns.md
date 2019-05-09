+++
title = 'Append Utility Columns'
solution = 'Migration'
+++

# Append Utility Columns

<div class="use">

Use this page to [Append Columns to all Target or Source
Tables](../Use_Cases/Append_Utility_Columns_to_all_Tables) or [Allow
Mapping of Utility
Columns](../Use_Cases/Allow_Mapping_of_Utility_Columns).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Select **Configuration \> Append Utility Columns** in the
    *Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>COLUMN</p></td>
<td><p>Displays the name of the column to append to the table.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the field should be appended to the table.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If checked, the column is active and will be appended to the Target and or Source table as configured by the TARGET APPEND and SOURCE APPEND fields.</p>
<p>This check box is enabled by default.</p></td>
</tr>
<tr class="odd">
<td><p>KEY</p></td>
<td><p>If checked, the column is appended to the table as a key field.</p>
<p>This check box is disabled by default.</p></td>
</tr>
<tr class="even">
<td><p>DATA TYPE</p></td>
<td><p>Displays the column’s data type, such as NVARCHAR or DECIMAL.</p></td>
</tr>
<tr class="odd">
<td><p>LENGTH</p></td>
<td><p>Displays the maximum number of characters that can be stored in the field.</p></td>
</tr>
<tr class="even">
<td><p>DECIMALS</p></td>
<td><p>Displays the number of decimal places allowed in the column.</p>
<p><strong>NOTE</strong>: This field is required if the column’s data type is DECIMAL.</p></td>
</tr>
<tr class="odd">
<td><p>DEFAULT VALUE</p></td>
<td><p>Displays the default value added on the <span style="font-style: italic;"><a href="Utility_Field_Defaults">Utility Field Defaults</a></span> page.</p>
<p>Refer to <a href="../Use_Cases/Add_Utility_Field_Defaults">Add Utility Field Defaults</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>VISIBILITY</p></td>
<td><p>Displays how the appended utility field is used in mapping and whether it displays on the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Field_Mappings_H">Field Mappings</a></span> page in Map.</p>
<p>Values are:</p>
<ul>
<li><strong>Both</strong> – Mapping for Source and Target</li>
<li><strong>None</strong> – No mapping required for the field</li>
<li><strong>Source</strong> – Source only mapping</li>
<li><strong>Target</strong> – Target only mapping</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>TARGET APPEND</p></td>
<td><p>If checked, the column will be appended to all Target tables.</p>
<p>This check box is enabled by default.</p>
<p><strong>NOTE</strong>: In addition, the ACTIVE field must be enabled in order for the column to be appended.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE APPEND</p></td>
<td><p>If enabled, the column will be appended to all Source tables.</p>
<p>This check box is enabled by default.</p>
<p><strong>NOTE</strong>: In addition, the <span style="font-weight: bold;">ACTIVE</span> field must be enabled in order for the column to be appended.</p></td>
</tr>
<tr class="odd">
<td><p>DSP SUPPLIED</p></td>
<td></td>
</tr>
</tbody>
</table>
