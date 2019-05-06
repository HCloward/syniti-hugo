# <span id="YourAppTbl_H"></span>Your Application Tables H

[Your Application Tables V](#YourAppTbl_V)

<div class="use">

Use this page to:

  - [View Your Application
    Tables](../Use_Cases/View_Your_Application_Tables.htm)
  - [Profile a Target Table in
    dspMonitor](../Use_Cases/Profile_a_Target_Table_in_dspMonitor.htm)

</div>

To access this page:

1.  Select **dspMonitor \> Your Applications** in *Navigation* pane.
2.  Click the **Tables** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>APPLICATION</p></td>
<td><p>Displays the name of the application.</p></td>
</tr>
<tr class="odd">
<td><p>TABLE NAME</p></td>
<td><p>Displays the name of the table.</p></td>
</tr>
<tr class="even">
<td><p>SIGMA LEVEL</p></td>
<td><p>Displays the sigma level based on data quality score calculations.</p>
<p>The Enable Sigma Level checkbox on the <em><a href="Parameters.htm">Parameters</a></em> page must be checked for this field to display.</p></td>
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
<td><p>Displays the cost of data quality issues for all reports based on data in the application table.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays status based on defect percentage and data quality score thresholds. Statuses are Red (critical), Yellow (warning) and Green. Hover over a Status icon to view the threshold.</p>
<p><strong>NOTE:</strong> A Warning icon (yellow triangle) in the Status field indicates that none of the associated reports have an opportunity view, or that in all reports, the number of opportunities is less than the number of number of defects in the rolled up calculations.</p></td>
</tr>
<tr class="even">
<td><p>Columns</p></td>
<td><p>Click to open the <em><a href="Your_Application_Table_Columns.htm">Your Application Table Columns</a></em> page to view data quality information for the columns in the application table.</p></td>
</tr>
<tr class="odd">
<td><p>Reports</p></td>
<td><p>Click to open the <em><a href="Your_Application_Table_Reports_H.htm">Your Application Table Reports</a></em> page to view all application table reports to which the logged in user has access.</p></td>
</tr>
</tbody>
</table>

## <span id="YourAppTbl_V"></span>Your Application Tables V

[Your Application Tables H](#YourAppTbl_H)

<div class="use">

Use this page to:

  - [View Your Application
    Tables](../Use_Cases/View_Your_Application_Tables.htm)
  - [Profile a Target Table in
    dspMonitor](../Use_Cases/Profile_a_Target_Table_in_dspMonitor.htm)

</div>

|             |                                                                                                                                                                                         |
| ----------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field       | Description                                                                                                                                                                             |
| Application | Displays the name of the application.                                                                                                                                                   |
| Table Name  | Displays the name of the table.                                                                                                                                                         |
| Profile     | Click to profile the application table. Refer to [Profile a Target Table in dspMonitor™](../Use_Cases/Profile_a_Target_Table_in_dspMonitor.htm) for information about profiling tables. |
| View Data   | Click to view data within report.                                                                                                                                                       |
| View Fields | Click to open the *[Table Field (Results)](../../../Platform/Common/Page_Desc/Table_Field_Results_H.htm)* page in Common to view the results of a profile run on the table.             |
