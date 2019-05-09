+++
title = 'Target Sources (Add Row)'
solution = 'Migration'
+++

# Target Sources (Add Row)

<div class="use">

Use this page while:

  - [Add Update Row Sources that are
    Views](../Use_Cases/Add_Update_Row_Sources#Add_Update_Row_Sources_that_are_Views)
  - [Add Update Row Sources that are
    Tables](../Use_Cases/Add_Update_Row_Sources#Add_Update_Row_Sources_that_are_Tables)
  - [Adding an External Source](../Use_Cases/Add_an_External_Source)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Map </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](Process_Area_Launch_map)* page.
4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.
5.  Click the <span style="font-weight: bold;">Update Row Sources</span>
    icon for a Source.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Sync from Target Design</p></td>
<td><p>Click to sync Map with Target Design, updating tables, fields, Sources and lookup tables.</p>
<p>When Map and Target Design are out of sync, the message Pending Design Changes displays to the right of the page name.</p></td>
</tr>
<tr class="odd">
<td><p>Auto Map</p></td>
<td><p>Click to create a copy of the rule mappings for fields that exist in the Target table and the Source database object. The fields in the Target table and the Source database object must match for rule mappings to be created.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE DATABASE OBJECT</p></td>
<td><p>Displays name of the Source table or view, or indicates if the Source is an Update Row Source.</p>
<p><strong>NOTE:</strong> When a user sets the Source database object and clicks Save, Map validates that the Source database object exists in the System Type. If the Source database object does not exist:</p>
<p>If the user imported a System Type in Target Design for the Target Source, the Source database object is imported into the System Type.</p>
<p>If the user did not import a System Type in Target Design (i.e., an Excel file import, database table import, or manual entry was used for the Target Design), Map displays an error message that the user must set a System Type before field mapping can be performed. Add a System Type to a Target in Target Design (Design &gt; Targets &gt;Vertical View for a Target &gt; System Type ID).</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If checked, the Source is active for the Wave.</p></td>
</tr>
<tr class="even">
<td><p>Secondary Source</p></td>
<td><p>Click to open the <em><a href="Target_Sources_Update_Row">Target Sources (Update Row)</a></em> page to add an Update Row Source to the selected Add Row Source.</p>
<p>Add an Update Row when data from another Source table is needed to update the Add Row Source.</p></td>
</tr>
<tr class="odd">
<td><p>Mappings</p></td>
<td><p>Click to open the <em><a href="Field_Mappings_H">Field Mappings</a></em> page to create and reset field mappings for all fields in the selected Add Row Source, to view the history for a selected mapping, or to view mapping details. A number does not display on this icon if no field mappings have been activated for the current context.</p></td>
</tr>
</tbody>
</table>
