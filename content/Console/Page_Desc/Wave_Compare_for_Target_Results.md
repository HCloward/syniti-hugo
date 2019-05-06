# Wave Compare for Target Results H

[Wave Compare for Target Results
V](Wave_Compare_for_Target_Results.htm#Wave_Compare_for_Target_Results_V)

<div class="use" data-xmlns="">

Use this page to [Synchronize Target Designs Across
Waves](../Use_Cases/Synchronize_Target_Designs_Across_Waves.htm).

</div>

**NOTE**: This page is only accessible if the current user is a member
of the WebApp group WaveSynchronizer in Console or is assigned to a
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
2.  Click
    the<span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">
    Build Comparison</span> icon in the Page toolbar.
3.  Click the
    <span style="font-weight: bold;" data-xmlns="http://www.w3.org/1999/xhtml">Targets
    </span>icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Hide Identical</p></td>
<td><p>Click to hide or unhide all matching comparisons in the targets (as in, those comparisons that do not need to be synced) to make comparisons easier to review.</p></td>
</tr>
<tr class="odd">
<td><p>Sync Target</p></td>
<td><p>Click to sync the Target design in the selected Target between the child Wave and the baseline Wave.</p></td>
</tr>
<tr class="even">
<td><p>Sync All Targets</p></td>
<td><p>Click to sync the Target design in all Targets between the child Wave and the baseline Wave.</p></td>
</tr>
<tr class="odd">
<td><p>Process Area</p></td>
<td><p>Displays the Process Area in the child Wave that has been compared to the baseline Wave.</p></td>
</tr>
<tr class="even">
<td><p>OBJECT</p></td>
<td><p>Displays the Object in the child Wave that has been compared to the baseline Wave.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET</p></td>
<td><p>Displays the name of the Target in the child Wave.</p></td>
</tr>
<tr class="even">
<td><p>TYPE</p></td>
<td><p>Displays how fields in the Target are used. Values are:</p>
<ul>
<li><strong>Natural</strong> – The fields exist in the Target system. The system adds a “z” to the front of the field name used in the Source table.</li>
<li><strong>Utility</strong> – The fields do not exist in the Target system, but can be used to register rules and reports to in Transform. Fields of this type should be captured in Target Design.  A utility field is added to the target table to be used by the AutoGen process.  Utility fields will be appended to BOTH the target and source table as is.  No “z” field will be appended.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>TARGET SYSTEM TABLE NAME</p></td>
<td><p>Displays the name of the table in the Target system, which is the name in the NAME field without the tt appended to the front.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a brief description of the Target table.</p></td>
</tr>
<tr class="odd">
<td><p>SYSTEM TYPE ID</p></td>
<td><p>Displays the System Type that was imported to create the Target design, or the System Type that was selected for the Target.</p>
<p>Refer to <a href="../../Design/Use_Cases/Import_from_a_System_Type.htm">Import a Target Design from a System Type</a> and <a href="../../../Platform/Common/Use_Cases/System_Types_Overview.htm">System Types</a>  for more information.</p></td>
</tr>
<tr class="even">
<td><p>Fields</p></td>
<td><p>Click to open the <em><a href="Wave_Compare_for_Target_Field_Results.htm">Wave Compare for Target Field Results</a></em> page to review differences and sync the baseline and child Wave Target design at the Target field level.</p></td>
</tr>
</tbody>
</table>

## <span id="Wave_Compare_for_Target_Results_V"></span>Wave Compare for Target Results V

[Wave Compare for Target Results
H](Wave_Compare_for_Target_Results.htm)

|                  |                                                                                                                                                                |
| ---------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field            | Description                                                                                                                                                    |
| Hide Identical   | Click to hide or unhide all matching comparisons in the targets (as in, those comparisons that do not need to be synced) to make comparisons easier to review. |
| Process Area     | Displays the Process Area in the child Wave that has been compared to the baseline Wave.                                                                       |
| Object           | Displays the Object in the child Wave that has been compared to the baseline Wave.                                                                             |
| Target           | Displays the name of the Target.                                                                                                                               |
| Field Comparison | Displays a table that lists the fields in the baseline Wave and the child Wave and the differences between them for the selected Target.                       |
