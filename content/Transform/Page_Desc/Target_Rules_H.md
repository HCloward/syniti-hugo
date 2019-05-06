# Target Rules H

[Target Rules V All Tabs](#Target_Rules_V_All_Tabs)

<div class="use">

Use this page to [Add Target Rules](../Use_Cases/Add_Target_Rules.htm).

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. Refer to [Use Bulk
Execution](../../../Platform/Bulk_Exec/Use_Bulk_Execution.htm) for more
information.

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Click the **Targets** icon on the *[Process Area
    Launch](Process_Area_Launch.htm)* page.
3.  Click the **Rules** icon for a Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Execute</p></td>
<td><p>Click to run the selected rule immediately in the foreground.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset the processing status if a process fails for the selected target rule.</p></td>
</tr>
<tr class="even">
<td><p>Debug</p></td>
<td><p>Click to open the <em><a href="Debug_Breakpoints.htm"><em>Debug – Breakpoints</em></a></em> page to add breakpoints to steps in the process for the selected target for target rules. Use breakpoints to debug issues with failed processing.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the target rule is processed.</p></td>
</tr>
<tr class="even">
<td><p>STATUS</p></td>
<td><p>Displays the <span id="Status" class="popUpLink">status</span> of the target rule.</p></td>
</tr>
<tr class="odd">
<td><p>RULE TYPE</p></td>
<td><p>Displays the action the rule will take. Options include:</p>
<ul>
<li><strong>Delete</strong> – Delete only rules.</li>
<li><strong>Insert</strong> – Insert only rules.</li>
<li><strong>Manual</strong> – All rules.</li>
<li><strong>Move</strong> – Move only rules.</li>
<li><strong>Update</strong> – Update only rules</li>
</ul></td>
</tr>
<tr class="even">
<td><p>TARGET RULE VIEW</p></td>
<td><p>Displays the view created in SQL server for the selected target rule.</p>
<p><strong>NOTE:</strong> Only views that follow the proper naming convention display. Refer to <a href="../Use_Cases/Naming_Conventions.htm">Naming Conventions</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the rule.</p></td>
</tr>
<tr class="even">
<td><p>ACTION ON</p></td>
<td><p>Displays the last date the target rule was processed.</p></td>
</tr>
<tr class="odd">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of records affected by the target rule’s execution.</p></td>
</tr>
<tr class="even">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time Transform took to process the selected target rule. If the field is empty the target rule has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
<tr class="odd">
<td><p>Queue</p></td>
<td><p>Click to open the <em><a href="Monitor_Transform_H.htm">Monitor</a></em> page to monitor the background job processes for the selected target rule. If a rule has no data to process, this icon is disabled.</p></td>
</tr>
</tbody>
</table>

## <span id="Target_Rules_V_All_Tabs"></span>Target Rules V All Tabs

[Target Rules H](Target_Rules_H.htm)

<div class="use">

Use this page to [Add Target Rules](../Use_Cases/Add_Target_Rules.htm).

</div>

This page has the following tabs:

  - [General tab](#General_Tab4)
  - [Documentation tab](#Documentation_Tab4)
  - [Process Information tab](#Process_Information_Tab4)

## <span id="General_Tab4"></span>General tab

Field

Description

Reset

Click to reset the processing status if a process fails for the selected
target rule.

Debug

Click to open the *[Debug – Breakpoint](Debug_Breakpoints.htm)s* page to
add breakpoints to steps in the process for the selected target for
target rules. Use breakpoints to debug issues with failed processing.

Target Rule

Displays the name of the view stored in the target database that
corresponds to the selected target rule.

Rule Automation Information

Rule Type

Displays the action the rule will take. Options include Delete, Insert,
Manual, Move, and Update.

Target Rule View

Displays the view created in SQL server for the selected target rule.

Target Rule Table

Displays the title of the table in SQL corresponding to the view.

Build Rule

Click to build a new rule based on the target rule.

**NOTE:** If a rule already exists, it is overwritten.

Status Information

Priority

Displays the order the target rule is processed.

Status

Displays the <span id="Status" class="popUpLink">status</span> of the
target
rule.

## <span id="Documentation_Tab4"></span>Documentation tab

|             |                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field       | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| Description | Displays a description of the target rule.                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Comment     | Displays user-entered comments about the selected target rule.                                                                                                                                                                                                                                                                                                                                                                                                     |
| Recon Type  | Displays an option to indicate if a target rule adds records, deletes records or is informational. If a data audit is conducted to determine if all data records were loaded (as they were expected to be loaded), the Recon Type justifies why records were not loaded. Use the options Adds records (+) or Deletes records (-) include or exclude, respectively, on certain exports (delta loads, multi-step loads, etc.) from the Target Reconciliation Report. |
| Audit       | Click to open the *[Target Rule Audit](Target_Rule_Audit_H.htm)* page to add, edit and delete an audit report with a sample method for the target rule and to download the results.                                                                                                                                                                                                                                                                                |

## <span id="Process_Information_Tab4"></span>Process Information tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Action On</p></td>
<td><p>Displays the date Transform processed the selected target rule.</p></td>
</tr>
<tr class="odd">
<td><p>Record Count</p></td>
<td><p>Displays the number of records affected by the target rule’s execution.</p></td>
</tr>
<tr class="even">
<td><p>Duration</p></td>
<td><p>Displays the amount of time Transform took to process the selected target rule. If the field is empty, the target rule has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
<tr class="odd">
<td><p>Process</p></td>
<td><p>Click to process the target rule in the background. View the status of background processing on the <em><a href="../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm">Monitor</a></em> page.  </p></td>
</tr>
</tbody>
</table>
