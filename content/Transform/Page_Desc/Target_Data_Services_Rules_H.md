+++
title = 'Target Data Services Rules H'
solution = 'Migration'
+++

# Target Data Services Rules H

[Target Data Services Rules V](#Target_Data_Services_Rules_V)

<div class="use">

Use this page to [Add Target Data Services
Rules](../Use_Cases/Add_Target_DS_Rules.htm).

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. Refer to [Use Bulk
Execution](../../../Platform/Bulk_Exec/Use_Bulk_Execution.htm) for more
information.

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Click the **Targets** icon on the *[Process Area
    Launch](Process_Area_Launch.htm)* page.
3.  Click the **Data Services Rules** icon for a Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Execute</p></td>
<td><p>Click to execute the Data Services Job.</p>
<p><strong>NOTE:</strong> The status for the Data Services rule must have an Active status before it can be executed in Data Services.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset the request, which overrides the current state of the request and resets it for processing. Reset should only be used if an error occurred during processing which left the request in an unusable state.</p></td>
</tr>
<tr class="even">
<td><p>Debug</p></td>
<td><p>Click to open the <em><a href="Debug_Breakpoints.htm">Debug – Breakpoints</a></em> page to add breakpoints to steps in the process for the selected target, including target rules and target reports. Use breakpoints to debug issues with failed processing.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the Data Services target rules are processed.</p></td>
</tr>
<tr class="even">
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
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays the <span id="Status" class="popUpLink">status</span> of the rule.</p></td>
</tr>
<tr class="even">
<td><p>TARGET DATA SERVICES RULE</p></td>
<td><p>Displays the name of the job in Data Services to execute from within Transform.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the rule.</p></td>
</tr>
<tr class="even">
<td><p>ACTION ON</p></td>
<td><p>Displays the last date the Data Services target rule was processed.</p></td>
</tr>
<tr class="odd">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of records affected by the Data Services target rule’s execution.</p></td>
</tr>
<tr class="even">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time Transform took to process the selected Data Services target rule. If the field is empty, the target rule has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
<tr class="odd">
<td><p>QUEUE</p></td>
<td><p>Click to open the<em>Monitor</em>page to monitor the background job processes for the selected target rule. If a rule has no data to process, this icon is disabled.</p></td>
</tr>
</tbody>
</table>

 

## <span id="Target_Data_Services_Rules_V"></span>Target Data Services Rules V

[Target Data Services Rules H](#Target_DS_Rules_H)

<div class="use">

Use this page to [Add Target Data Services
Rules.](../Use_Cases/Add_Target_DS_Rules.htm)

</div>

This page contains the following tabs:

  - [General](#General)
  - [Documentation](#Documentation)
  - [Process Information](#Process_Info)

## <span id="General"></span>General

Field

Description

Target Data Services Rule

Displays the name of the job in Data Services that you want to execute
from within Transform.

Rule Automation Information

Rule Type

Displays the action the rule will take. Options include:

  - **Delete** – Delete only rules.
  - **Insert** – Insert only rules.
  - **Manual** – All rules.
  - **Move** – Move only rules.
  - **Update** – Update only rules

Target Data Services Rule Table

Not used in the current version of the tool.

Status Information

Priority

Displays the rule priority.

**NOTE:** Rules are grouped and run by priority in Data Services.

Status

Displays whether the rule is active or inactive.

Additional Properties

Global Variables

Click to update the Global Variables. Refer to [Configure Target Data
Services Rule Global
Variables](../Use_Cases/Configure_Target_DS_Rule_Global_Var.htm) for
more
information.

 

## <span id="Documentation"></span>Documentation

|             |                                                             |
| ----------- | ----------------------------------------------------------- |
| Field       | Description                                                 |
| Description | Displays the description of the target Data Services rule.  |
| Comment     | Displays a comment regarding the target Data Services rule. |
| Recon Type  | Not used in the current version of the tool.                |
| Audit       | Not used in the current version of the tool.                |

 

## <span id="Process_Info"></span>Process Information

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Action On</p></td>
<td><p>Displays the date and time the Data Services rules were processed.</p></td>
</tr>
<tr class="odd">
<td><p>Record Count</p></td>
<td><p>Displays the record count for the Data Services rules processed. This will not be populated for the Data Services AutoGen jobs as it includes multiple tables being processed in a single job.</p></td>
</tr>
<tr class="even">
<td><p>Duration</p></td>
<td><p>Displays the amount of time Transform took to process the selected Data Services target rule. If the field is empty, the target rule has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
<tr class="odd">
<td><p>Process</p></td>
<td><p>Click to process the Data Services target rule.</p></td>
</tr>
</tbody>
</table>
