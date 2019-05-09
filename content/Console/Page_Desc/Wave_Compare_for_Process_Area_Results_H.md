+++
title = 'Wave Compare for Process Area Results H'
solution = 'Migration'
+++

# Wave Compare for Process Area Results H

[Wave Compare for Process Area Results
V](Wave_Compare_for_Process_Area_Results_H#Wave_Compare_for_Process_Area_Results_V)

<div class="use" data-xmlns="">

Use this page to [Synchronize Target Designs Across
Waves](../Use_Cases/Synchronize_Target_Designs_Across_Waves).

</div>

**NOTE**: This page is only accessible if the current user is a member
of the WebApp group WaveSynchronizer in Console or is assigned to a
security role with access to the page. Refer to [Set
Security](../../../Platform/Sys_Admin/Use_Cases/Setting_security) in
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
3.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Process
    Areas</span> icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Hide Identical</p></td>
<td><p>Click to hide or unhide all matching comparisons in the Process Areas (as in, those comparisons that do not need to be synced) to make comparisons easier to review.</p></td>
</tr>
<tr class="odd">
<td><p>Sync Process Area</p></td>
<td><p>Click to sync the Target design in the selected Process Area between the child Wave and the baseline Wave.</p></td>
</tr>
<tr class="even">
<td><p>Sync All Process Areas</p></td>
<td><p>Click to sync the Target design in all Process Areas between the child Wave and the baseline Wave.</p></td>
</tr>
<tr class="odd">
<td><p>Process Area</p></td>
<td><p>Displays the Process Area in the child Wave that has been compared to the baseline Wave.</p></td>
</tr>
<tr class="even">
<td><p>CONSTRUCTION WEB APP ID</p></td>
<td><p>Displays the name of the WebApp used to store construction pages for the child Wave.</p>
<p>By default, the WebApp that displays the Construction pages is Construct and the source data source used for construction pages is sdbDSPConstruct. Using default values, a construct page, the underlying table, menu registrations and the schema of the construction table are automatically generated.</p></td>
</tr>
<tr class="odd">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the data source used by target rules/reports/exports for the child Wave..</p></td>
</tr>
<tr class="even">
<td><p>TARGET SYSTEM DATA SOURCE ID</p></td>
<td><p>Displays the Target system used by all object in the Wave-Process Area.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If checked, the Process Area is active. If unchecked, any context that uses the Process Area does not display in the Context Bar and cannot be used in other dspMigrate™ Advanced Data Migration (ADM) components.</p></td>
</tr>
<tr class="even">
<td><p>Objects</p></td>
<td><p>Click to open the <em><a href="Wave_Compare_for_Object_Results_H">Wave Compare for Object Results</a></em> page to review differences and sync the baseline and child Wave Target design at the Object level.</p></td>
</tr>
<tr class="odd">
<td><p>Targets</p></td>
<td><p>Click to open the <em><a href="Wave_Compare_for_Target_Results">Wave Compare for Target Result</a>s</em> page to review differences and sync the baseline and child Wave Target design at the Target level.</p></td>
</tr>
<tr class="even">
<td><p>Fields</p></td>
<td><p>Click to open the <em><a href="Wave_Compare_for_Target_Field_Results">Wave Compare for Target Field Results</a></em> page to review differences and sync the baseline and child Wave Target design at the Target field level.</p></td>
</tr>
</tbody>
</table>

## <span id="Wave_Compare_for_Process_Area_Results_V"></span>Wave Compare for Process Area Results V

[Wave Compare for Process Area Results
H](Wave_Compare_for_Process_Area_Results_H)

|                  |                                                                                                                                                                      |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field            | Description                                                                                                                                                          |
| Hide Identical   | Click to hide or unhide all matching comparisons in the Process Areas (as in, those comparisons that do not need to be synced) to make comparisons easier to review. |
| Process Area     | Displays the Process Area in the child Wave that has been compared to the baseline Wave.                                                                             |
| Field Comparison | Displays a table that lists the fields in the baseline Wave and the child Wave and the differences between them for the selected Process Area.                       |
