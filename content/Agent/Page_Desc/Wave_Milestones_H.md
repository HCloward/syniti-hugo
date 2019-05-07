+++
title = ''
solution = 'Platform'
+++

# <span id="top"></span>Wave Milestones H

[Wave Milestones V](#Wave)

<div class="use">

Use this page to [Configure the IGC Migration
dashboard](../Use_Cases/Configure_the_Migration_Dashboard.htm).

</div>

To access this page:

1.  Select **Agent Interface \> Dashboards \> Migration Dashboard** in
    the *Navigation* pane.
2.  Click the **Milestones** icon for a wave.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the name of the milestone.</p></td>
</tr>
<tr class="odd">
<td><p>ABBREVIATION</p></td>
<td><p>Displays a four-character abbreviation of the milestone name that displays on the Migration dashboard.</p></td>
</tr>
<tr class="even">
<td><p>MILESTONE DATE</p></td>
<td><p>Displays the date of the milestone used in metrics calculations.</p>
<p><strong>NOTE</strong>: A milestone added for the current date does not display on the Migration dashboard.</p></td>
</tr>
<tr class="odd">
<td><p>REQUIRED</p></td>
<td><p>If checked, the milestone cannot be deleted. The Start Date and End Date milestones, added by default when the user checks the Send Wave And Milestone Metrics check box on the <em><a href="Wave_Identification_H.htm">Wave Identification</a></em> page, have this check box checked. The check box cannot be checked for any other milestones.</p>
<p>If unchecked, the milestone can be deleted.</p></td>
</tr>
<tr class="even">
<td><p>DESIGN COMPLETE UPPER THRESHOLD</p></td>
<td><p>Displays the percentage to be compared with the Design Complete metric percentage calculation. If the percentage calculation is equal to or greater than the upper threshold percentage, this milestone is complete and the detail row for the Design Complete metric displays green on the dashboard.</p>
<p><strong>NOTE:</strong> Design Complete indicates how much of the design work has been completed. This percentage is calculated as the total number of active fields within active targets where design is complete (the design status is Design Complete or Finished) divided by the total number of active fields within active targets, regardless of design status.</p></td>
</tr>
<tr class="odd">
<td><p>DESIGN COMPLETE LOWER THRESHOLD</p></td>
<td><p>Displays the percentage to be compared with the Design Complete metric percentage calculation. If the percentage calculation is between the upper and lower thresholds, the detail row for the metric displays light blue. If the percentage calculation is less than or equal to the lower threshold, the detail row for the metric displays red.</p></td>
</tr>
<tr class="even">
<td><p>MAPPING COMPLETE UPPER THRESHOLD</p></td>
<td><p>Displays the percentage to be compared with the Mapping Complete metric percentage calculation. If the percentage calculation is equal to or greater than the upper threshold percentage, this milestone is complete and the detail row for the Mapping Complete metric displays green on the dashboard.</p>
<p><strong>NOTE:</strong> Mapping Complete indicates how much of the field mapping and value mapping work has been completed. This percentage is calculated as the total number of total mappings opportunities for both value and field mapping divided by the total number of mappings in Complete status.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPING COMPLETE LOWER THRESHOLD</p></td>
<td><p>Displays the percentage to be compared with the Mapping Complete metric percentage calculation. If the percentage calculation is between the upper and lower thresholds, the detail row for the metric displays light blue. If the percentage calculation is less than or equal to the lower threshold, the detail row for the metric displays red.</p></td>
</tr>
<tr class="even">
<td><p>RULES COMPLETE UPPER THRESHOLD</p></td>
<td><p>Displays the percentage to be compared with the Rules Complete metric percentage calculation. If the percentage calculation is equal to or greater than the upper threshold percentage, this milestone is complete and the detail row for the Rules Complete metric displays green on the dashboard.</p>
<p><strong>NOTE:</strong> Rules Complete indicates how many of the rules have been completed. This percentage is calculated by the total number of source and target rules for the active fields with a rule status of Complete divided by the total number of source and target rules (also called rule opportunities).</p></td>
</tr>
<tr class="odd">
<td><p>RULES COMPLETE LOWER THRESHOLD</p></td>
<td><p>Displays the percentage to be compared with the Rules Complete metric percentage calculation. If the percentage calculation is between the upper and lower thresholds, the detail row for the metric displays light blue. If the percentage calculation is less than or equal to the lower threshold, the detail row for the metric displays red.</p></td>
</tr>
<tr class="even">
<td><p>QUALITY UPPER THRESHOLD</p></td>
<td><p>Displays the percentage to be compared with the Quality metric percentage calculation. If the percentage calculation is equal to or greater than the upper threshold percentage, this milestone is complete and the detail row for the Quality metric displays green on the dashboard.</p>
<p><strong>NOTE:</strong> Quality indicates the data quality of the wave. This percentage is calculated using the totals on the error reports registered to the wave and targets (post load reports) divided by the total number of records on the opportunity reports registered to the waves and targets (preload reports).</p>
<p><strong>NOTE:</strong> The reports used in this calculation are registered on the <em><a href="Data_Quality_Report_Assignment.htm">Data Quality Report Assignment</a></em> page.</p>
<p><strong>NOTE:</strong> This percentage has 7 decimal positions to support a six sigma-level quality definition.</p></td>
</tr>
<tr class="odd">
<td><p>QUALITY LOWER THRESHOLD</p></td>
<td><p>Displays the percentage to be compared with the Quality metric percentage calculation. If the percentage calculation is between the upper and lower thresholds, the detail row for the metric displays light blue. If the percentage calculation is less than or equal to the lower threshold, the detail row for the metric displays red.</p>
<p><strong>NOTE:</strong> The reports used in this calculation are registered on the <em><a href="Data_Quality_Report_Assignment.htm">Data Quality Report Assignment</a></em> page.</p>
<p><strong>NOTE:</strong> This percentage has 7 decimal positions to support a six sigma-level quality definition.</p></td>
</tr>
</tbody>
</table>

## <span id="Wave"></span>Wave Milestones V

[Wave Milestones H](#top)

Field

Description

Delete

Click to delete the milestone.

The milestone is removed from the Migration dashboard.

**NOTE:** The Start Date and End Date milestones cannot be deleted.

Name

Displays the name of the milestone.

Abbreviation

Displays a four-character abbreviation of the milestone name that
displays on the Migration dashboard.

Milestone Date

Displays the date of the milestone used in metrics calculations.

Required

If checked, the milestone cannot be deleted. The Start Date and End Date
milestones, added by default when the user checks the Send Wave And
Milestone Metrics check box on the *[Wave
Identification](Wave_Identification_H.htm)* page, have this check box
checked. The check box cannot be checked for any other milestones.

If unchecked, the milestone can be deleted.

Metric Thresholds

Design Complete Upper Threshold

Displays the percentage to be compared with the Design Complete metric
percentage calculation. If percentage calculation is equal to or greater
than the upper threshold percentage, this milestone is complete and the
detail row for the Design Complete metric displays green on the
dashboard.

**NOTE:** Design Complete indicates how much of the design work has been
completed. This percentage is calculated as the total number of active
fields within active targets where design is complete (the design status
is Design Complete or Finished) divided by the total number of active
fields within active targets, regardless of design status.

Design Complete Lower Threshold

Displays the percentage to be compared with the Design Complete metric
percentage calculation. If the percentage calculation is between the
upper and lower thresholds, the detail row for the metric displays light
blue. If the percentage calculation is less than or equal to the lower
threshold, the detail row for the metric displays red.

Mapping Complete Upper Threshold

Displays the percentage to be compared with the Mapping Complete metric
percentage calculation. If percentage calculation is equal to or greater
than the upper threshold percentage, this milestone is complete and the
detail row for the Mapping Complete metric displays green on the
dashboard.

**NOTE:** Mapping Complete indicates how much of the field mapping and
value mapping work has been completed. This percentage is calculated as
the total number of total mappings opportunities for both value and
field mapping divided by the total number of mappings in Complete
status.

Mapping Complete Lower Threshold

Displays the percentage to be compared with the Mapping Complete metric
percentage calculation. If the percentage calculation is between the
upper and lower thresholds, the detail row for the metric displays light
blue. If the percentage calculation is less than or equal to the lower
threshold, the detail row for the metric displays red.

Rules Complete Upper Threshold

Displays the percentage to be compared with the Rules Complete metric
percentage calculation. If the percentage calculation is equal to or
greater than the upper threshold percentage, this milestone is complete
and the detail row for the Rules Complete metric displays green on the
dashboard.

**NOTE:** Rules Complete indicates how many of the rules have been
completed. This percentage is calculated by the total number of source
and target rules for the active fields with a rule status of complete
divided by the total number of source and target rules (also called rule
opportunities).

Rules Complete Lower Threshold

Displays the percentage to be compared with the Rules Complete metric
percentage calculation. If the percentage calculation is between the
upper and lower thresholds, the detail row for the metric displays light
blue. If the percentage calculation is less than or equal to the lower
threshold, the detail row for the metric displays red.

Quality Upper Threshold

Displays the percentage to be compared with the Quality metric
percentage calculation. If the percentage calculation is equal to or
greater than the upper threshold percentage, this milestone is complete
and the detail row for the Quality metric displays green on the
dashboard.

**NOTE:** Quality indicates the data quality of the wave. This
percentage is calculated using the totals on the error reports
registered to the wave and targets (post load reports) divided by the
total number of records on the opportunity reports registered to the
waves and targets (preload reports).

**NOTE:** The reports used in this calculation are registered on the
*[Data Quality Report Assignment](Data_Quality_Report_Assignment.htm)*
page.

**NOTE:** This percentage has 7 decimal positions to support a six
sigma-level quality definition.

Quality Lower Threshold

Displays the percentage to be compared with the Quality metric
percentage calculation. If the percentage calculation is between the
upper and lower thresholds, the detail row for the metric displays light
blue. If the percentage calculation is less than or equal to the lower
threshold, the detail row for the metric displays red.

**NOTE:** The reports used in this calculation are registered on the
*[Data Quality Report Assignment](Data_Quality_Report_Assignment.htm)*
page.

**NOTE:** This percentage has 7 decimal positions to support a six
sigma-level quality definition.
