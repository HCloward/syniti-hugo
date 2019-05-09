+++
title = 'Source Where Used'
solution = 'Migration'
+++

# Source Where Used

<div class="use">

Use this page to [View Target and Source
Assignments](../Use_Cases/View_Target_and_Source_Assignments).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Select <span style="font-weight: bold;">Configuration \>
    Source</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
4.  Click the <span style="font-weight: bold;">Targets</span> icon for a
    Source.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the name of the Target table that uses the Source data source.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE DATA SOURCE</p></td>
<td><p>Displays the name of the Source data source. This Source data source can be either a database (.sdb) or sdbDSPConstruct which is a Source built in Construct.</p>
<p>A Source data source can be assigned to only one System Type across all Targets and Waves</p></td>
</tr>
<tr class="even">
<td><p>SYSTEM TYPE ID</p></td>
<td><p>Displays the System Type of the data source, if one was added.</p>
<p>System Types are added in Common and contain generic information including keys, fields, check tables, join relationships between tables and generic mappings for external systems (for example, Target ERP and Legacy) being used for a data migration.</p>
<p>The System Type is assigned to a Source on the <span style="font-style: italic;"><a href="Target_Sources_H_Design">Target Sources</a></span> page.</p>
<p>Refer to <a href="../../../Platform/Common/Use_Cases/System_Types_Overview">System Types</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Wave NAME</p></td>
<td><p>Displays the name of the Wave to which the selected Source belongs.</p>
<p><strong>NOTE</strong>: A Wave and Process Area are combined to create a context. The current context displays in the Context bar.</p></td>
</tr>
<tr class="even">
<td><p>Process Area</p></td>
<td><p>Displays the name of the Process Area to which the selected Source belongs.</p>
<p><strong>NOTE</strong>: A Wave and Process Area are combined to create a context. The current context displays in the Context bar.</p></td>
</tr>
<tr class="odd">
<td><p>OBJECT ID</p></td>
<td><p>Displays the name of the Object containing the Target that uses the Source.</p></td>
</tr>
</tbody>
</table>
