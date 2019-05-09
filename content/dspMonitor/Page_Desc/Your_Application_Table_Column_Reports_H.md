+++
title = 'Your Application Table Column Reports H'
solution = 'Data Quality'
+++

# Your Application Table Column Reports H

**NOTE:** When a user accesses this page in the *Navigation* pane, the
fields below display. When a user clicks the View icon on this page to
view report data, the report title still displays as the page name even
though columns that display depend on the columns on the generated
report. In this case, the page displays the report’s columns only and
not the fields below.

[Your Application Table Column Reports V](#TblClmRpt_V)

<div class="use">

Use this page to:

  - [View Your Application Table Column
    Reports](../Use_Cases/View_Your_Application_Table_Column_Reports)
  - [Manually Process Single Application Table Column
    Report](../Use_Cases/Process_Reports#Manually_Process_Single_Application_Table_Column_Report)

</div>

To access this page:

1.  Click **dspMonitor \> Your Applications** in the *Navigation* pane.
2.  Click the **Tables** icon.
3.  Click the **Columns** icon.
4.  Click the **Reports** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>GROUP ID</p></td>
<td><p>Displays name of group to which the report belongs.</p></td>
</tr>
<tr class="odd">
<td><p>QUALITY DIMENSION</p></td>
<td><p>A Quality Dimension is a recognized term used by data management professionals to describe a feature of data that can be measured or assessed against defined standards to determine data quality. Refer to <a href="../Use_Cases/Populate_Configuration_Tables#Register_Quality_Dimensions">Register Quality Dimensions</a> for more information.</p>
<p><strong>NOTE:</strong> dspMonitor™ is delivered with six industry standard quality dimensions: Accuracy, Completeness, Conformity, Integrity, Timeliness and Uniqueness.</p>
<p><strong>NOTE:</strong> All Error reports require a quality dimension.</p></td>
</tr>
<tr class="even">
<td><p>DATA QUALITY RULE</p></td>
<td><p>Displays the name of the report.</p></td>
</tr>
<tr class="odd">
<td><p>REPORT TYPE</p></td>
<td><p>Displays the categorization of report. Values are: Error, Information and Metric.</p></td>
</tr>
<tr class="even">
<td><p>SIGMA LEVEL</p></td>
<td><p>Displays the sigma level based on data quality score calculations.</p>
<p>The Enable Sigma Level checkbox on the <em><a href="Parameters">Parameters</a></em> page must be checked for this field to display.</p></td>
</tr>
<tr class="odd">
<td><p>OPPORTUNITIES</p></td>
<td><p>Displays the number of records in the opportunity view, which contains the full set of possible records that could potentially fail in the error report.</p></td>
</tr>
<tr class="even">
<td><p>DEFECTS</p></td>
<td><p>Displays the number of errors on the report.</p></td>
</tr>
<tr class="odd">
<td><p>DPMO</p></td>
<td><p>Displays the Defects Per Million Opportunities as calculated based on Opportunities and Defects.</p>
<p>DPMO = (Total Defects / Total Opportunities) * 1,000,000</p></td>
</tr>
<tr class="even">
<td><p>DEFECT PERCENTAGE</p></td>
<td><p>Displays the defect percentage.</p>
<p>(Total Defects / Total Opportunities)* 100%</p></td>
</tr>
<tr class="odd">
<td><p>DATA QUALITY SCORE</p></td>
<td><p>Displayed the data quality score.</p>
<p>(100 - %Defects)</p></td>
</tr>
<tr class="even">
<td><p>ERROR COST</p></td>
<td><p>Displays the cost of data quality issues for the report.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays status based on defect percentage and data quality score thresholds. Statuses are Red (critical), Yellow (warning) and Green. Hover over a Status icon to view the threshold.</p>
<p><strong>NOTE:</strong> A Warning icon (yellow triangle) in the Status field indicates the error report does not have an assigned opportunity view, or that the number of opportunities is less than the number of number of defects in the rolled up calculations for the report.</p></td>
</tr>
<tr class="even">
<td><p>View</p></td>
<td><p>Click to view data within report.</p></td>
</tr>
<tr class="odd">
<td><p>Download a file</p></td>
<td><p>Click to download a file that contains the report data.</p></td>
</tr>
<tr class="even">
<td><p>Metrics</p></td>
<td><p>Click to open the Your Report Metrics Chart to view a line chart of the report’s record count history and the <em><a href="Your_Metrics">Your Metrics</a></em> page to view data about the report, e.g., the last time the report was processed.</p></td>
</tr>
</tbody>
</table>

## <span id="TblClmRpt_V"></span>Your Application Table Column Reports V

[Your Application Table Column Reports H](#TblClmRpt_H)

<div class="use">

Use this page to.

  - [View Your Application Table Column
    Reports](../Use_Cases/View_Your_Application_Table_Column_Reports)
  - [Manually Process Single Application Table Column
    Report](../Use_Cases/Process_Reports#Manually_Process_Single_Application_Table_Column_Report)

</div>

This page contains the following tabs:

  - [General tab](#General)
  - [Report Generation Info tab](#Report)

## <span id="General"></span>General tab

Field

Description

Execute

Click to process the report for the logged in user.

Execute For All Users

Click to process the reports for all users who have access to the
reports.

Reset

Click to reset running report. Reset report if process backs up due to
network problems.

Report Info

Repository

Displays name of database where reports reside.

Group ID

Displays name of group to which the report belongs.

Report

Displays name of report as it appears in the report repository.

Opportunity View

Displays the name of the opportunity view, which contains the full set
of possible records that could potentially fail in the associated error
report.

**NOTE:** An opportunity view is only applicable to Error reports.

The opportunity view is used in data quality score calculations. When
calculating data quality scores on the Your Groups, Your Objects, and
Your Applications summary and report pages, error reports without an
opportunity view are not included in the data quality scoring
calculations.

The opportunity view must include all required key fields of the error
report and any fields needed for user filters.

Quality Dimension

Displays the Quality Dimension, an industry- recognized term used by
data management professionals to describe a feature of data that can be
measured or assessed against defined standards to determine data
quality. Refer to [Register Quality
Dimensions](../Use_Cases/Populate_Configuration_Tables#Register_Quality_Dimensions)
for more information.

**NOTE:** dspMonitor™ is delivered with six industry standard quality
dimensions: Accuracy, Completeness, Conformity, Integrity, Timeliness
and Uniqueness.

**NOTE:** All Error reports require a quality dimension.

Report Type

Displays the categorization of report. Values are: Error, Information
and Metric.

Data Quality Rule

Displays the name of the report.

Implication

Displays description of what the report means to the business.

Comment

Displays comment or description about report.

Scorecard Link

This field is not used.

Where Clause

Displays filter applied to report for user to limit data displayed in
report.

Order By

Displays columns by which the report is sorted.

Favorite Settings

Favorite

If enabled, the selected report has been added as a favorite report and
displays on the *[Your Favorite Reports](Your_Favorite_Reports_H)*
page.

## <span id="Report"></span>Report Generation Info tab

Field

Description

Opportunity Count

Displays the number of records in the opportunity view, which contains
the full set of possible records that could potentially fail in the
error report.

Defects

Displays the number of errors on the report.

Process Started On

Displays date and time when report started running.

Process Completed On

Displays date and time when report completed running.

Queue

Click to open the *[Monitor](Monitor_H)* page to view the process
queue for reports.

View

Click to view data within report.

Metric Info

Latest Metric Date

Displays date when metrics were last built.

Metrics

Click to open the Your Report Metrics Chart to view a line chart of the
report’s record count history and the *[*Your
Metrics*](Your_Metrics)* page to view data about the report, e.g.,
the last time the report was processed.

Reset Metrics

Click to clear metrics for the report. If the report is run more than
once within a 24-hour period, the previous metrics are overwritten.
