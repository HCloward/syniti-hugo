+++
title = 'Target Data Services Reports H <span id="Target_Data_Services_Reports_H"></span>'
solution = 'Migration'
+++

# Target Data Services Reports H <span id="Target_Data_Services_Reports_H"></span>

[Target Data Services Reports V](#Target_Data_Services_Reports_V)

<div class="use">

Use this page to [Grant a User Access to Sensitive Data on Report
Delivery
Pages](../Use_Cases/Grant_Users_Access_to_Reports_and_Sensitive_Data.htm#Grant_a_User_Access_to_Sensitive_Data_on_Report_Delivery_Pages).

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. Refer to [Use Bulk
Execution](../../../Platform/Bulk_Exec/Use_Bulk_Execution.htm) for more
information.

To access this page in Transform:

1.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](Process_Area_Launch.htm)* page.
2.  Click the <span style="font-weight: bold;">Data Services
    Reports</span> icon for a Target.

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
<td><p>Click to open the <em><a href="Debug_Breakpoints.htm">Debug – Breakpoints</a></em> page to add breakpoints to steps in the process for the selected target, including target rules and target reports. Use breakpoints to debug issues with failed processing.</p></td>
</tr>
<tr class="odd">
<td><p>Remove From Report Delivery</p></td>
<td><p>Click to unpublish/remove the selected report from all Report Delivery pages and reset the run history metrics.</p></td>
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
<td><p>TARGET DATA SERVICES REPORT</p></td>
<td><p>Displays the name of the report.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the report.</p></td>
</tr>
<tr class="odd">
<td><p>ACTION ON</p></td>
<td><p>Displays the date Transform processed the selected Target Data Services report.</p></td>
</tr>
<tr class="even">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of records on the selected target Data Services report.</p></td>
</tr>
<tr class="odd">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time Transform took to process the selected Target Data Services report. If the field is empty, the target report has not been processed.</p></td>
</tr>
<tr class="even">
<td><p>PUBLISH</p></td>
<td><p>If checked, the report is published to the report delivery pages.</p>
<p>If unchecked, the report will not be published to the report delivery pages.</p></td>
</tr>
<tr class="odd">
<td><p>TR</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Target_Remediation_Overview.htm">Target Remediation Overview</a></span> page to view details about remediation rules applied to an error report for any reports associated with the selected target.</p>
<p>If the icon is active, the count displays the total number of fixed remediation and remediation rules applied to reports. If the icon is disabled, no remediation rules have been applied to any reports associated with the selected target.</p></td>
</tr>
<tr class="even">
<td><p>View Target</p></td>
<td><p>Click to display the <span style="font-style: italic;"><a href="Targets_H.htm">Targets</a></span> page where the records of the target table are viewed.</p></td>
</tr>
<tr class="odd">
<td><p>Queue</p></td>
<td><p>Click to display the <span style="font-style: italic;"><a href="Monitor_Transform_H.htm">Monitor</a></span> page where the current Transform jobs can be viewed as they execute</p></td>
</tr>
</tbody>
</table>

## <span id="Target_Data_Services_Reports_V"></span>Target Data Services Reports V

[Target Data Services Reports H](#Target_Data_Services_Reports_H)

This page has the following tabs:

  - [General tab](#General_Tab)
  - [Documentation tab](#Documentation_Tab)
  - [Remediation Information tab](#Remediation_Information_Tab)
  - [Process Information tab](#Process_Information_Tab)
  - [Business User Settings](#Business_User_Settings_Tab)

## <span id="General_Tab"></span>General tab

Field

Description

Debug

Click to open the *[Debug – Breakpoints](Debug_Breakpoints.htm)* page to
add breakpoints to steps in the process for the selected target,
including target rules and target reports. Use breakpoints to debug
issues with failed processing.

Report Details

Target Data Services Report

Click the link to view the database name and the view definition for the
SQL view corresponding to the selected target report.

Timeframe

Displays the time frame for the report.

File Location

Click to download the report. If it has not been processed, the icon is
disabled.

Segment By Field

Displays the field in the report that Transform uses to create a
separate report and a sub-directory for each value in this field.

Segments

Click to view the report grouped by the segment selected in Segment by
Field. This icon is disabled if no value has been selected in the
Segment by Field list box or if the report has not yet been processed.

Status Information

Priority

Displays the order the target report is processed.

Status

Displays the <span id="Status" class="popUpLink">status</span> of the
target
report.

## <span id="Documentation_Tab"></span>Documentation tab

|                       |                                                                                                                                              |
| --------------------- | -------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                 | Description                                                                                                                                  |
| Specification Section | Displays the section of the specifications that correspond to the report. This is a free-form text field to store data and is not validated. |
| Description           | Displays a description of the target report.                                                                                                 |
| Comment               | Displays user-entered comments about the selected target report.                                                                             |
| Report Type           | Displays the <span id="Report Type" class="popUpLink">report type</span>.                                                                    |

## <span id="Remediation_Information_Tab"></span>Remediation Information tab

Field

Description

Remediation

Click to open the *[Target Remediation](Target_Remediation_H.htm)* page
to register remediation rules, which are applied to target error reports
to allow data to be loaded into a test environment.

Fixed Remediation

Remediation Status

Displays the status of the fixed remediation rule.

Remediate Field

Displays the field to which the remediation rule will be applied.

Remediate Value

Displays the value to be applied to the remediate field.

Remediation Comment

Displays user-entered comments about the remediation rule.

Fixed Remediation Results

Remediated Count

Displays the number of records affected by the remediation rule.

View Remediated

Click to view the fields that were affected by the remediation rule.

## <span id="Process_Information_Tab"></span>Process Information tab

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

Process

Click to process the target report in the background. View the status of
background processing on the
*[Monitor](../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm)*
page. 

Sampling

Sample Method

Displays the method used on target audit (info type) reports to select
random rows for the users to verify data. Sample Methods are set up in
Transform under Configuration \> Setup on the *[Sampling Methods
(Setup)](Sample_Sizes_Setup.htm)* page.

Sample Record Count

Displays the number of records retrieved using the sampling method.

Sample File Location

Click to download the file that was sampled. This file contains all the
records prior to sampling. If the sample criterion is met, the icon is
enabled.

Sample Only

Click to view the sampled records only.

Advanced

Report Format

Displays whether the target report will translate the column headings,
list field names for column headings, or display both. Field names in
SAP are abbreviations in German.

Report Order By

Displays the field used to sort the result set in the
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
<td><p>If checked, the report is published to the Report Delivery pages</p></td>
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
<p>If unchecked, all report content will be displayed regardless of sensitivity.</p>
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
</tbody>
</table>
