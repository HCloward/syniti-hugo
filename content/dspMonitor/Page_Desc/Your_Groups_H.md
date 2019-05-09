+++
title = 'Your Groups H'
solution = 'Data Quality'
+++

# Your Groups H

[Your Groups V](#Your_Groups_V)

<div class="use">

Use this page to:

  - [Manually Process Group
    Reports](../Use_Cases/Process_Reports#Manually_Process_Group_Reports)
  - [View Your Groups](../Use_Cases/View_Your_Groups)

</div>

To access this page, select <span style="font-weight: bold;">dspMonitor
\> </span>**Your Groups** in *Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Process</p></td>
<td><p>Click to process your reports within the group.</p></td>
</tr>
<tr class="odd">
<td><p>Process For All Users</p></td>
<td><p>Click to process all the reports within the group for all users who have access to the reports.</p></td>
</tr>
<tr class="even">
<td><p>Reset</p></td>
<td><p>Click to reset running report. Reset report if process backs up due to network problems.</p></td>
</tr>
<tr class="odd">
<td><p>GROUP ID</p></td>
<td><p>Displays name of report group.</p></td>
</tr>
<tr class="even">
<td><p>GROUP DESCRIPTION</p></td>
<td><p>Displays description of report group.</p></td>
</tr>
<tr class="odd">
<td><p>SIGMA LEVEL</p></td>
<td><p>Displays the sigma level based on data quality score calculations.</p>
<p>The Enable Sigma Level checkbox on the <em><a href="Parameters">Parameters</a></em> page must be checked for this field to display.</p></td>
</tr>
<tr class="even">
<td><p>OPPORTUNITIES</p></td>
<td><p>Displays the number of records in the opportunity view, which contains the full set of possible records that could potentially fail in the error report.</p></td>
</tr>
<tr class="odd">
<td><p>DEFECTS</p></td>
<td><p>Displays the sum of errors on each report assigned to the Group</p></td>
</tr>
<tr class="even">
<td><p>DPMO</p></td>
<td><p>Displays the Defects Per Million Opportunities as calculated based on Opportunities and Defects.</p>
<p>(DPMO) = (Total Defects / Total Opportunities) * 1,000,000</p></td>
</tr>
<tr class="odd">
<td><p>DEFECT PERCENTAGE</p></td>
<td><p>Displays the defect percentage.</p>
<p>(Total Defects / Total Opportunities)* 100%</p></td>
</tr>
<tr class="even">
<td><p>DATA QUALITY SCORE</p></td>
<td><p>Displayed the data quality score.</p>
<p>(100 - %Defects)</p></td>
</tr>
<tr class="odd">
<td><p>ERROR COST</p></td>
<td><p>Displays the cost of data quality issues for all reports in the group.</p></td>
</tr>
<tr class="even">
<td><p>STATUS</p></td>
<td><p>Displays status based on defect percentage and data quality score thresholds. Statuses are Red (critical), Yellow (warning) and Green. Hover over a Status icon to view the threshold.</p>
<p><strong>NOTE:</strong> A Warning icon (yellow triangle) in the Status field indicates that none of the associated reports have an opportunity view, or that in all reports, the number of opportunities is less than the number of number of defects in the rolled up calculations.</p></td>
</tr>
<tr class="odd">
<td><p>Favorites</p></td>
<td><p>Click to open the <em>Your Favorite Reports</em> page to view a list of reports in the selected group that have been marked as favorites for the current user.</p>
<p>The number on the icon represents the count of favorite reports in the current group that have been added for the current user.</p>
<p>Refer to <a href="../Use_Cases/View_Your_Favorite_Reports">View Your Favorite Reports</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Reports</p></td>
<td><p>Click to view reports within group to which you have access.</p></td>
</tr>
<tr class="odd">
<td><p>Metrics</p></td>
<td><p>Click to open the <em><a href="../Use_Cases/View_Your_Group_Metrics_Chart">Your Group Metrics</a></em> page to the metrics chart for your group.</p></td>
</tr>
<tr class="even">
<td><p>Queue</p></td>
<td><p>Click to view the process queue of reports.</p></td>
</tr>
</tbody>
</table>

## <span id="Your_Groups_V"></span>Your Groups V

[Your Groups H](Your_Groups_H)

<div class="use">

Use this page to:

  - [Manually Process Group
    Reports](../Use_Cases/Process_Reports#Manually_Process_Group_Reports)
  - [View Your Groups](../Use_Cases/View_Your_Groups)

</div>

Field

Description

Group ID

Displays name of report group.

Group Description

Displays description of report group.

Group Owner

Displays individual whose task is to manage reports registered to the
group and to define the report-level parameters.

Admin

User

Click to open the <span style="font-style: italic;">[Group
Users](Group_Users)</span> page to manage users who have security to
view reports within the group. Icon is only available if the current
user is the group owner for the group.

Group Reports

Click to open the [<span style="font-style: italic;">Group
Reports</span>](Group_Reports_H) page to manage reports within
group. Icon is only available of the current user is the group owner for
the group.
