+++
title = 'Target Remediation H'
solution = 'Migration'
+++

# Target Remediation H

[Target Remediation V All Tabs](#Target_Remediation_V_All)

<div class="use">

Use this page to [Register Target Remediation
Rules](../Use_Cases/Register_Target_Remediation_Rules.htm).

</div>

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Click the **Targets**icon on the *[Process Area
    Launch](Process_Area_Launch.htm)* page.
3.  Click the **Reports** icon for a Target.
4.  Click the **Vertical View** icon for a report.
5.  Click the **Remediation Information** tab.
6.  Click the **Remediation** icon.

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
<td><p>Click to reset the processing status if a process fails for the selected target remediation rule.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the remediation rule is processed.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays the <span id="Status" class="popUpLink">status</span> of the remediation rule.</p></td>
</tr>
<tr class="even">
<td><p>TARGET REPORT REMEDIATION RULE VIEW</p></td>
<td><p>Displays the view Map created in SQL server for the selected target remediation rule.</p></td>
</tr>
<tr class="odd">
<td><p>RULE TYPE</p></td>
<td><p>Displays the action the rule will take. Options are:</p>
<ul>
<li><strong>Delete</strong> – Delete only rules.</li>
<li><strong>Insert</strong> – Insert only rules.</li>
<li><strong>Manual</strong> – All rules.</li>
<li><strong>Move</strong> – Move only rules.</li>
<li><strong>Update</strong> – Update only rules</li>
</ul></td>
</tr>
<tr class="even">
<td><p>TARGET REPORT REMEDIATION RULE</p>
<p> </p></td>
<td><p>Displays the stored procedure Map created in SQL. The Rule Builder will automatically build the stored procedure if no data is entered in this field when the record is saved.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the remediation rule.</p></td>
</tr>
<tr class="even">
<td><p>ACTION ON</p></td>
<td><p>Displays the date Transform processed the selected remediation rule. If the field is empty, the report has not been processed.</p></td>
</tr>
<tr class="odd">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of records affected by the selected remediation rule.</p></td>
</tr>
<tr class="even">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time Transform took to process the selected remediation rule. If the field is empty, the rule has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
<tr class="odd">
<td><p>Queue</p></td>
<td><p>Click to open the <em><a href="Monitor_Transform_H.htm">Monitor</a></em> page to monitor the background job processes for the selected target remediation rule. If a rule has no data to process, this button is disabled.</p></td>
</tr>
</tbody>
</table>

##  

## <span id="Target_Remediation_V_All"></span>Target Remediation V All Tabs

[Target Remediation H](Target_Remediation_H.htm)

<div class="use">

Use this page to [Register Target Remediation
Rules](../Use_Cases/Register_Target_Remediation_Rules.htm).

</div>

This page has the following tabs:

  - [General tab](#General_Tab6)
  - [Documentation tab](#Documentation_Tab6)
  - [Process Information tab](#Process_Information_Tab5)

## <span id="General_Tab6"></span>General tab

Field

Description

Target Report Remediation Rule

Displays the stored procedure Map created in SQL when the remediation
rule was created. The Rule Builder will automatically build this stored
procedure if no data is entered in this field when the record is saved.

Rule Automation Information

Rule Type

Displays the action the rule will take. Options include:

  - **Delete** – Delete only rules.
  - **Insert** – Insert only rules.
  - **Manual** – All rules.
  - **Move** – Move only rules.
  - **Update** – Update only rules

Target Report Remediation Rule View

Displays the view Map created in SQL server for the selected target
remediation rule.

Target Report Remediation Rule Table

Displays the table Map created in SQL server for the selected target
remediation rule.

Build Rule

Click to build a new target remediation rule based on the Target
Remediation Rule View.

**NOTE:** If a rule already exists, it is overwritten.

Status Information

Priority

Displays the order the remediation rule is processed.

Status

Displays the <span id="Status" class="popUpLink">status</span> of the
remediation
rule.

## <span id="Documentation_Tab6"></span>Documentation tab

|             |                                                                   |
| ----------- | ----------------------------------------------------------------- |
| Field       | Description                                                       |
| Description | Displays a description of the target remediation rule.            |
| Comment     | Displays user-entered comments about the target remediation rule. |

## <span id="Process_Information_Tab5"></span>Process Information tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Duration</p></td>
<td><p>Displays the amount of time Transform took to process the selected remediation rule. If the field is empty, the rule has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
<tr class="odd">
<td><p>Record Count</p></td>
<td><p>Displays the number of records affected in the target by the selected remediation rule.</p></td>
</tr>
<tr class="even">
<td><p>Action On</p></td>
<td><p>Displays the date Transform processed the selected remediation rule. If the field is empty, the rule has not been processed.</p></td>
</tr>
<tr class="odd">
<td><p>Process</p></td>
<td><p>Click to process the target remediation rule in the background. View the status of background processing on the <em><a href="../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm">Monitor</a></em> page. </p></td>
</tr>
</tbody>
</table>
