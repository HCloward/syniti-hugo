# Target Source Reports H

[Target Source Reports V All Tabs](#Target_Source_Reports_V)

<div class="use">

Use this page to:

  - [Add Target Source
    Reports](../Use_Cases/Add_Target_Source_Reports.htm)
  - [Publish Reports to Report Delivery
    Pages](../Use_Cases/Publish_Reports_to_Report_Delivery_Pages.htm)

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. See the Bulk Execution topic in System
Administration for more information.

To access this page in Transform:

1.  Select the **Targets** icon on the *[Process Area
    Launch](Process_Area_Launch.htm)* page.
2.  Click the **Sources** icon for a Target.
3.  Click the **Reports** icon for a Target Source.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Execute</p></td>
<td><p>Click to run the selected Target Source report immediately in the foreground.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset the processing status if a process fails for the selected Target Source report.</p></td>
</tr>
<tr class="even">
<td><p>Debug</p></td>
<td><p>Click to open the <a href="Debug_Breakpoints_Target_Sources.htm"><em>Debug – Breakpoints (Target Sources)</em></a> page to add breakpoints to steps in the process for the selected Target Source for Target Source rules and Target Source reports. Use breakpoints to debug issues with failed processing.</p></td>
</tr>
<tr class="odd">
<td><p>Remove From Report Delivery</p></td>
<td><p>Click to unpublish/remove the selected report from all Report Delivery pages and reset the run history metrics.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the Target Source report is processed.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays the <span id="Status" class="popUpLink">status</span> of the Target Source report.</p></td>
</tr>
<tr class="even">
<td><p>REPORT TYPE</p></td>
<td><p>Displays the <span id="Report Type" class="popUpLink">report type</span>.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description of the Target Source report.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE REPORT</p></td>
<td><p>Click the link to view the database name and the view definition for the SQL view corresponding to the selected Target Source report.</p></td>
</tr>
<tr class="odd">
<td><p>ACTION ON</p></td>
<td><p>Displays the last date the source report was processed.</p></td>
</tr>
<tr class="even">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of records on the Target Source report.</p></td>
</tr>
<tr class="odd">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time Transform took to process the selected Target Source report. If the field is empty, the Target Source report has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
<tr class="even">
<td><p>PUBLISH</p></td>
<td><p>If checked, the report is visible to the Business Users assigned to it.</p></td>
</tr>
<tr class="odd">
<td><p>View Report</p></td>
<td><p>Click to view the <em><a href="#">Target Source Reports</a></em> page to view details about the source.</p></td>
</tr>
<tr class="even">
<td><p>Queue</p></td>
<td><p>Click to open the <em><a href="Monitor_Transform_H.htm">Monitor</a></em> page to monitor the background job processes for the selected Target Source report. If a report has no data to process, this button is disabled.</p></td>
</tr>
</tbody>
</table>

###  

## <span id="Target_Source_Reports_V"></span>Target Source Reports V All Tabs

[Target Source Reports H](Target_Source_Reports_H.htm)

<div class="use">

Use this page to [Add Target Source
Reports](../Use_Cases/Add_Target_Source_Reports.htm).

</div>

This page has the following tabs:

  - [General tab](#General_Tab3)
  - [Documentation tab](#Documentation_Tab3)
  - [Process Information tab](#Process_Information_Tab3)
  - [Business User Settings tab](#Business_User_Settings_Tab)
  - [Data Assessment tab](#Data_Assessment)

## <span id="General_Tab3"></span>General tab

Field

Description

Debug

Click to open the *[Debug – Breakpoints](Debug_Breakpoints.htm)* page to
add breakpoints to steps in the process for the selected Target Source
for Target Source rules and Target Source reports. Use breakpoints to
debug issues with failed processing.

Source Report

Click the link to view the database name and the view definition for the
SQL view corresponding to the selected Target Source report.

Report Details

Timeframe

Displays the timeframe for the report.

File Location

Click to download the report. If it has not been processed, the icon is
disabled.

Segment By Field

Displays the field in the report that Transform uses to create a
separate report and a sub-directory for each value in this field.

Segments

Click to view the report arranged by the segment selected in Segment by
Field. This icon is disabled if no value has been selected in the
Segment by Field list box or if the report has not yet been processed.

Status Information

Priority

Displays the order the Target Source report is processed.

Status

Displays the <span id="Status" class="popUpLink">status</span> of the
Target Source
report.

## <span id="Documentation_Tab3"></span>Documentation tab

|             |                                                                         |
| ----------- | ----------------------------------------------------------------------- |
| Field       | Description                                                             |
| Description | Displays a user-entered description about the Target Source report.     |
| Comment     | Displays user-entered comments about the selected Target Source report. |

## <span id="Process_Information_Tab3"></span>Process Information tab

Field

Description

Action On

Displays the date Transform processed the selected Target Source report.

Record Count

Displays the number of records on the selected Target Source report.

Duration

Displays the amount of time Transform took to process the selected
Target Source report. If the field is empty, the Target Source report
has not been processed.

**NOTE:** If a process takes less than 0.5 seconds to run, the duration
in the DURATION field is 0.

Reset

Click to reset the processing status if a process fails for the selected
Target Source report.

Process

Click to process the Target Source report in the background. View the
status of background processing on the
*[Monitor](../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm)*
page.

Sampling

Sample Method

Displays the method used on target audit (info type) reports to select
random rows for the users to verify data. Sample Methods are set up in
Transform under Configuration \> Setup on the *[Sampling Methods
(Setup)](Sampling_Methods_Setup.htm)* page.

Sample Record Count

Displays the number of records retrieved using the sampling method.

Sample File Location

Click to download the file that was sampled. This file contains all the
records prior to sampling. If sample criterion is met, the icon is
enabled.

Sample Only

Click to view the sampled records only.

Advanced

Report Format

Displays whether the Target Source report will translate the column
headings, list field names for column headings, or display both. Field
names in SAP are abbreviations in German.

Report Order By

Displays the field to sort the result set in the Target Source
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
<td><p>If checked, the report is published to the report delivery pages. If unchecked, the report will not be published to the report delivery pages.</p></td>
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
<td><p>If checked, denotes that the report contains sensitive data that should be restricted from view.</p>
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

## **<span id="Data_Assessment"></span>Data Assessment**

**NOTE:** These fields are reserved for use by the Data Assessment
team.

|                         |                                                                                                                           |
| ----------------------- | ------------------------------------------------------------------------------------------------------------------------- |
| Field                   | Description                                                                                                               |
| Candidate               | If enabled, reports that should be considered to be included in the Data Assessment customer deliverable are highlighted. |
| Internal Comment        | Displays comments reserved for use by the Data Assessment team.  Not intended to be communicated to external users.       |
| Comment Client Specific | Displays comments that are intended for reporting to the external users as a part of the Data Assessment.                 |
