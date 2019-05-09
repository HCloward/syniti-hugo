+++
title = 'Value Mapping (Sources) H'
solution = 'Migration'
+++

# Value Mapping (Sources) H

[Value Mapping (Sources) V](#Value_Mapping_Sources_V)

<div class="use">

Use this page to [Perform Value
Mapping](../Use_Cases/Perform_Value_Mapping_Overview).

</div>

To access this page:

1.  Click **dspMigrate** in the *Navigation* pane.
2.  Click **Map** in the Context bar.
3.  Click the **Value Mapping** icon on the *[Process Area
    Launch](Process_Area_Launch_map)* page.
4.  Click the **Mappings** icon for a check table.
5.  Click the check table name link in the **LOOKUP** column on the
    *[Field Mappings](Field_Mappings_H)* page next to a mapping with
    Xref or RuleXref action.
6.  Click the **Sources** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SOURCE</p></td>
<td><p>Displays the name of the Target Source.</p></td>
</tr>
<tr class="odd">
<td><p>CHECK TABLE</p></td>
<td><p>Displays the name of the Source check table. Click link to open the <span><a href="Value_Mapping_Config_H">Value Mapping (Config)</a></span> page to view details about the check table.</p>
<p>Check tables are also called lookup tables and are added in Target Design or imported with a System Type when it is imported into Target Design.</p></td>
</tr>
<tr class="even">
<td><p>MAPPED PERCENT</p></td>
<td><p>Displays the percent of value mapping that is complete for the selected check table.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPED</p></td>
<td><p>Displays the number of values mapped for the selected check table.</p></td>
</tr>
<tr class="even">
<td><p>PROPOSED VALUES</p></td>
<td><p>Displays the number of proposed values on the <em><a href="Value_Mapping_Legacy_to_Target_H">Value Mapping (Legacy to Target)</a></em> page for the selected check table. These proposed values are for informational purposes only.</p></td>
</tr>
<tr class="odd">
<td><p>Source Config</p></td>
<td><p>Click to open the <em><a href="Source_Check_Table_Config_H">Source Check Table (Config)</a></em> page to view additional information about the check table and to refresh check table values.</p></td>
</tr>
<tr class="even">
<td><p>Value Mappings</p></td>
<td><p>Click to open the <em><a href="Value_Mapping_Legacy_to_Target_H">Value Mapping (Legacy to Target)</a></em> page to perform value mappings for the selected check table. If mappings are 100% complete, no data displays on this page.</p></td>
</tr>
<tr class="odd">
<td><p>Mappings</p></td>
<td><p>Click to open the <em><a href="Field_Mappings_H">Field Mappings</a></em> page to view and edit the field mappings related to the selected check table.</p></td>
</tr>
</tbody>
</table>

###  

## <span id="Value_Mapping_Sources_V"></span>Value Mapping (Sources) V

[Value Mapping (Sources) H](Value_Mapping_Sources_H)

<div class="use">

Use this page to

  - [Perform Value
    Mapping](../Use_Cases/Perform_Value_Mapping_Overview)

  - [Remove Unmapped Source
    Values](../Use_Cases/Remove_Unmapped_Source_Values)

</div>

Field

Description

Check Table

Displays the name of the Source check table. Click link to open the
<span>[Value Mapping (Config)](Value_Mapping_Config_H)</span> page
to view details about the check table.

Check tables are also called lookup tables and are added in Target
Design or imported with a System Type when it is imported into Target
Design.

Mapped

Displays the number of values mapped for the selected check table.

Values

Click to open the *[Value Mapping (Legacy to
Target)](Value_Mapping_Legacy_to_Target_H)* page to perform value
mappings for the selected check table. If mappings are 100% complete, no
data displays on this page.

Advanced

Target Table Import

Click to perform a Target table import. This feature is used when a
Source may have many values being used, but only values in the Target
table need to be mapped. Click Remove Values to delete all unmapped
Source values and then click Target Table Import to load used values
that need to be mapped.

Source Tables

Click to open the *[Legacy Value (Source Table
Fields)](Legacy_Value_Source_Table_Fields_H)* page to add, edit and
delete additional Source tables and fields that must be value mapped for
the check table.

Remove Values

Click to remove all values in the Source field (stored in the Source
data source) that have not yet been value mapped to a Target table. Use
this feature only if the remaining values in the Source field should not
be mapped to the Target field.

Source

Click to open the *[Source Check Table
(Config)](Source_Check_Table_Config_H)* page to edit and configure
the check table for the Source.
