# Metric Summary H

<span>[Metric Summary V](#Metric_Summary_V)</span>

<div class="use">

Use this page to [Download ISA Metrics Summary
Information](../Use_Cases/Download_ISA_Metrics_Summary_Information).

</div>

To access this page, select **Information Steward Accelerator
\>**Advanced \> Metric Summary in the *Navigation* pane.

<span style="font-weight: bold;">NOTE:</span> The rules that display on
this page depend on how the page is accessed.

  - If this page is accessed when a user drills down through the [Total
    Opportunities vs Failures
    Summary](../Use_Cases/Total_Opportunities_vs._Failures_Summary)
    dashboard or the [Failure Percentage
    Summary](../Use_Cases/Failure_Percentage_Summary) dashboard, the
    rules and all rule bindings for the selected rule display.
  - If the page is accessed from the [Report Data Viewer
    (](Report_Data_Viewer)Report Data Viewer \> Reports \> Metrics
    icon for a report) the data displays for the selected rule and rule
    binding only.
  - If the page is accessed by selecting **Advanced \> Metrics Summary**
    in the <span style="font-style: italic;">Navigation</span> pane all
    rules and rule bindings display.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PROJECT_NAME</p></td>
<td><p>Displays the name of the project added in Information Steward and loaded into ISA.</p></td>
</tr>
<tr class="odd">
<td><p>PROJECT DISTRIBUTION ID</p></td>
<td><p>Displays the name of the Project Distribution to which the selected rule is assigned.</p></td>
</tr>
<tr class="even">
<td><p>RULE_NAME</p></td>
<td><p>Displays the name of the rule created in IS that is run for the Project Distribution.</p></td>
</tr>
<tr class="odd">
<td><p>RULE BINDING ID</p></td>
<td><p>Displays the description of the rule binding. The description can be added on the <span style="font-style: italic;"><a href="Rule_Binding_List">Rule Binding List</a></span> page.</p></td>
</tr>
<tr class="even">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of records that failed the rule.</p></td>
</tr>
<tr class="odd">
<td><p>TOTAL_ROWS</p></td>
<td><p>Displays the total number of records that the rule processed.</p></td>
</tr>
<tr class="even">
<td><p>PERCENTAGE</p></td>
<td><p>Displays, of the total number of records, the percentage of records that failed the rule.</p></td>
</tr>
<tr class="odd">
<td><p>DATE</p></td>
<td><p>Displays the last date the rule ran.</p>
<p><strong>NOTE:</strong> ISA runs a service page every hour to check if IS has processed rules.</p></td>
</tr>
</tbody>
</table>

## <span><span id="Metric_Summary_V"></span>Metric Summary V</span>

<span>[Metric Summary H](Metric_Summary_H)</span>

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Project_Name</p></td>
<td><p>Displays the name of the project added in Information Steward and loaded into ISA.</p></td>
</tr>
<tr class="odd">
<td><p>Project Distribution ID</p></td>
<td><p>Displays the name of the Project Distribution to which the selected user is assigned.</p></td>
</tr>
<tr class="even">
<td><p>Rule_Name</p></td>
<td><p>Displays the name of the rule created in IS that is run for the Project Distribution.</p></td>
</tr>
<tr class="odd">
<td><p>Record Count</p></td>
<td><p>Displays the number of records that failed the rule.</p></td>
</tr>
<tr class="even">
<td><p>Total_Rows</p></td>
<td><p>Displays the total number of records that the rule processed.</p></td>
</tr>
<tr class="odd">
<td><p>Run ID</p></td>
<td><p>Displays a unique number to identify when the rule was processed.</p></td>
</tr>
<tr class="even">
<td><p>Rule ID</p></td>
<td><p>Displays a unique number for the rule.</p></td>
</tr>
<tr class="odd">
<td><p>Binding ID</p></td>
<td><p>Displays a unique number for the rule.</p></td>
</tr>
<tr class="even">
<td><p>Date</p></td>
<td><p>Displays the last date the rule ran.</p>
<p><strong>NOTE:</strong> ISA runs a service page every hour to check if IS has processed rules.</p></td>
</tr>
<tr class="odd">
<td><p>Dimension_Name</p></td>
<td><p>Displays the Quality Dimension assigned to the rules in the project. A project can have multiple Quality Dimensions.</p>
<p>Quality Dimensions, such as Conformity and Consistency, . organize rules and provide a score that contributes to the scorecard value.</p>
<p>When a user creates a rule in IS, it is assigned to a Quality Dimension.</p></td>
</tr>
<tr class="even">
<td><p>FD_Table_Alias_Name</p></td>
<td><p>Displays the Failed Data Table name stored in the IsFailedData database.</p>
<p>Two tables with this name are created each time the rule is run. One table name has _FD appended; the other has _FR (e.g., MARA_P127T164_FD and MARA_P127T164_FR).</p>
<p>The table ending with FD stores all the data from the IS Rule.</p>
<p>The table ending with FR stores all the records failing a Rule binding with a ROW Key stored in the table ending with FD.</p></td>
</tr>
</tbody>
</table>
