+++
title = 'Your Object Reports H'
solution = 'Data Quality'
+++

# Your Object Reports H

**NOTE:** When a user accesses this page in the *Navigation* pane, the
fields below display. When a user clicks the View icon on this page to
view report data, the report title still displays as the page name even
though columns that display depend on the columns on the generated
report. In this case, the page displays the report’s columns only and
not the fields below.

[Your Object Reports V](#YourObjectRptV)

<div class="use">

Use this page to [View Your Object
Reports](../Use_Cases/View_Your_Object_Reports).

</div>

To access this page:

1.  Select **dspMonitor \> Your Objects** in the *Navigation* pane
2.  Click the **Reports** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Your Favorite</p></td>
<td><p>Displays a green check if the report has been added to the <em>Your Favorite Reports</em> page.</p></td>
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
</tbody>
</table>

## <span id="YourObjectRptV"></span>Your Object Reports V

[Your Object Reports H](#YourObjectRptH)

<div class="use">

Use this page to [View Your Object
Reports](../Use_Cases/View_Your_Object_Reports).

</div>

This page contains the following tabs:

  - [General](#General)
  - [Report Generation Info tab](#Report)

## <span id="General"></span>General tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Repository</p></td>
<td><p>Displays the name of the database where reports reside.</p></td>
</tr>
<tr class="odd">
<td><p>Report</p></td>
<td><p>Displays the name of the report as it appears in the repository.</p></td>
</tr>
<tr class="even">
<td><p>Opportunity View</p></td>
<td><p>Displays the name of the opportunity view, which contains the full set of possible records that could potentially fail in the associated error report.</p>
<p><strong>NOTE:</strong> An opportunity view is only applicable to Error reports.</p>
<p>The opportunity view is used in data quality score calculations. When calculating data quality scores on the Your Groups, Your Objects, and Your Applications summary and report pages, error reports without an opportunity view are not included in the data quality scoring calculations.</p>
<p>The opportunity view must include all required key fields of the error report and any fields needed for user filters.</p></td>
</tr>
<tr class="odd">
<td><p>Quality Dimension</p></td>
<td><p>A Quality Dimension is a recognized term used by data management professionals to describe a feature of data that can be measured or assessed against defined standards to determine data quality. Refer to <a href="../Use_Cases/Populate_Configuration_Tables#Register_Quality_Dimensions">Register Quality Dimensions</a> for more information.</p>
<p><strong>NOTE:</strong> dspMonitor™ is delivered with six industry standard quality dimensions: Accuracy, Completeness, Conformity, Integrity, Timeliness and Uniqueness.</p>
<p><strong>NOTE:</strong> All Error reports require a quality dimension.</p></td>
</tr>
<tr class="even">
<td><p>Report Type</p></td>
<td><p>Displays the categorization of report. Values are: Error, Information and Metric.</p></td>
</tr>
<tr class="odd">
<td><p>Data Quality Rule</p></td>
<td><p>Displays the name of the report.</p></td>
</tr>
<tr class="even">
<td><p>Implication</p></td>
<td><p>Displays description of what the report means to the business.</p></td>
</tr>
<tr class="odd">
<td><p>Comment</p></td>
<td><p>Displays comment or description about report.</p></td>
</tr>
<tr class="even">
<td><p>Scorecard Link</p></td>
<td><p>This field is not used.</p></td>
</tr>
<tr class="odd">
<td><p>Where Clause</p></td>
<td><p>Displays filter applied to report for user to limit data displayed in report.</p></td>
</tr>
<tr class="even">
<td><p>Order By</p></td>
<td><p>Displays columns by which the report is sorted.</p></td>
</tr>
</tbody>
</table>

## <span id="Report"></span>Report Generation Info tab

|                      |                                                                                                                                                          |
| -------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                | Description                                                                                                                                              |
| Opportunity Count    | Displays the number of records in the opportunity view, which contains the full set of possible records that could potentially fail in the error report. |
| Defects              | Displays the number of errors on the report.                                                                                                             |
| Process Started On   | Displays date and time when report started running.                                                                                                      |
| Process Completed On | Displays date and time when report completed running.                                                                                                    |
| View                 | Click to view data within report.                                                                                                                        |
