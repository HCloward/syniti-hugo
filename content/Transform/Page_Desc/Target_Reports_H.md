+++
title = 'Target Reports H'
solution = 'Migration'
+++

# Target Reports H

[Target Reports V All Tabs](#Target_Reports_V_All_Tabs)

<div class="use">

Use this page to [Add Target
Reports](../Use_Cases/Add_Target_Reports.htm).

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. Refer to [Use Bulk
Execution](../../../Platform/Bulk_Exec/Use_Bulk_Execution.htm) for more
information.

To access this page in Transform:

1.  Click the **Targets** icon on the *[Process Area
    Launch](Process_Area_Launch.htm)* page.
2.  Click the **Reports** icon for a Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Execute</p></td>
<td><p>Click to run the selected target report immediately in the foreground.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset the processing status if a process fails for the selected target report.</p></td>
</tr>
<tr class="even">
<td><p>Debug</p></td>
<td><p>Click to open the <a href="Debug_Breakpoints.htm"><em>Debug – Breakpoints</em></a> page to add breakpoints to steps in the process for the selected target, including target rules and target reports. Use breakpoints to debug issues with failed processing.</p>
<p>Refer to <a href="../Use_Cases/Debug_Rules_and_Reports_using_Brkpnts.htm">Debug Rules and Reports using Breakpoints</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Remove From Report Delivery</p></td>
<td><p>Click to remove the selected report from all Report Delivery pages and reset the run history metrics.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order in which the target report is processed.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays the <span id="Status" class="popUpLink">status</span> of the target report.</p></td>
</tr>
<tr class="even">
<td><p>REPORT TYPE</p></td>
<td><p>Displays the <span id="Report Type" class="popUpLink">report type</span>.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET REPORT</p></td>
<td><p>Displays the name of the view in SQL corresponding to the target report.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the target report.</p></td>
</tr>
<tr class="odd">
<td><p>ACTION ON</p></td>
<td><p>Displays the last date the report was run.</p></td>
</tr>
<tr class="even">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of records on the target report.</p></td>
</tr>
<tr class="odd">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time Transform took to process the selected target report. If the field is empty, the target report has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
<tr class="even">
<td><p>PUBLISH</p></td>
<td><p>If checked, the report is visible to the Business Users assigned to it.</p>
<p><strong>NOTE:</strong> If Publish is unchecked, only see the Publish, Implication and Recommendation fields display. If Publish is enabled, the Publish, Business User Priority, Sensitive, Implication, Recommendation and Business User Assignment fields display.</p>
<p>Refer to <a href="../Use_Cases/Publish_Reports_to_Report_Delivery_Pages.htm">Publish Reports to Report Delivery Pages</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>TR</p></td>
<td><p>Click to open the <em><a href="Target_Remediation_Overview.htm">Target Remediation Overview</a></em> page to view details about remediation rules applied to an error report. If the icon is active, a remediation rule has been applied to the selected report and the page displays. If the icon is not active, no remediation rule has been applied to the selected report and the page does not display.</p>
<p>Refer to <a href="../Use_Cases/View_Remediation_Rule_Information.htm">View Remediation Rule Information</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>View Report</p></td>
<td><p>Click to view the <em><a href="#">Target Reports</a></em> page to view all columns captured on the report.</p></td>
</tr>
<tr class="odd">
<td><p>Queue</p>
<p> </p></td>
<td><p>Click to open the <em><a href="Monitor_Transform_H.htm">Monitor</a></em> page to monitor the background job processes for the selected target report. If a report has no data to process, this icon is disabled.</p>
<p>Refer to <a href="../Use_Cases/Monitor_Jobs.htm">Monitor Jobs</a> for more information.</p></td>
</tr>
</tbody>
</table>

## <span id="Target_Reports_V_All_Tabs"></span>Target Reports V All Tabs

[Target Reports H](Target_Reports_H.htm)

<div class="use">

Use this page to:

  -  [Add Target Reports](../Use_Cases/Add_Target_Reports.htm)
  - [Create Target Report
    Segments](../Use_Cases/Target_Report_Segments.htm)

</div>

This page has the following tabs:

  - [General tab](#General_Tab5)
  - [Documentation tab](#Documentation_Tab5)
  - [Remediation Information tab](#Remediation_Information)
  - [Process Information tab](#Process_Information_Tab7)
  - [Business User Settings tab](#Business_User_Settings_Tab)
  - [Data Assessment tab](#Data_Assessment)

## <span id="General_Tab5"></span>General tab

Field

Description

Reset

Click to reset the processing status if a process fails for the selected
target report.

Debug

Click to open the *[Debug – Breakpoints](Debug_Breakpoints.htm)* page to
add breakpoints to steps in the process for the selected target,
including target rules and target reports. Use breakpoints to debug
issues with failed processing.

Refer to [Debug Rules and Reports using
Breakpoints](../Use_Cases/Debug_Rules_and_Reports_using_Brkpnts.htm) for
more information.

Report Details

Target Report

Click the link to view the database name and the view definition for the
SQL view corresponding to the selected target report.

Timeframe

Displays the timeframe for the report.

File Location

Click to download the report. If the reporthas not been processed, the
icon is disabled.

Segment By Field

Displays the field in the report that Transform uses to create a
separate report and a sub-directory for each value in this field.

Segments

Click to view the report arranged by the segment selected in Segment by
Field. This icon is disabled if no value has been selected in the
Segment by Field list box or if the report has not yet been processed.

Status Information

Priority

Displays the order the target report is processed.

Status

Displays the <span id="Status" class="popUpLink">status</span> of the
target
report.

## <span id="Documentation_Tab5"></span>Documentation tab

|                       |                                                                                                                                              |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                 | Description                                                                                                                                  |
| Specification Section | Displays the section of the specifications that correspond to the report. This is a free-form text field to store data and is not validated. |
| Description           | Displays a description of the target report.                                                                                                 |
| Comment               | Displays user-entered comments about the selected target report.                                                                             |
| Report Type           | Displays the <span id="Report Type" class="popUpLink">report type</span>.                                                                    |

## <span id="Remediation_Information"></span>Remediation Information tab

Use this page to [Correct Errors in Target Data with Fixed Remediation
Rules.](../Use_Cases/Correct_Errors_in_Target_Data_With_Fixed.htm)

Field

Description

Remediation

Click to open the *[Target Remediation](Target_Remediation_H.htm)* page
to register remediation rules, which are applied to target error reports
to allow data to be loaded into a test environment.

Refer to [View Remediation Rule
Information](../Use_Cases/View_Remediation_Rule_Information.htm) for
more information.

Fixed Remediation

Remediation Status

Displays the <span id="Status" class="popUpLink">status</span> of the
fixed remediation rule.

Remediate Field

Displays the field to which the remediation rule is applied.

Remediate Value

Displays the value to be applied to the remediate field.

Remediation Comment

Displays user-entered comments about the remediation rule.

Fixed Remediation Results

Remediated Count

Displays the number of records affected by the remediation rule.

View Remediated

Click to open the *[Target Reports](#)* page and view the fields
affected by the remediation rule.

## <span id="Process_Information_Tab7"></span>Process Information

Field

Description

Action On

Displays the date Transform processed the selected target report.

Record Count

Displays the number of records on the selected target report.

Duration

Displays the amount of time Transform took to process the selected
target report. If the field is empty, the target report has not been
processed.

**NOTE:** If a process takes less than 0.5 seconds to run, the duration
in the DURATION field is 0.

Process

Click to process the target report in the background. View the status of
background processing on the
*[Monitor](../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm)*
page. 

Refer to [Monitor Jobs](../Use_Cases/Monitor_Jobs.htm) for more
information.

Sampling

Sample Method

Displays the method used on target audit (info type) reports to select
random rows for the users to verify data. Sample Methods are set up in
Transform under Configuration \> Setup on the *[Sampling Methods
(Setup)](Sampling_Methods_Setup.htm)* page.

Refer to [Configure Sampling
Methods](../Config/Configure_Sampling_Methods.htm) for more information.

Sample Record Count

Displays the number of records retrieved using the sampling method.

Sample File Location

Click to download the sampled file. This file contains all the records
prior to sampling. If sample criterion is met, the icon is enabled.

Sample Only

Click to view the sampled records only.

Advanced

Report Format

Displays whether the target report translates the column headings, list
field names for column headings, or displays both. Field names in SAP
are abbreviations in German.

Report Order By

Displays a field to sort the result set in the
report.

## <span id="Business_User_Settings_Tab"></span>Business User Settings tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Publish</p></td>
<td><p>If enabled, the report is published to the report delivery pages. If not enabled, the report is not  published to the report delivery pages.</p>
<p>Refer to <a href="../Use_Cases/Publish_Reports_to_Report_Delivery_Pages.htm">Publish Reports to Report Delivery Pages</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Business User Priority</p></td>
<td><p>Displays the level of importance of the report when displaying it to a business user through the report delivery pages. The options are:</p>
<ul>
<li>Critical</li>
<li>High</li>
<li><span>Low</span></li>
</ul>
<p><strong>NOTE</strong>: This field displays when the Publish check box is checked.</p></td>
</tr>
<tr class="even">
<td><p>Sensitive</p></td>
<td><p>If checked, denotes that the report contains sensitive data that must be restricted from view.</p>
<p>If unchecked, all report content is displayed regardless of sensitivity.</p>
<p><strong>NOTE</strong>: This field displays when the Publish check box is checked.</p></td>
</tr>
<tr class="odd">
<td><p>Implication</p></td>
<td><p>Displays notes about what the implications of the report are.</p></td>
</tr>
<tr class="even">
<td><p>Recommendation</p></td>
<td><p>Displays notes regarding recommendations for fixing the errors (if any) returned by the report.</p></td>
</tr>
<tr class="odd">
<td><p>Business User Assignment</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="All_Reports_All_Users.htm">All Reports All Users</a></span> page to assign or unassign business users access to the report and grant sensitive data access if necessary. The icon only displays of Publish is checked.</p>
<p>Refer to <a href="../Use_Cases/Grant_Users_Access_to_Reports_and_Sensitive_Data.htm#Assign_a_User_to_a_Report_on_Report_Delivery_Pages">Assign a User to a Report</a>  for more information.</p>
<p><strong>NOTE</strong>: This field displays when the Publish check box is checked.</p></td>
</tr>
<tr class="even">
<td><p>Business User Segment Assignment</p></td>
<td><p>Click to open the <em><a href="Target_Reports_Segments.htm">Target Report Segments</a></em> and <em><a href="Target_Report_Segment_User_Assignment.htm">Target Report Segment User Assignment</a></em> pages to assign a user to a target report segment.</p>
<p>The icon only displays if Segment By Field is populated on the General tab and the Publish check box is enabled on the Business User Settings tab.</p>
<p>Refer to <a href="../Use_Cases/Target_Report_Segments.htm#Assign_a_User_to_a_Target_Report_Segment">Assign a User to a Target Report Segment</a> for more information.</p>
<p><strong>NOTE</strong>: This field displays when the Publish check box is checked.</p></td>
</tr>
</tbody>
</table>

## **<span id="Data_Assessment"></span>Data Assessment**

**NOTE**: These fields are reserved for use by the Data Assessment
team.

|                         |                                                                                                                    |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------ |
| Field                   | Description                                                                                                        |
| Candidate               | If checked, reports to be considered for inclusion in the Data Assessment customer deliverable are highlighted.    |
| Internal Comment        | Displays comments reserved for use by the Data Assessment team. Not intended to be communicated to external users. |
| Comment Client Specific | Displays comments that are intended for reporting to the external users as a part of the Data Assessment.          |
