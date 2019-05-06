# Source

<div class="use">

Use this page to:

  - [View Sources Assigned to
    Targets](../Use_Cases/View_Target_and_Source_Assignments.htm).
  - [Update System Types for a
    Source](../Use_Cases/Update_System_Types_for_a_Source.htm)

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Select <span style="font-weight: bold;">Configuration \>
    Source</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SOURCE ID</p></td>
<td><p>Displays the name of the Source data source, a database with the .sdb extension. If the name is sdbDSPConstruct, the Source selected when the Source was added in Target Design was {Full Construction}, a Source built in Construct.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE</p></td>
<td><p>Displays the Source name.</p>
<p>Data sources should be registered in Common. Refer to <a href="../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm">Register a Data Source in Common</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>SYSTEM TYPE ID</p></td>
<td><p>Displays the System Type of the data source, if one was added.</p>
<p>System Types are added in Common and contain generic information including keys, fields, check tables, join relationships between tables and generic mappings for external systems (for example, Target ERP and Legacy) being used for a data migration.</p>
<p>The System Type is assigned to a Source on the <span style="font-style: italic;"><a href="Target_Sources_H_Design.htm">Target Sources</a></span> page.</p>
<p>Refer to <a href="../../../Platform/Common/Use_Cases/System_Types_Overview.htm">System Types</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a brief description of the data source.</p>
<p>Data sources should be registered in Common. Refer to <a href="../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm">Register a Data Source in Common</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Targets</p></td>
<td><p>Click to open the <em><a href="Source_Where_Used.htm">Source When Used</a></em> page to view a list of Targets that use the selected Source and to sync Source data source-System Types across all Targets.</p></td>
</tr>
</tbody>
</table>
