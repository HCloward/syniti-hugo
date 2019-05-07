+++
title = 'Target Sources H'
solution = 'Migration'
+++

# Target Sources H

[Target Sources V All Tabs](#Target_Sources_V_All_Tabs)

<div class="use">

Use this page to [Manage Target
Sources](../Use_Cases/Manage_Target_Sources.htm).

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. Refer to [Use Bulk
Execution](../../../Platform/Bulk_Exec/Use_Bulk_Execution.htm) for more
information.

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Click the **Targets** icon on the *[Process Area
    Launch](Process_Area_Launch.htm)* page.
3.  Click the **Sources** icon for a Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Process</p></td>
<td><p>Click to run the entire source in the background by importing all data from all sources and running all source rules and source reports. View the status of background processing on the <em>Monitor</em> page.</p>
<p><strong>NOTE:</strong> If the selected source is inactive, the Process icon is disabled.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset the processing status if a process fails for any of the Target Source’s Target Source reports or Target Source rules.</p></td>
</tr>
<tr class="even">
<td><p>Debug</p></td>
<td><p>Click to open the <em><a href="Debug_Breakpoints_Target_Sources.htm">Debug – Breakpoints (Target Sources)</a></em> page to add breakpoints to steps in the process for the selected Target Source for Target Source rules and Target Source reports. Use breakpoints to debug issues with failed processing.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the source is processed.</p></td>
</tr>
<tr class="even">
<td><p>STATUS</p></td>
<td><p>Displays the <span id="Status" class="popUpLink">status</span>.</p>
<p>If Source Active On Build is enabled on the <span style="font-style: italic;"><a href="../../Console/Page_Desc/Parameters.htm">Parameters</a></span> page in Console, target sources are auto-generated with a default status of active in Transform. If feature is disabled, target sources are auto-generated with a default status of inactive in Transform.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE ID</p></td>
<td><p>Displays the user friendly source name for the source data source assigned to the target in Console.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE DATABASE OBJECT</p></td>
<td><p>Displays the name of the object that stores the source data. Default value is SrcTable.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE CONNECTION TYPE</p></td>
<td><p>Displays the connection type for the source import associated with a CranPort, SSIS, or Data Services package. These imports can be from comma-separated text files, Excel files, Access databases, SQL Server databases or ODBC databases, such as DB2 and Oracle.</p></td>
</tr>
<tr class="even">
<td><p>ACTION ON</p></td>
<td><p>Displays the last date the reports or rules in the source were processed.</p></td>
</tr>
<tr class="odd">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the total number of records on source reports.</p></td>
</tr>
<tr class="even">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time in seconds that it took for all reports and rules in the source to process.</p>
<p><strong>NOTE:</strong> The duration for sources, targets, and objects is calculated as the sum of the durations of the various tasks that run within said sources, targets, and objects.</p></td>
</tr>
<tr class="odd">
<td><p>PUBLISH</p></td>
<td><p>If checked, the reports in the source are visible to the Business Users assigned to it.</p>
<p><strong>NOTE:</strong> If Publish is not checked, the user will only see the Publish, Implication and Recommendation fields. If Publish is checked, the user will see the Publish, Business User Priority, Sensitive, Implication, Recommendation and Business User Assignment fields.</p></td>
</tr>
<tr class="even">
<td><p>Rules</p></td>
<td><p>Click to open the <em><a href="Target_Source_Rules_H.htm">Target Source Rules</a></em> page to add, edit and delete rules for the selected source.</p>
<p><strong>NOTE:</strong> If the source’s status is inactive or if the Source Database Object is –SrcTable—this icon is disabled</p></td>
</tr>
<tr class="odd">
<td><p>Reports</p></td>
<td><p>Click to open the <em><a href="Target_Source_Reports_H.htm">Target Source Reports</a></em> page to add, edit and delete reports for the selected source.</p>
<p><strong>NOTE:</strong> If the source’s status is inactive or if the Source Database Object is –SrcTable—this icon is disabled</p></td>
</tr>
<tr class="even">
<td><p>View Source</p></td>
<td><p>Click to open the <em><a href="#">Target Sources</a></em> page to view the source data.</p></td>
</tr>
<tr class="odd">
<td><p>Queue</p></td>
<td><p>Click to open the <em><a href="Monitor_Transform_H.htm">Monitor</a></em> page to monitor the background job processes for the selected source. If a source has no data to process, this icon is disabled.</p></td>
</tr>
</tbody>
</table>

## <span id="Target_Sources_V_All_Tabs"></span>Target Sources V All Tabs

[Target Sources H](Target_Sources_H.htm)

<div class="use">

Use this page to [Manage Target
Sources](../Use_Cases/Manage_Target_Sources.htm).

</div>

This page has the following tabs:

  - [General tab](#General_Tab1)
  - [Process Information tab](#Process_Information_Tab1)

## <span id="General_Tab1"></span>General tab

Field

Description

Reset

Click to reset the processing status if a process fails for any of the
Target Source’s Target Source reports or Target Source rules.

Process

Click to run the entire source in the background by importing all data
from all sources and running all source rules and source reports in that
order. View the status of background processing on the
*[Monitor](../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm)*
page.

**NOTE:** If the selected source is inactive, the Process icon is
disabled.

Debug

Click to open the *[Debug – Breakpoints (Target
Sources)](Debug_Breakpoints_Target_Sources.htm)* page to add breakpoints
to steps in the process for the selected Target Source, including Target
Source rules and Target Source reports. Use breakpoints to debug issues
with failed processing.

Source Information

Source ID

Displays the source name.

Source Database Object

Displays the name of the object that stores the source data.

Source Connection Type

Displays the connection type for the source import associated with a
CranPort, SSIS or Data Services package. These imports can be from
comma-separated text files, Excel Files, Access databases, SQL Server
databases or ODBC databases, such as DB2 and Oracle.

Package Name

Displays the CranPort, SSIS or Data Services import package name. This
field does not display if the CONNECTION TYPE set on the *Target Source*
page’s *Horizontal* View is None.

The naming convention for packages is \#Database\#%\#Source\#%, for
example dswBRAZIL.stKNA1\_QALegacyData\_Customer.imp for an import or
dswBRAZIL.stKNA1\_QALegacyData\_Customer.exp for an export.

Truncate Before Import

If checked, a source table is truncated before an import package is run
against it. This field does not display if the CONNECTION TYPE set on
the *Target Source* page’s *Horizontal* View is None.

Status Information

Priority

Displays the order the source is processed.

Status

Displays the <span id="Status" class="popUpLink">status</span>. Only
active sources are run.

If Source Active On Build is enabled on the
<span style="font-style: italic;">[Parameters](../../Console/Page_Desc/Parameters.htm)</span>
page in Console, target sources are auto-generated with a default status
of active in Transform. If disabled target sources are auto-generated
with a default status of inactive in Transform.

Contact Information

Primary Developer

Displays the name of the primary developer responsible for the target.
This field is for documentation purposes only.

Secondary Developer

Displays the name of the secondary developer responsible for the target.
This field is for documentation purposes only.

Documentation

Generated Documentation

Click to open the *[Target Documentation](Target_Documentation.htm)*
page to generate and download audit documentation, reconciliation
reports, and technical documentation.

## <span id="Process_Information_Tab1"></span>Process Information tab

Field

Description

Action On

Displays the date Transform processed the selected Target Source.

Record Count

Displays the number of records in the selected source.

Duration

Displays the amount of time Transform took to process the selected
Target Source. If the field is empty, the Target Source has not been
processed.

**NOTE:** The duration for sources, targets, and objects is calculated
as the sum of the durations of the various tasks that run within said
sources, targets, and objects.

Queue

Click to open the *[Monitor](Monitor_Transform_H.htm)* page to monitor
the background job processes for the selected source. If a source has no
data to process, this icon is disabled.

Import Table

Create Import Table

If checked, Transform automatically generates the import table when
importing data from the source. Transform provides the ability to import
data from an Excel file, a text file, or another source table in another
database on the same server into a source table.

View Import Table

Click to view the import table.

**NOTE:** This icon is disabled if the user has checked the Create
Import Table check box but has not processed the Target Source after
doing so. The View Import Table icon will be disabled until the user
clicks the Process icon for the Target Source.

Actions

Import Only

Click to only import the selected source and not process source rules or
reports.

Source Rules Only

Click to only process rules only for the selected source.

Source Reports Only

Click to only process reports for the selected source.
