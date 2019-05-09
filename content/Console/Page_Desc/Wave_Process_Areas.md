+++
title = 'Wave: Process Areas H'
solution = 'Migration'
+++

# Wave: Process Areas H

[Wave: Process Areas V](#Wave)

<div class="use">

Use this page to [Create the Contexts for Migration
Projects.](../Use_Cases/Create_Contexts_for_Migration_Projects)

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane, or select
    <span style="font-weight: bold;">Console</span> in the Context bar.
2.  Click <span style="font-weight: bold;">Waves</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
3.  Click the <span style="font-weight: bold;">Process Areas</span> icon
    for a
Wave.

|                                 |                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field                           | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Create Milestones From Template | This icon will be used in a future release.                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| Process Area ID                 | Displays a concatenated value that is comprised of the Process Area name and the description (\<Process Area name\> + ‘-‘ + \<description\>). Combining a Process Area with a Wave creates a context, which can be selected in the Context bar and used throughout dspMigrate™ Advanced Data Migration (ADM) components while working on a migration project.                                                                                                                        |
| ACTIVE                          | If checked, the Process Area is active and will display in the Context Bar. The Process Area is associated with an active Wave to create a context. A user selects the context in the Context bar to work in and it displays the associated dspMigrate™ Advanced Data Migration (ADM) components.  If unchecked, any context that uses the Process Area does not display in the Context bar and cannot be used in the other of dspMigrate™ Advanced Data Migration (ADM) components. |
| Objects                         | Click to open the *[Process Area: Object](Process_Area_ObjectH)* page to add, edit, or delete an Object in the selected Process Area.                                                                                                                                                                                                                                                                                                                                            |
| Metrics                         | Click to open the *[Wave Process Area Gate Metrics (Field Mapping)](Wave_Process_Area_Gate_Metrics_Field_Mapping_H)* page to add, edit or delete metrics for field mapping.                                                                                                                                                                                                                                                                                                      |
| Summary Construction            | Click to display the dashboard for field construction by Wave and Process Area for the selected Wave ID.                                                                                                                                                                                                                                                                                                                                                                             |
| Summary Field Mapping           | Click to display the dashboard for field mapping by Wave and Process Area for the selected Wave ID.                                                                                                                                                                                                                                                                                                                                                                                  |
| Summary Value Mapping           | Click to display the dashboard for field value by Wave and Process Area for the selected Wave ID.                                                                                                                                                                                                                                                                                                                                                                                    |
| COMMENT                         | Displays user-entered comments about the Process Area.                                                                                                                                                                                                                                                                                                                                                                                                                               |

## <span id="Wave"></span>Wave Process Areas V

[Wave: Process Areas H](#Wave:_Process_Areas_H)

<div class="use">

Use this page to

  - [Create the Contexts for Migration
    Projects.](../Use_Cases/Create_Contexts_for_Migration_Projects)
  - [Set the Data Source](../Use_Cases/Set_the_Data_Source)
  - [Add Multiple Target
    Systems](../Use_Cases/Add_Multiple_Target_Systems)

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Process Area ID</p></td>
<td><p>Displays the name of the Process Area. Combining a Process Area with a Wave creates a context, which can be selected in the Context bar and used throughout dspMigrate™ Advanced Data Migration (ADM) components while working on a migration project.</p></td>
</tr>
<tr class="odd">
<td><p>Target System Data Source ID</p></td>
<td><p>Displays the Target system used by all Object in the Wave-Process Area. The default value is the Target system set at the Wave level. The Target system can be overridden at the Wave-Process Area level.</p>
<p>Refer to <a href="../Use_Cases/Add_Multiple_Target_Systems">Add Multiple Target Systems at the Wave-Process Area Level</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Data Source ID</p></td>
<td><p>Displays the data source used by Target rules/reports/exports.</p>
<p><span style="font-size: 11.0pt;font-family: Arial, sans-serif;">The data source used here cascades through all Objects in the Process Area.</span></p>
<p>Refer to <a href="../Use_Cases/Set_the_Data_Source">Set the Data Source at the Wave Process Area or Object Level</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Construction Web App ID</p></td>
<td><p>Displays the name of the Web App used.</p></td>
</tr>
<tr class="even">
<td><p>Construction Source Data Source</p></td>
<td><p>Displays the name of the data source used.</p></td>
</tr>
<tr class="odd">
<td><p>Comment</p></td>
<td><p>Displays user-entered comments about the Process Area.</p></td>
</tr>
</tbody>
</table>
