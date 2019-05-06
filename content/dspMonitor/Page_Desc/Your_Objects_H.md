# <span id="YourObjectsH"></span>Your Objects H

[Your Objects V](#YourObjectsV)

<div class="use">

Use this page to [View Your
Objects](../Use_Cases/View_Your_Objects.htm).

</div>

To access this page, select **dspMonitor \> Your Objects** in the
*Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>OBJECT NAME</p></td>
<td><p>Displays the object name.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a description on the object.</p></td>
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
<td><p>Displays the sum of errors on each report assigned to the Object.</p></td>
</tr>
<tr class="odd">
<td><p>DPMO</p></td>
<td><p>Displays the Defects Per Million Opportunities as calculated based on Opportunities and Defects.</p>
<p>(DPMO) = (Total Defects / Total Opportunities) * 1,000,000</p></td>
</tr>
<tr class="even">
<td><p>DEFECT PERCENTAGE</p></td>
<td><p>Displays the defect percentage.</p>
<p>(Total Defects / Total Opportunities) * 100%</p></td>
</tr>
<tr class="odd">
<td><p>DATA QUALITY SCORE</p></td>
<td><p>Displayed the data quality score.</p>
<p>(100 - %Defects)</p></td>
</tr>
<tr class="even">
<td><p>ERROR COST</p></td>
<td><p>Displays the cost of data quality issues for all reports in the object.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays status based on defect percentage and data quality score thresholds. Statuses are Red (critical), Yellow (warning) and Green. Hover over a Status icon to view the threshold.</p>
<p><strong>NOTE:</strong> A Warning icon (yellow triangle) in the Status field indicates that none of the associated reports have an opportunity view, or that in all reports, the number of opportunities is less than the number of number of defects in the rolled up calculations.</p></td>
</tr>
<tr class="even">
<td><p>Reports</p></td>
<td><p>Click to view reports within the object to which you have access.</p></td>
</tr>
</tbody>
</table>

## <span id="YourObjectsV"></span>Your Objects V

[Your Objects H](#YourObjectsH)

<div class="use">

Use this page to [View Your
Objects](../Use_Cases/View_Your_Objects.htm).

</div>

Field

Description

Object Name

Displays the object name.

Description

Displays a description on the object.

Admin

Object Reports

Click to open the *Object Reports* page to [Register Reports to
Objects](../Use_Cases/Register_Object_Reports.htm#Register_Reports_to_Objects)
or [Register Objects to
Reports](../Use_Cases/Register_Object_Reports.htm#Register_Objects_to_Reports).
