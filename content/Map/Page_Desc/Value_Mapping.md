+++
title = 'Value Mapping'
solution = 'Migration'
+++

# Value Mapping

<div class="use">

Use this page to [Perform Value
Mapping](../Use_Cases/Perform_Value_Mapping_Overview).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Map </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Value Mapping</span> icon
    on the *[Process Area Launch](Process_Area_Launch_map)* page.

<table>
<tbody>
<tr class="odd">
<td><p>Field   </p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Auto Map by Description</p></td>
<td><p>Click to automatically map the Target value to a Source value by comparing the legacy description to the Target description.</p>
<p>For example, the description of a legacy field is United States of America in both the legacy and Target ERP systems. A value in the field that corresponds to the description for the legacy system is US while a value in the field that corresponds to the description in the Target system is USA.  Map will use USA as the mapped value.</p></td>
</tr>
<tr class="odd">
<td><p>Auto Map by Value</p></td>
<td><p>Click to automatically update mapped Target Values by comparing the Legacy Value to the Target Value. This can be performed when a Source and Target have identical System Types, such as SAP to SAP ECC or Oracle to Oracle.</p></td>
</tr>
<tr class="even">
<td><p>CHECK TABLE</p></td>
<td><p>Displays the name of the Target ERP check table. Click the link to open the <span><a href="Value_Mapping_Config_H">Value Mapping (Config)</a></span> page to view details about the check table.</p>
<p>Check tables are also called lookup tables and are added in Target Design or imported with a System Type when it is imported into Target Design.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the description of the check table.</p>
<p><strong>NOTE:</strong> This field may be populated when a System Type was imported into Target Design, or may have been updated by a user on the <span style="font-style: italic;"><a href="../../Design/Page_Desc/Target_Lookup_Table_H">Target Lookup Table</a></span> page’s <span style="font-style: italic;">Vertical</span> View in Target Design.</p></td>
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
<td><p>Displays the count of proposed values on the <em><a href="Value_Mapping_Legacy_to_Target_H">Value Mapping (Legacy to Target)</a></em> page (as in, how many records have a Proposed Value entered) for the selected check table.  These values are for informational purposes only.</p></td>
</tr>
<tr class="odd">
<td><p>Values</p></td>
<td><p>Click to open the <a href="Value_Mapping_Legacy_to_Target_H"><em>Value Mapping (Legacy to Target)</em></a> page to perform value mappings for the selected check table. If mappings are 100% complete, no data displays on this page.</p></td>
</tr>
<tr class="even">
<td><p>Mappings</p></td>
<td><p>Click to open the <em><a href="Field_Mappings_H">Field Mappings</a></em> page to view and edit the field mappings related to the check table.</p></td>
</tr>
<tr class="odd">
<td><p>Tracking Value Mapping</p></td>
<td><p>Click to open the Mapping Values Dashboard to view a summary of value mapping progress.</p></td>
</tr>
</tbody>
</table>
