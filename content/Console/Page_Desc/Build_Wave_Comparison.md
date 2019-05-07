+++
title = 'Build Wave Comparison'
solution = 'Migration'
+++

# Build Wave Comparison

<div class="use" data-xmlns="">

Use this page to [Synchronize Target Designs Across
Waves](../Use_Cases/Synchronize_Target_Designs_Across_Waves.htm).

</div>

**NOTE**: This page is only accessible if the current user is a member
of the WebApp group Wavesynchronizer in Console or is assigned to a
security role with access to the page. Refer to [Set
Security](../../../Platform/Sys_Admin/Use_Cases/Setting_security.htm) in
System Administration for more information.

To access this page:

1.  Select
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">dspMigrate</span>
    in the
    <span style="font-style: italic;" data-xmlns="http://www.w3.org/1999/xhtml">Navigation</span>
    pane, or select
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Console</span>
    in the Context bar.
2.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">
    Build Comparison</span> icon in the Page toolbar.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Process</p></td>
<td><p>Click to compare the selected child Wave with the baseline Wave.</p></td>
</tr>
<tr class="odd">
<td><p>Hide Identical/ Un Hide Identical</p></td>
<td><p>Click to hide or unhide all matching comparisons (as in, those comparisons that do not need to be synced) to make comparisons easier to review. When used on this page, all matching comparisons are hidden at all levels of the migration hierarchy – Process Areas, Objects, Targets and fields.</p></td>
</tr>
<tr class="even">
<td><p>Wave ID</p></td>
<td><p>Displays the name of the child Wave compared to the baseline Wave selected on the <em><a href="Waves_H.htm">Waves</a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the child Wave.</p></td>
</tr>
<tr class="even">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the Data Source ID against which the child Wave is executed.</p></td>
</tr>
<tr class="odd">
<td><p>CLIENT</p></td>
<td><p>Displays the ERP system client name for the child Wave. This value must match an entry in T000 and a single client should be used.</p>
<p><strong>NOTE:</strong> This value is used with SAP only.</p></td>
</tr>
<tr class="even">
<td><p>LANGUAGE</p></td>
<td><p>Displays the ERP system language for the child Wave. This value must match an entry in T002 and is used to update the description of Target check table values.</p>
<p><strong>NOTE:</strong> This value is used with SAP only.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If checked, the child Wave is active. Comparisons can be made between inactive Waves.</p></td>
</tr>
<tr class="even">
<td><p>COMPARE COMPLETED</p></td>
<td><p>Displays the date and time the compare process finished running.</p>
<p>If the field is blank, the compare process has not yet been run.</p></td>
</tr>
<tr class="odd">
<td><p>Process Areas</p></td>
<td><p>Click to open the <em><a href="Wave_Compare_for_Process_Area_Results_H.htm">Wave Compare for Process Area Results</a></em> page to review differences after the compare process runs and sync the baseline and child Wave target design at the Process Area level.</p></td>
</tr>
<tr class="even">
<td><p>Objects</p></td>
<td><p>Click to open the <em><a href="Wave_Compare_for_Object_Results_H.htm">Wave Compare for Object Results</a></em> page to review differences after the compare process runs and sync the baseline and child Wave target design at the Object level.</p></td>
</tr>
<tr class="odd">
<td><p>Targets</p></td>
<td><p>Click to open the <em><a href="Wave_Compare_for_Target_Results.htm">Wave Compare for Target Results</a></em> page to review differences after the compare process runs and sync the baseline and child Wave Target design at the Target level.</p></td>
</tr>
<tr class="even">
<td><p>Fields</p></td>
<td><p>Click to open the <em><a href="Wave_Compare_for_Target_Field_Results.htm">Wave Compare for Target Field Results</a></em> page to review differences after the compare process runs and sync the baseline and child Wave Target design at the Target field level.</p></td>
</tr>
</tbody>
</table>
