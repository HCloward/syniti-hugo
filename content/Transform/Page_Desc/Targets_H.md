# Targets H

[Targets V All Tabs](#Targets_V_All_Tabs)

<div class="use">

Use this page to:

  - [Manage Targets](../Use_Cases/Manage_Targets.htm)
  - [Edit the Priority  and Publish
    Setting](../Use_Cases/Edit_the_Priority_and_Publish_Setting.htm)
  - [Grant a User Access to Sensitive Data on Report Delivery
    Pages](../Use_Cases/Grant_Users_Access_to_Reports_and_Sensitive_Data.htm#Grant_a_User_Access_to_Sensitive_Data_on_Report_Delivery_Pages)

</div>

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Click the **Targets** icon on the *[Process Area
    Launch](Process_Area_Launch.htm)* page.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Process</p></td>
<td><p>Click to run the entire target in the background by importing all data from all sources and running all active source rules and source reports, target rules, target reports and target exports (in that order). View the status of background processing on the <em><a href="../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm">Monitor</a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset the processing status if a process fails for any of the target’s target reports, target rules, and target exports.</p></td>
</tr>
<tr class="even">
<td><p>Debug</p></td>
<td><p>Click to open the <a href="Debug_Breakpoints.htm"><em>Debug – Breakpoints</em></a> page to add breakpoints to steps in the process for the selected target, including target rules and target reports. Use breakpoints to debug issues with failed processing.</p></td>
</tr>
<tr class="odd">
<td><p>OBJECT</p></td>
<td><p>Displays the name of the object as created in Console.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the target is processed. If the target did not have a priority when it was created in Map, Map copies the priority value entered in Console for the target on the <em><a href="#">Targets</a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays the <span id="Status" class="popUpLink">status</span> of the target in the data conversion project. Only active targets are processed.</p></td>
</tr>
<tr class="even">
<td><p>TARGET</p></td>
<td><p>Displays the name of the target table.</p></td>
</tr>
<tr class="odd">
<td><p>ACTION ON</p></td>
<td><p>Displays the last date that a rule, report or export was processed for the target.</p></td>
</tr>
<tr class="even">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time in seconds that all reports, rules and exports took to process.</p>
<p><strong>NOTE:</strong> The duration for sources, targets and objects is calculated as the difference of the start and end times for the job in the Transform JobQueue.</p></td>
</tr>
<tr class="odd">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the total record count on all source reports.</p></td>
</tr>
<tr class="even">
<td><p>PUBLISH</p></td>
<td><p>If checked, Transform uses the report level publish setting for each report registered to the target to determine whether to publish the report to the report delivery pages.</p>
<p>If unchecked, the Report Cache  will not be created for publishing to the report delivery pages.</p></td>
</tr>
<tr class="odd">
<td><p>Sources</p></td>
<td><p>Click to open the <em><a href="Target_Sources_H.htm">Targets Sources</a></em> page to add, edit and delete sources for the target.</p></td>
</tr>
<tr class="even">
<td><p>Rules</p></td>
<td><p>Click to open the <em><a href="Target_Rules_H.htm">Target Rules</a></em> page to add, edit and delete target rules, including setting the rule type and the view that the rule is based on.</p></td>
</tr>
<tr class="odd">
<td><p>Reports</p></td>
<td><p>Click to open the <a href="Target_Reports_H.htm"><em>Target Reports</em></a> page to add, edit and delete target reports.</p></td>
</tr>
<tr class="even">
<td><p>TR</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Target_Remediation_Overview.htm">Target Remediation Overview</a></span> page to view details about remediation rules applied to an error report for any reports associated with the selected target. If the icon is active, the count displays the total number of fixed remediation and remediation rules applied to reports. If the icon is disabled, no remediation rules have been applied to any reports associated with the selected target.</p></td>
</tr>
<tr class="odd">
<td><p>Data Services Rules</p></td>
<td><p>Click to open the <em><a href="Target_Data_Services_Rules_H.htm">Target Data Services Rules</a></em> page where target data services rules can be registered and run.</p>
<p><strong>NOTE:</strong> This icon displays if a Data Services repository has been set at the object level. Refer to <a href="../../Console/Config/Configure_Data_Services_Functionality.htm">Configure Data Services Functionality</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Data Services Reports</p></td>
<td><p>Click to open the <em><a href="Target_Data_Services_Reports_H.htm">Target Data Services Reports</a></em> page where target data services reports can be registered and run.</p>
<p><strong>NOTE:</strong> This icon displays if a Data Services repository has been set at the object level. Refer to <a href="../../Console/Config/Configure_Data_Services_Functionality.htm">Configure Data Services Functionality</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Data Services Remediation</p></td>
<td><p>Click to open the <em><a href="Target_DS_Remediation_H.htm">Target Data Services Remediation</a></em> page. This page displays target data services remediation rules that have been run.</p>
<p><strong>NOTE:</strong> This icon displays if a Data Services repository has been set at the object level. Refer to <a href="../../Console/Config/Configure_Data_Services_Functionality.htm">Configure Data Services Functionality</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Exports</p></td>
<td><p>Click to open the <a href="Target_Exports_H.htm"><em>Target Exports</em></a> page to export the target to a database, local file, or protected package.</p></td>
</tr>
<tr class="odd">
<td><p>View Target</p></td>
<td><p>Click to open the <em>Targets</em> page, which displays all the details for the selected target.</p></td>
</tr>
<tr class="even">
<td><p>Queue</p></td>
<td><p>Click to open the <em><a href="Monitor_Transform_H.htm">Monitor</a></em> page to monitor the background job processes for the selected target.</p></td>
</tr>
<tr class="odd">
<td><p>Rule Report Summary</p></td>
<td><p>Click to open the Rule Report Summary dashboard at the target level to view the number of active rules and reports for the target.</p></td>
</tr>
<tr class="even">
<td><p>Report Process Count</p></td>
<td><p>Click to open the Report Process Count dashboard at the target level to view the count of processes for all reports in the target.</p></td>
</tr>
</tbody>
</table>

## <span id="Targets_V_All_Tabs"></span>Targets V All Tabs

[Targets H](Targets_H.htm)

<div class="use">

Use this page to [Manage Targets](../Use_Cases/Manage_Targets.htm).

</div>

This page has the following tabs:

  - [General tab](#General_Tab)
  - [Process Information tab](#Process_Information_Tab)

## <span id="General_Tab"></span>General tab

Field

Description

Reset

Click to reset the processing status if a process fails for any of the
target’s target reports, target rules, and target exports.

Process

Click to run the entire target in the background by importing all data
from all sources and running all source rules and source reports, target
rules, target reports and target exports in that order. View the status
of background processing on the *Monitor* page.

Debug

Click to open the [*Debug – Breakpoints*](Debug_Breakpoints.htm) page to
add breakpoints to steps in the process for the selected target for
target rules and target reports. Use breakpoints to debug issues with
failed processing.

Object

Displays the object name.

Target Type

Displays a category for the target, such as Historical Data or
Transaction Data.

Status Information

Priority

Displays the order the target is processed. If the target did not have a
priority when it was created in Map, Map copies the priority value
entered in Console for the target on the *Targets* page into this field.

Status

Displays the <span id="Status" class="popUpLink">status</span>. Only
active targets are processed.

Metrics

Click to open the *Target Metrics* page to view the metric, weight and
percent complete for the selected target.

Contact Information

Primary Developer

Displays the name of the primary developer responsible for the target.
This field is for documentation purposes only.

Secondary Developer

Displays the name of the secondary developer responsible for the target.
This field is for documentation purposes only.

Documentation

Complexity

Displays the complexity for building the target used to evaluate work
assignments. Options include Average, Simple or Complex.

Generated Documentation

Click to open the *[Target Documentation](Target_Documentation.htm)*
page to generate and download audit documentation, reconciliation
reports, and technical documentation.

## <span id="Process_Information_Tab"></span>Process Information tab

Field

Description

Record Count

Displays the number of records in the target table.

Action On

Displays the date Transform processed the selected target.

View Target

Click to opens the *Targets* page to view all target data.

Queue

Click to open the *[Monitor](Monitor_Transform_H.htm)* page to monitor
the background job processes for the selected target. If a target has no
data to process, this icon is disabled.

Data Services Components

**NOTE:** The fields in this section display if a Data Services
repository has been set at the object level. Refer to [Configure Data
Services
Functionality](../../Console/Config/Configure_Data_Services_Functionality.htm)
for more information.

Data Services Rules

Click to open the *[Target Data Services
Rules](Target_Data_Services_Rules_H.htm)* page where target data
services rules can be registered and run.

Data Services Reports

Click to open the *[Target Data Services
Reports](Target_Data_Services_Reports_H.htm)* page where target data
services reports can be registered and run.

Data Services Remediations

Click to open the *[Target Data Services
Remediation](Target_DS_Remediation_H.htm)* page. This page displays
target data services remediation rules that have been run.

Actions

Sources Only

Click to process all sources for the selected target. This procedure is
terminated after sources are processed. Target rules, target reports and
target exports are exempt from this procedure.

Rules Only

Click to process all target rules for the selected target.

Reports Only

Click to process all target reports for the selected target.

Data Services Rules Only

Click to process all target data services rules for the selected target.

**NOTE:** This field displays if a Data Services repository has been set
at the object level. Refer to [Configure Data Services
Functionality](../../Console/Config/Configure_Data_Services_Functionality.htm)
for more information.

Data Services Rules Only

Click to process all target data services reports for the selected
target.

**NOTE:** This field displays if a Data Services repository has been set
at the object level.

Exports Only

Click to process all target exports for the selected target.

Refresh Error Aggregate Cache Schema

Click to drop all the records from the current cache table for the
*[Target All Errors Report](Target_All_Errors_Report.htm)* and build a
new, updated version of the cache table based on an updated target
schema.

This action syncs the cache table for the Target All Errors Report with
a target’s updated schema that has been changed during development.

**NOTE:** If the Target All Errors Report displays results when a user
clicks this icon, the records are cleared from the report..
