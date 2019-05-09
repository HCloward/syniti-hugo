# Report Data Viewer H

[Report Data Viewer V](#ReportDataViewer)

<div class="use">

Use this page to [Create a Request in dspCompose™ From the ISA Report
Data Viewer
Page](../Use_Cases/Create_a_Request_in_dspCompose_From_ISA).

</div>

To access this page, select **Information Steward Accelerator \>**
<span style="font-weight: bold;">Report Data Viewer</span> in the
*Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>DATE</p></td>
<td><p>Displays the date and time the rule was processed.</p></td>
</tr>
<tr class="odd">
<td><p>RULE ID</p></td>
<td><p>Displays a name of the rule.</p></td>
</tr>
<tr class="even">
<td><p>RULE BINDING ID</p></td>
<td><p>Displays the name of the table to which the selected rule is bound.</p></td>
</tr>
<tr class="odd">
<td><p>RULE DESCRIPTION</p></td>
<td><p>Displays the rule description added in IS when the rule was created.</p></td>
</tr>
<tr class="even">
<td><p>QUALITY DIMENSION</p></td>
<td><p>Displays the Quality Dimension assigned to the rules in the project. A project can have multiple Quality Dimensions.</p>
<p>Quality Dimensions, such as Conformity and Consistency, . organize rules and provide a score that contributes to the scorecard value.</p>
<p>When a user creates a rule in IS, it is assigned to a Quality Dimension.</p></td>
</tr>
<tr class="odd">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of failed records returned when the rule is run in IS.</p></td>
</tr>
<tr class="even">
<td><p>Query</p></td>
<td><p>Click to view the data that the rule returned (i.e., the data that failed the rule).</p></td>
</tr>
<tr class="odd">
<td><p>Metrics</p></td>
<td><p>Click to open the Metrics Summary page for the selected rule.</p>
<p>Refer to <a href="../Use_Cases/Download_ISA_Metrics_Summary_Information">Download ISA Metrics Summary Information</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Create Compose Request</p></td>
<td><p>Click to create a request for this run of the rule and binding. The failed report data moves to a staging table to use as the basis for a request. In the staging table, dspCompose™ runs rules on the data, then copies it to the Data Entry table. The user assigned to the first Data Entry role receives a notification that work on the request can begin.</p>
<p><strong>NOTE:</strong> The button is disabled if an external request scenario has not been created using the report. In this case, the hover text above the icon reads “No Template Mapped.”</p>
<p><strong>NOTE:</strong> The button is active if an external request scenario has been created using the report but the template is not active. In this case, the hover text above the icon reads “Template Inactive” and an error message displays if the user clicks the Create Compose Request button.</p>
<p><strong>NOTE:</strong> This button does not display if dspCompose™ is not installed and licensed.</p></td>
</tr>
<tr class="odd">
<td><p>dspCompose Request</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="../../dspCompose/Page_Desc/Request_H">Request</a></span> page in dspCompose™ to display the newly created request based on the IS data.</p>
<p><strong>NOTE:</strong> This button does not display if dspCompose™ is not installed and licensed.</p>
<p><strong>NOTE:</strong> This button is active after a user creates a request for this run of the rule and binding by clicking the Create Compose Request button.</p></td>
</tr>
</tbody>
</table>

## <span id="ReportDataViewer"></span>Report Data Viewer ISA V

[Report Data Viewer ISA H](#)

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Date</p></td>
<td><p>Displays the date and time the rule was processed.</p></td>
</tr>
<tr class="odd">
<td><p>Rule ID</p></td>
<td><p>Displays a name of the rule.</p></td>
</tr>
<tr class="even">
<td><p>Rule Binding ID</p></td>
<td><p>Displays the name of the table to which the selected rule is bound.</p></td>
</tr>
<tr class="odd">
<td><p>Rule Description</p></td>
<td><p>Displays the rule description added in IS when the rule was created.</p></td>
</tr>
<tr class="even">
<td><p>Quality Dimension</p></td>
<td><p>Displays the Quality Dimension assigned to the rules in the project. A project can have multiple Quality Dimensions.</p>
<p>Quality Dimensions, such as Conformity and Consistency, organize rules and provide a score that contributes to the scorecard value.</p>
<p>When a user creates a rule in IS, it is assigned to a Quality Dimension.</p></td>
</tr>
<tr class="odd">
<td><p>Record Count</p></td>
<td><p>Displays the number of failed records returned when the rule is run in IS.</p></td>
</tr>
<tr class="even">
<td><p>Query</p></td>
<td><p>Click to view the data that the rule returned (i.e., the data that failed the rule).</p></td>
</tr>
<tr class="odd">
<td><p>Metrics</p></td>
<td><p>Click to open the Metrics Summary page for the selected rule.</p>
<p>Refer to <a href="../Use_Cases/Download_ISA_Metrics_Summary_Information">Download ISA Metrics Summary Information</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Create Compose Request</p></td>
<td><p>Click to create a request for this run of the rule and binding. The failed report data moves to a staging table to use as the basis for a request. In the staging table, dspCompose™ runs rules on the data, then copies it to the Data Entry table. The user assigned to the first Data Entry role receives a notification that work on the request can begin.</p>
<p><strong>NOTE:</strong> The button is disabled if an external request scenario has not been created using the report. In this case, the hover text above the icon reads &quot;No Template Mapped.&quot;?</p>
<p><strong>NOTE:</strong> The button is active if an external request scenario has been created using the report but the template is not active. In this case, the hover text above the icon reads &quot;Template Inactive&quot; and an error message displays if the user clicks the Create Compose Request button.</p>
<p><strong>NOTE:</strong> This button does not display if dspCompose™ is not installed and licensed.</p></td>
</tr>
<tr class="odd">
<td><p>dspCompose Request</p></td>
<td><p>Click to open the <em><a href="../../dspCompose/Page_Desc/Request_H"><em>Request</em></a></em> page in dspCompose™ to display the newly created request based on the IS data.</p>
<p><strong>NOTE:</strong> This button does not display if dspCompose™ is not installed and licensed.</p>
<p><strong>NOTE:</strong> This button is active after a user creates a request for this run of the rule and binding by clicking the Create Compose Request button.</p></td>
</tr>
<tr class="even">
<td><p>IMPLICATION</p></td>
<td><p>Displays information about the implication of failed data for this rule and rule binding, including downstream issues or other rule and rule binding combinations that may be affected.</p></td>
</tr>
<tr class="odd">
<td><p>RECOMMENDATION</p></td>
<td><p>Displays information about how to resolve records that fail for this rule and rule binding.</p></td>
</tr>
</tbody>
</table>
