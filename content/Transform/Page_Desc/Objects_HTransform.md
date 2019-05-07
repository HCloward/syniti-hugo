+++
title = 'Objects H'
solution = 'Migration'
+++

# Objects H

[Objects V](#Objects_V)

<div class="use">

Use this page to [Work with
Objects](../Use_Cases/Work_with_Objects.htm).

</div>

To access this page in Transform, select the **Objects** icon on
the *[Process Area Launch](Process_Area_Launch.htm)* page.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Process</p></td>
<td><p>Click to run the entire target in the background by importing all data from all sources and running all source rules and source reports, target rules, target reports and target exports (in that order). View the status of background processing on the <em><a href="../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm">Monitor</a></em> page. If a user clicks the Process icon, the action affects all of the object’s associated targets, target sources, and their associated rules and reports, along with target exports.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset the processing status if a process fails for any of the object’s targets, target reports, target rules, or target exports. If a user clicks the Reset icon, the action affects all of the object’s associated targets, target sources, and their associated rules and reports, along with target exports.</p></td>
</tr>
<tr class="even">
<td><p>Publish Object</p></td>
<td><p>Click to publish the selected object, which allows the object to be used in reports on a Business User’s All Business Reports and Actionable Reports. Refer to <a href="../Use_Cases/Publish_Reports_to_Report_Delivery_Pages.htm">Report Publishing</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Unpublish Object</p></td>
<td><p>Click to remove the object from reports on the Business User’s All Business Reports and Actionable Reports.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the object is processed. Priority is set in Console (Elements &gt; Object) but can be updated in Transform on the Targets page (Process Area Launch &gt; Targets).</p></td>
</tr>
<tr class="odd">
<td><p>OBJECT</p></td>
<td><p>Displays the name of the object as created in Console.</p></td>
</tr>
<tr class="even">
<td><p>DATA SOURCE ID</p></td>
<td><p>Displays the data source assigned to the object. This value is set in Console and is the Transform database where all target tables and all source tables will be registered for the object.</p></td>
</tr>
<tr class="odd">
<td><p>ACTION ON</p></td>
<td><p>Displays the date when a rule, report or export in the object was last processed.</p></td>
</tr>
<tr class="even">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time Transform took to process the rule, report or exports in the object. If the field is empty the object has not been processed.</p>
<p>The duration for sources, targets, and objects is calculated as the sum of the durations of the various tasks that run within said sources, targets, and objects.</p></td>
</tr>
<tr class="odd">
<td><p>PUBLISH</p></td>
<td><p>If checked, reports in the object are visible to the Business Users assigned to the reports.</p></td>
</tr>
<tr class="even">
<td><p>Targets</p></td>
<td><p>Click to open the <em><a href="Targets_H.htm">Targets</a></em> page to edit the priority of an object, add sources, rules, and reports, and export the target data.</p></td>
</tr>
<tr class="odd">
<td><p>Queue</p></td>
<td><p>Click to open the <em><a href="Monitor_Transform_H.htm">Monitor</a></em> page to monitor background processes running for the object’s targets and target sources, along with all rules, reports and target exports. If an object has no data to process, this button is disabled.</p></td>
</tr>
<tr class="even">
<td><p>Report Readiness Notification</p></td>
<td><p>Click to open the <em><a href="Report_Readiness_Notification.htm">Report Readiness Notification</a></em> page to add and remove users from notifications and to send notifications. Report Readiness Notifications are sent to Business users who access Report Delivery pages when there are errors on their assigned reports.</p></td>
</tr>
<tr class="odd">
<td><p>Rule Report Summary</p></td>
<td><p>Click to open the Rule Report Summary dashboard at the object level to view the number of active rules and reports for all targets and sources in the object.</p></td>
</tr>
<tr class="even">
<td><p>Report Process Count</p></td>
<td><p>Click to open the Report Process Count dashboard at the object level to view the count of processes for all reports in the object.</p></td>
</tr>
<tr class="odd">
<td><p>Change Summary</p></td>
<td><p>Click to open the Change Summary dashboard at the object level to view counts for updates to procedures, tables, and views for all targets in the object.</p></td>
</tr>
</tbody>
</table>

## <span id="Objects_V"></span>Objects  V

[Objects H](Objects_HTransform.htm)

<div class="use">

Use this page to [Work with
Objects](../Use_Cases/Work_with_Objects.htm).

</div>

Field

Description

Reset

Click to reset the processing status if a process fails for any of the
object’s targets, target reports, target rules, and target exports.

Process

Click to run the entire target in the background by importing all data
from all sources and running all source rules and source reports, target
rules, target reports and target exports (in that order). View the
status of background processing on the *Monitor* page. If a user clicks
the Process icon, the action affects all of the object’s associated
targets, target sources, and their associated rules and reports, along
with target exports.

Settings

Priority

Displays the sort order for the object.

Object

Displays the name of object as created in Console.

Data Source ID

Displays the data source assigned to the object. This value is set in
Console and is the Transform database where all target tables and all
source tables will be registered for the object.

ERP Database

Displays the ERP system database that stores the object. This is a
free-form text field to store data and is not validated.

ERP Instance

Displays the ERP system instance that stores the object. This is a
free-form text field to store data and is not validated.

ERP Client

Displays the ERP system client name that stores the object. This is a
free-form text field to store data and is not validated.

Documentation

Generated Documentation

Click to open the *[Object Documentation](Object_Documentation.htm)*
page to generate and download audit documentation.

Process Information

Action Date

Displays an auto-generated date when the object is processed.

Object Duration

Displays the amount of time Transform took to process the selected
object. If the field is empty, the object has not been processed.

**NOTE:** The duration for sources, targets, and objects is calculated
as the sum of the durations of the various tasks that run within said
sources, targets, and objects.

Queue

Click to open the *[Monitor](Monitor_Transform_H.htm)* page to monitor
the background job processes for the selected object. If an object has
no data to process, this icon is disabled.
