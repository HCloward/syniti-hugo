+++
title = 'Your Application Table Columns'
solution = 'Data Quality'
+++

# Your Application Table Columns

<div class="use">

Use this page to [View Your Application Table
Columns](../Use_Cases/View_Your_Application_Table_Columns).

</div>

To access this page:

1.  Select **dspMonitor \> Your Applications** in the *Navigation* pane.
2.  Click the **Tables** icon.
3.  Click the **Columns** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>TABLE NAME</p></td>
<td><p>Display the name of the table.</p></td>
</tr>
<tr class="odd">
<td><p>COLUMN NAME</p></td>
<td><p>Displays the name of the column.</p></td>
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
<td><p>Displays the data quality score.</p>
<p>(100 - %Defects)</p></td>
</tr>
<tr class="even">
<td><p>ERROR COST</p></td>
<td><p>Displays the cost of data quality issues for all reports based on data in the application table columns.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays status based on defect percentage and data quality score thresholds. Statuses are Red (critical), Yellow (warning) and Green. Hover over a Status icon to view the threshold.</p>
<p><strong>NOTE:</strong> A Warning icon (yellow triangle) in the Status field indicates that none of the associated reports have an opportunity view, or that in all reports, the number of opportunities is less than the number of number of defects in the rolled up calculations.</p></td>
</tr>
<tr class="even">
<td><p>Reports</p></td>
<td><p>Click to open the <em><a href="Your_Application_Table_Column_Reports_H">Your Application Table Column Reports</a></em> page to view the reports.</p></td>
</tr>
</tbody>
</table>
