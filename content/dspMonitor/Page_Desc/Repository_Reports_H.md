+++
title = ''
solution = 'Data Quality'
+++

# <span id="Repository_Reports_H"></span>Repository Reports H

[Repository Reports V](#Repository_Reports_V)

<div class="use">

Use this page to [Register Reports to a Report
Repository](../Use_Cases/Register_Reports_to_a_Report_Repo.htm).

</div>

To access this page:

1.  Select **dspMonitor \> Configuration \> Report
    Repositories** in *Navigation* pane.
2.  Click **Reports** for Repository.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>REPORT</p></td>
<td><p>Displays name of report as it appears in the report repository. Click link to view SQL code used to generate report.</p></td>
</tr>
<tr class="odd">
<td><p>OPPORTUNITY VIEW</p></td>
<td><p>Displays the name of the opportunity view, which contains the full set of possible records that could potentially fail in the associated error report.</p>
<p><strong>NOTE:</strong> An opportunity view is only applicable to Error reports.</p>
<p>The opportunity view is used in data quality score calculations. When calculating data quality scores on the Your Groups, Your Objects, and Your Applications summary and report pages, error reports without an opportunity view are not included in the data quality scoring calculations.</p>
<p>The opportunity view must include all required key fields of the error report and any fields needed for user filters.</p></td>
</tr>
<tr class="even">
<td><p>STATUS</p></td>
<td><p>Displays status of report for review purposes.</p></td>
</tr>
<tr class="odd">
<td><p>REPORT TYPE</p></td>
<td><p>Displays the categorization of report. Values are: Error, Information and Metric.</p></td>
</tr>
<tr class="even">
<td><p>View Data</p></td>
<td><p>Click to view data within report.</p></td>
</tr>
<tr class="odd">
<td><p>Objects</p></td>
<td><p>Click to manage object reports.</p></td>
</tr>
<tr class="even">
<td><p>Groups</p></td>
<td><p>Click to view groups to which the report belongs.</p></td>
</tr>
<tr class="odd">
<td><p>Target Tables</p></td>
<td><p>Click to open the <em><a href="Report_Target_Tables%20H.htm">Report Target Tables</a></em> page to register target tables to reports.</p></td>
</tr>
</tbody>
</table>

## <span id="Data_Source_Reports_V"></span>Repository Reports Reports V

[Repository Reports H](#Repository_Reports_H)

<div class="use">

Use this page to [Register Reports to a Report
Repository](../Use_Cases/Register_Reports_to_a_Report_Repo.htm).

</div>

This page contains the following tabs:

  - [General tab](#General_Tab)
  - [Metric Data Information tab](#Metric_Data_Information)
  - [Processing Information tab](#Processing_Information)

### <span id="General_Tab"></span>General tab

<div class="use">

Use this tab to [Configure the Business Value
Dashboard](../Use_Cases/Configure_the_Business_Value_Dashboard.htm).

</div>

Field

Description

Report

Displays name of report as it appears in the report repository. Click
link to view SQL code used to generate report.

Report Type

Displays the categorization of report. Values are: Error, Information
and Metric.

Implication

Displays description of what the report means to the business.

Comment

Displays comment or description of report.

Opportunity View

Displays the name of the opportunity view, which contains the full set
of possible records that could potentially fail in the associated error
report.

The opportunity view must include all required key fields of the error
report and any fields needed for user filters.

Data Quality Rule

Displays user-friendly name of report.

Quality Dimension

A Quality Dimension is a recognized term used by data management
professionals to describe a feature of data that can be measured or
assessed against defined standards to determine data quality. Refer to
[Register Quality
Dimensions](../Use_Cases/Populate_Configuration_Tables.htm#Register_Quality_Dimensions)
for more information.

**NOTE:** dspMonitor™ is delivered with six industry standard quality
dimensions: Accuracy, Completeness, Conformity, Integrity, Timeliness
and Uniqueness.

**NOTE:** All Error reports require a quality dimension.

Scorecard Link

This field is not used.

Status

Displays status of report for review purposes.

Allow Manual Run

If checked, report is permitted to be manually run. If unchecked, report
can only be run on a schedule.

Output File Type

Displays type of file generated for reports. Values are File Excel and
File Delimited.

Output File Delimiter

Displays delimiter that separates columns in the report when the report
is outputted.

Report Directory Path

Displays path on the file system (NOT the root of a disk drive) where
reports are stored.

Report Order By

Displays sort value of data to override the SQL Order By.

Report Specification

Click to upload a file about what information the report documents
(i.e., the specifications for the report), which is attached to workflow
emails.

Data Quality Scoring Threshold

Threshold ID

Displays the threshold ID used for data quality scoring.

**NOTE:** If no threshold is selected the threshold ID set on the
*Parameters* page is used in the data quality status calculation. Refer
to [Register Data Quality Score
Thresholds](../Use_Cases/Populate_Configuration_Tables.htm#Register_Data_Quality_Score_Thresholds)
for more information.

Business Value Parameters

Application Currency

Displays the currency set on the *[Parameters](Parameters.htm)* page,
and used for the Cost per Failure calculation on the Business Value
dashboard.

Cost Per Failure

Displays the cost per failure applied to each error record.

**NOTE:** The Cost per Failure value only displays on the Error type
reports (Business Readiness, Target Readiness, and
Error).

### <span id="Metric_Data_Information"></span>Metric Data Information tab

<div class="use">

Use this tab to while [Registering Reports to a Report
Repository](../Use_Cases/Register_Reports_to_a_Report_Repo.htm) and to
[Track Error Records on
Reports](../Use_Cases/Track_Error_Records_on_Reports.htm).

</div>

|                                 |                                                                             |
| ------------------------------- | --------------------------------------------------------------------------- |
| Field                           | Description                                                                 |
| Report Metric Data Build        | If checked, data aging process for the report is activated.                 |
| Report Metric Data Started On   | Displays date and time when data aging process started recording the data.  |
| Report Metric Data Completed On | Displays date and time when data aging process finished recording the data. |
| Metric Data Report              | Click to view the tracked data for the data aging process.                  |
| Report Columns                  | Click to add columns tracked for Metric Data Tracking.                      |
| Process                         | Click to execute the report.                                                |
| Results                         | Click to view results of the metric data report.                            |
| Delete History                  | Click to delete the aged data for the report.                               |

### <span id="Processing_Information"></span>Processing Information tab

|                      |                                                                          |
| -------------------- | ------------------------------------------------------------------------ |
| Field                | Description                                                              |
| Job ID               | Displays Platform job that runs the queued report.                       |
| Process Started On   | Displays date and time when report started running.                      |
| Process Completed On | Displays date and time when report completed running.                    |
| Metrics              | Click to view data about the report, e.g., the last time the report ran. |
| Workflows            | Click to view workflow emails that were sent for the report.             |
