# <span id="Waves_H"></span>Waves H

[Waves V](#Waves_V)

<div class="use">

Use this page to [Create the Contexts for Migration
Projects.](../Use_Cases/Create_Contexts_for_Migration_Projects.htm)

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane, or select
    <span style="font-weight: bold;">Console</span> in the Context bar.
2.  Click <span style="font-weight: bold;">Waves</span> in the
    <span style="font-style: italic;">Navigation</span> pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Copy Wave</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Copy_Wave.htm">Copy Wave</a></span> page to create a Wave based on the selected Wave.</p></td>
</tr>
<tr class="odd">
<td><p>Create Milestones From Template</p></td>
<td><p>This icon will be used in a future release.</p></td>
</tr>
<tr class="even">
<td><p>Build Comparison</p></td>
<td><p>Click to open the <em><a href="Build_Wave_Comparison.htm">Build Wave Comparison</a></em> page to compare and sync target designs across Waves.</p>
<p><strong>NOTE</strong>: This icon only displays if the current user is a member of the WebApp group Wavesynchronizer in Console or is assigned to a security role with access to the page. Refer to <a href="../../../Platform/Sys_Admin/Use_Cases/Setting_security.htm">Set Security</a> in System Administration for more information.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the name of the Wave, which categorizes the migration project. Examples of Wave names include country names or specific work locations where the migration will be rolled out.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If checked, the Wave is active and will display in the Context bar. The Wave is associated with an active Process Area to create a context. A user selects the context in the Context bar to work in and it displays the associated dspMigrate™ Advanced Data Migration (ADM) components. If unchecked, any context that uses the Wave does not display in the Context bar and cannot be used in other dspMigrate™ Advanced Data Migration (ADM) components.</p>
<p><strong>NOTE</strong>: If this wave is included in IGC’s Migration dashboard and this value is then unchecked, the wave continues to display on the dashboard until the current date is greater than one month from the wave’s end date, but no metrics data is sent to the dashboard for this wave.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the Wave.</p></td>
</tr>
<tr class="even">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the Data Source ID against which the Wave is executed.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET DATASOURCE</p></td>
<td><p>Displays the data source that contains the Target tables downloaded from the ERP system. This data source must be registered in Common. Refer to <a href="../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm">Register a Data Source in Common</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Process Area</p></td>
<td><p>Click to open the <em><a href="Wave_Process_Areas.htm"><em>Wave: Process Areas</em></a></em> page to add, edit or delete a Process Area for the selected Wave.</p></td>
</tr>
<tr class="odd">
<td><p>Metrics</p></td>
<td><p>Click to open the <em><a href="Wave_Gate_Metrics_Value_Mapping_H.htm">Wave Gate Metrics (Value Mapping</a>)</em> page to add, edit or delete Wave gate metrics for value mappings for the selected Wave.</p></td>
</tr>
<tr class="even">
<td><p>Summary Construction</p></td>
<td><p>Click to display the Field Construction charts which display a summary of construction status by the number of fields that are expected, the number of fields that are in process, and the total number of fields for the target.</p>
<p>Refer to <a href="../../Construct/Use_Cases/Field_Construction_by_Wave.htm">Field Construction by Wave</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Summary Field Mapping</p></td>
<td><p>Click to display the dashboard for a summary of field mappings for the selected Wave ID.</p>
<p>Refer to <a href="../../Map/Use_Cases/Field_Mapping_by_Wave.htm">Field Mapping by Wave</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Summary Value Mapping</p></td>
<td><p>Click to display the Value Mapping by Wave chart for the selected Wave ID to view Value Mapping progress.</p>
<p>Refer to <a href="../../Map/Use_Cases/Value_Mapping_by_Wave.htm">Value Mapping by Wave</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Waves_V"></span>Waves V

[Waves H](#Waves_H)

<div class="use">

Use this page to [Create the Contexts for Migration
Projects](../Use_Cases/Create_Contexts_for_Migration_Projects.htm).

</div>

Field

Description

Name

Displays the name of the Wave, which categorizes the migration project.
Examples of Wave names include country names or specific work locations
where the migration will be rolled out.

Description

Displays a description of the Wave.

ERP Settings

Target System

Displays the data source that contains the Target tables downloaded from
the ERP system. This data source must be registered in Common  and the
tables downloaded in Collect. Refer to [Register a Data Source in
Common](../../../Platform/Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
for more information.

Multiple target systems can be added to a Wave. Refer to [Add Multiple
Target Systems at the Wave-Process Area
Level](../Use_Cases/Add_Multiple_Target_Systems.htm) for more
information.

Client

Displays the ERP system client name. This value should match an entry in
T000 and a single client should be used.

Language

Displays the ERP system language. This value should match an entry in
T002 and is used to update the description of Target check table values.

Start Date

Displays the date that work on the migration for this wave begins. This
date is used as a milestone by default in the Migration dashboard. Refer
to [Configure the IGC Migration
Dashboard](../../../Platform/Agent_Int/Use_Cases/Configure_the_Migration_Dashboard.htm)
for more information.

**NOTE**: If there are multiple instances of the DSP, and a wave's name,
start and end dates are identical in multiple instances, data from only
one wave displays on the dashboard.

End Date

Displays the date that work on the migration for this wave ends. This
date is used as a milestone by default in the Migration dashboard. Refer
to [Configure the IGC Migration
Dashboard](../../../Platform/Agent_Int/Use_Cases/Configure_the_Migration_Dashboard.htm)
for more information.

**NOTE**: If the current date is one month or later past this end date,
the wave does not display on the dashboard.

**NOTE**: If there are multiple instances of the DSP, and a wave's name,
start and end dates are identical in multiple instances, data from only
one wave displays on the dashboard.
