# Target Source Rules H

[Target Source Rules V (All Tabs)](#Target_Source_Rules_V)

<div class="use">

Use the page to [Add Target Source
Rules](../Use_Cases/Add_Target_Source_Rules.htm).

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. See the Bulk Execution topic in System
Administration for more information.

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Click the **Targets** icon on the *[Process Area
    Launch](Process_Area_Launch.htm)* page.
3.  Click the **Sources** icon for a Target.
4.  Click the **Rules** icon for a Target Source.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Execute</p></td>
<td><p>Click to run the selected Target Source rule immediately in the foreground and to create the stored procedure from the view.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset the processing status if a process fails for the selected Target Source rule.</p></td>
</tr>
<tr class="even">
<td><p>Debug</p></td>
<td><p>Click to open the <em><a href="Debug_Breakpoints_Target_Sources.htm">Debug – Breakpoints (Target Sources)</a></em> page to add breakpoints to steps in the process for the selected Target Source for Target Source rules and Target Source reports. Use breakpoints to debug issues with failed processing.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the Target Source rule is processed.</p></td>
</tr>
<tr class="even">
<td><p>STATUS</p></td>
<td><p>Displays the <span id="Status" class="popUpLink">status</span>. Only active rules are run.</p></td>
</tr>
<tr class="odd">
<td><p>RULE TYPE</p></td>
<td><p>Displays the action the Target Source rule will take. Options include Delete, Insert, Manual, Move, and Update.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE RULE VIEW</p></td>
<td><p>Displays the view created in SQL server for the selected Target Source rule.</p>
<p><strong>NOTE:</strong> Only views that follow the proper naming convention display. Refer to <a href="../Use_Cases/Naming_Conventions.htm">Naming Conventions</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the Target Source rule.</p></td>
</tr>
<tr class="even">
<td><p>ACTION ON</p></td>
<td><p>Displays the last date the rules was processed.</p></td>
</tr>
<tr class="odd">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of records affected by the Target Source rule’s execution.</p></td>
</tr>
<tr class="even">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time Transform took to process the selected Target Source rule. If the field is empty, the rule has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
<tr class="odd">
<td><p>Queue</p></td>
<td><p>Click to open the <em><a href="Monitor_Transform_H.htm">Monitor</a></em> page to monitor the background job processes for the selected Target Source rule. If a Target Source rule has no data to process, this button is disabled.</p></td>
</tr>
</tbody>
</table>

## <span id="Target_Source_Rules_V"></span>Target Source Rules V All Tabs

[Target Source Rules H](Target_Source_Rules_H.htm)

<div class="use">

Use the page to [Add Target Source
Rules](../Use_Cases/Add_Target_Source_Rules.htm).

</div>

This page has the following tabs:

  - [General tab](#General_Tab2)
  - [Documentation tab](#Documentation_Tab2)
  - [Process Information tab](#Process_Information_Tab2)

## <span id="General_Tab2"></span>General tab

Field

Description

Reset

Click to reset the processing status if a process fails for the selected
Target Source rule.

Process

Click to process the Target Source rule in the background. View the
status of background processing on the
*[Monitor](../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm)*
page.

Debug

Click to open the [*Debug – Breakpoints (Target
Sources)*](Debug_Breakpoints_Target_Sources.htm) page to add breakpoints
to steps in the process for the selected Target Source for Target Source
rules and Target Source reports. Use breakpoints to debug issues with
failed processing.

Source Rule

Displays the name of the view stored in the target database that
corresponds to the selected Target Source rule. Click to open the
<span style="font-style: italic;">[Definitions](../../../Platform/Common/Page_Desc/Definitions.htm)</span>
page to view the SQL definition of the rule.

Rule Automation Information

Rule Type

Displays the action the Target Source rule will take. Options include
Delete, Insert, Manual, Move, and Update.

Source Rule View

Displays the view created in SQL server for the selected Target Source
rule.

Source Rule Table

Displays the table in SQL that corresponds to the view.

**NOTE**: For insert or delete rules, this field must be blank.

Build Rule

Click to build a new Target Source rule or to build an updated Target
Source rule after updates have been made. If a rule already exists, it
is overwritten.

Status Information

Priority

Displays the order the Target Source rule is processed.

Status

Displays the <span id="Status" class="popUpLink">status</span>. Only
active Target Source rules are
run.

## <span id="Documentation_Tab2"></span>Documentation tab

|             |                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| ----------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field       | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| Description | Displays a description of the Target Source rule.                                                                                                                                                                                                                                                                                                                                                                                                                         |
| Comment     | Displays user-entered comments about the selected Target Source rule.                                                                                                                                                                                                                                                                                                                                                                                                     |
| Recon Type  | Displays an option to indicate if a Target Source rule adds records, deletes records or is informational. If a data audit is conducted to determine if all data records were loaded (as they were expected to be loaded), the Recon Type justifies why records were not loaded. Use the options Adds records (+) or Deletes records (-) include or exclude, respectively, on certain exports (delta loads, multi-step loads, etc.) from the Target Reconciliation Report. |
| Audit       | Click to open the *[Target Source Rule Audit](Target_Source_Rule_Audit.htm)* page to add, edit and delete an audit report with a sample method for the Target Source rule and to download the results.                                                                                                                                                                                                                                                                    |

## <span id="Process_Information_Tab2"></span>Process Information tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Action On</p></td>
<td><p>Displays the date Transform processed the selected Target Source rule.</p></td>
</tr>
<tr class="odd">
<td><p>Record Count</p></td>
<td><p>Displays the number of records affected by the Target Source rule’s execution.</p></td>
</tr>
<tr class="even">
<td><p>Duration</p></td>
<td><p>Displays the amount of time Transform took to process the selected Target Source rule. If the field is empty, the Target Source rule has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
</tbody>
</table>
