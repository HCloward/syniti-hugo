+++
title = 'Source Check Table (Config) H'
solution = 'Migration'
+++

# Source Check Table (Config) H

[Source Check Table (Config) V](#Source)

<div class="use">

Use this page when [Value Map Target Fields from Multiple Source
Systems](../Use_Cases/Value_Map_Target_Fields_from_Mulitple_Source_Systems.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Map </span> in the Context
    bar.
3.  Select <span style="font-weight: bold;">Configuration \> Value
    Mapping (Config)</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    check table.
5.  Click the <span style="font-weight: bold;">Source Config</span> icon
    for a Source.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SOURCE</p></td>
<td><p>Displays the name of the Source where the check table is stored as defined in Target Design.</p></td>
</tr>
<tr class="odd">
<td><p>CHECK TABLE</p></td>
<td><p>Displays the name of the ERP check table.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If checked, the check table is active and can be used in value mapping.</p></td>
</tr>
<tr class="odd">
<td><p>DEPLOYMENT DATE</p></td>
<td><p>Displays the date the Source check table is deployed.</p>
<p>This field is for documentation purposes only.</p></td>
</tr>
<tr class="even">
<td><p>VALUES PULLED ON</p></td>
<td><p>Displays the date and time Target values were last refreshed from the Wave Target data source. Target values are retrieved when a user clicks Refresh on the <span style="font-size: 11.0pt;font-family: Arial, sans-serif;font-style: italic;"><a href="Value_Mapping_Config_H.htm">Value Mapping (Config)</a></span> page's<span style="font-size: 11.0pt;font-family: Arial, sans-serif;font-style: italic;">Vertical</span> View.</p></td>
</tr>
<tr class="odd">
<td><p>Tables</p></td>
<td><p>Click to open the <em><a href="Legacy_Value_Source_Table_Fields_H.htm">Legacy Value (Source Table Fields)</a></em> page to add, edit and delete the Source tables used to create the value.</p></td>
</tr>
<tr class="even">
<td><p>Value Mappings</p></td>
<td><p>Click to open the <em><a href="Value_Mapping_Legacy_to_Target_H.htm">Value Mapping (Legacy to Target)</a></em> page to add, edit and delete the Target values that are mapped to the selected check table.</p></td>
</tr>
<tr class="odd">
<td><p>Mappings</p></td>
<td><p>Click to open the <em><a href="Field_Mappings_H.htm">Field Mappings</a></em> page to access only those mappings that use the selected check table.</p></td>
</tr>
<tr class="even">
<td><p>Value Tracking</p></td>
<td><p>Click to open the <em><a href="Value_Mapping_Legacy_to_Target_H.htm">Value Mapping (Legacy to Target)</a></em> page to add, edit and delete the Target values that are mapped to the selected check table.</p></td>
</tr>
<tr class="odd">
<td><p>Refresh</p></td>
<td><p>Click to refresh Source values in the check table.</p>
<p><strong>NOTE:</strong> After loading Source values into a lookup table in Map, only those Source values that are to be mapped (as in, only those fields for which a rule has been created) are retained in the lookup table when the Target is processed. Unmapped Source value fields are deleted if they are not used in the Target table.</p></td>
</tr>
</tbody>
</table>

## <span id="Source"></span>Source Check Table (Config) V

[Source Check Table (Config) H](#)

<div class="use">

Use this page when [Defining Tables and Fields for Multiple Source
Systems to Use in Value
Mapping](../Use_Cases/Value_Map_Target_Fields_from_Mulitple_Source_Systems.htm).

</div>

Field

Description

Source

Displays the name of the Source as defined in Target Design where the
check table is stored.

Click the link to open the *[Value Mapping
(Sources)](Value_Mapping_Sources_H.htm)* page to perform Value Mapping
for a rule with an Xref or Rule Xref action.

Source Details

Active

If checked, the check table is active and can be used in value mapping.

Comment

Displays brief description of the check table.

Deployment Date

Displays the date the Source check table is deployed.

This field is for documentation purposes only.

Values Pulled On

Displays the date and time Target values were last refreshed from the
Wave Target data source. Target values are retrieved when a user clicks
Refresh on
the<span style="font-size: 11.0pt;font-family: Arial, sans-serif;font-style: italic;">[Value
Mapping (Config)](Value_Mapping_Config_H.htm)</span>
page's <span style="font-size: 11.0pt;font-family: Arial, sans-serif;font-style: italic;">Vertical</span>
View.

Values Pulled By

Displays the user ID of the user who clicked Refresh.

Target Details

Check Table

Displays the name of the ERP check table. Click the link to open
the<span style="font-size: 11.0pt;font-family: Arial, sans-serif;">[Value
Mapping (Config)](Value_Mapping_Config_H.htm)</span>page to view details
about the check table.

<span id="Lookup Table Type" class="popUpLink">Type</span>

Displays an option indicating whether fields in the check table should
be value mapped.

Remediation Value

Displays a remediation value used to complete mock loads only and never
used in the Production environment.

Target Pulled On

Displays the date and time Target values were last retrieved from the
Wave Target data source. Target values are retrieved when a user clicks
Refresh on the *[Value Mapping (Config)](Value_Mapping_Config_H.htm)*
page's *Horizonta*l View.

Target Pulled By

Displays the user ID of the user who clicked Refresh.
