+++
title = 'Target Exports H'
solution = 'Migration'
+++

# Target Exports H

[Target Exports V All Tabs](#Target_Exports_V_All_Tabs)

<div class="use">

Use this page to [Add Target
Exports](../Use_Cases/Add_Target_Exports.htm).

</div>

To access this page:

1.  [Access Transform](../Config/Access_Transform.htm).
2.  Click the **Targets** icon on the *[Process Area
    Launch](Process_Area_Launch.htm)* page.
3.  Click the **Exports** icon for a Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Execute</p></td>
<td><p>Click to export the package immediately in the foreground.</p>
<p><strong>NOTE</strong>: This icon is dimmed when the export type is Integrate</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset the processing status if a process fails for the selected target export.</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the target export is processed.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays the <span id="Status" class="popUpLink">status</span> of the target export.</p></td>
</tr>
<tr class="even">
<td><p>EXPORT TYPE</p></td>
<td><p>Displays how data is exported from Transform. Options include Database, Integrate, Local File and Protected Package.</p>
<p><strong>NOTE:</strong> If a user saves a target export with an export type of Local File, an Assemble tab-delimited package is created and registered to the export.</p>
<p><strong>NOTE:</strong> If the export type is Integrate, refer to <a href="../Use_Cases/Use_an_Integrate_Process_as_an_Export_Type.htm">Use an Integrate Process as an Export Type</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET EXPORT</p></td>
<td><p>Displays the name of the set of rules to move the target data to a location so that it can be staged for export to an ERP system using a loading tool.</p>
<p><span style="font-weight: bold;">NOTE:</span> If a user saves a target export with an export type of Local File, an Assemble tab-delimited package is created and registered to the export.</p></td>
</tr>
<tr class="even">
<td><p>LOAD TYPE</p></td>
<td><p>Displays the method or tool Transform uses for the target export. This field is for documentation purposes only.</p>
<p>A list of Load Types displays in Transform on the <em><a href="Load_Type_Setup.htm">Load Types (Setup)</a></em> page.</p></td>
</tr>
<tr class="odd">
<td><p>ACTION ON</p></td>
<td><p>Displays the date Transform processed the selected target export.</p></td>
</tr>
<tr class="even">
<td><p>RECORD COUNT</p></td>
<td><p>Displays the number of records to be exported.</p></td>
</tr>
<tr class="odd">
<td><p>DURATION</p></td>
<td><p>Displays the amount of time Transform took to process the selected target export. If the field is empty, the target export has not been processed.</p>
<p><strong>NOTE:</strong> If a process takes less than 0.5 seconds to run, the duration in the DURATION field is 0.</p></td>
</tr>
<tr class="even">
<td><p>View Export</p></td>
<td><p>Click to view the export data.</p></td>
</tr>
<tr class="odd">
<td><p>Queue</p></td>
<td><p>Click to open the <em><a href="../../../Data_Quality/dspMonitor/Page_Desc/Monitor_H.htm">Monitor</a></em> page to monitor the background job processes for the selected target export. If an export has no data to process, this icon is disabled.</p></td>
</tr>
</tbody>
</table>

## <span id="Target_Exports_V_All_Tabs"></span>Target Exports V All Tabs

[Target Exports H](Target_Exports_H.htm)

<div class="use">

Use this page to [Add Target
Exports](../Use_Cases/Add_Target_Exports.htm).

</div>

This page has the following tabs:

  - [General tab](#General_Tab7)
  - [Process Information tab](#Process_Information_Tab6)

### <span id="General_Tab7"></span>General tab

Field

Description

Target

Displays the name of the target table.

Target Export

Displays the name of the set of rules to move the target data to a
location so that it can be staged for export to an ERP system using a
loading tool. This is a manually created view in SQL.

<span style="font-weight: bold;">NOTE:</span> If a user saves a target
export with an export type of Local File, an Assemble tab-delimited
package is created and registered to the export.

Export Type

Displays how data is exported from Transform. Options include Database,
Integrate, Local File and Protected Package.

**NOTE:** If a user saves a target export with an export type of Local
File, an Assemble tab-delimited package is created and registered to the
export.

**NOTE:** If the export type is Integrate, refer to [Use an Integrate
Process as an Export
Type](../Use_Cases/Use_an_Integrate_Process_as_an_Export_Type.htm) for
more information.

Export Name

Displays the name of the protected package.

If the Export Type is Integrate, an Integrate process name displays.
Refer to [Use an Integrate Process as an Export
Type](../Use_Cases/Use_an_Integrate_Process_as_an_Export_Type.htm)for
more information.

Export Instance

Displays the name of the database used in a target export for a Database
export type.

Status Information

Priority

Displays the target export priority, which is the order the target
export is processed.

Status

Displays the <span id="Status" class="popUpLink">status</span> of the
target export.

Load Information

Load Type

Displays the method or tool Transform uses for the target export. This
field is for documentation purposes only.

A list of Load Types displays in Transform on the *[Load Types
(Setup)](Load_Type_Setup.htm)* page.

Load Program

Displays the program used to load data. This is a free-form text field
and is not validated.

Load Person

Displays the name of the person responsible for the load.

Load Requirements

Displays notes about the load. This is a free-form text field and is not
validated.

Documentation

Comment

Displays user-entered comments about the target export.

Recon Type

Displays an option to indicate if a target export adds records, deletes
records or is informational. If a data audit is conducted to determine
if all data records were loaded (as they were expected to be loaded),
the Recon Type justifies why records were not loaded. Use the options
Adds records (+) or Deletes records (-), include or exclude,
respectively, on certain exports (delta loads, multi-step loads, etc.)
from the Target Reconciliation Report.

### <span id="Process_Information_Tab6"></span>Process Information tab

Field

Description

Action On

Displays the date Transform processed the selected target export.

Record Count

Displays the number of records affected by the target export’s
execution.

Duration

Displays the amount of time Transform took to process the selected
target export. If the field is empty, the target export has not been
processed.

**NOTE:** If a process takes less than 0.5 seconds to run, the duration
in the DURATION field is 0.

Reset

Click to reset the processing status if a process fails for the selected
target export.

Process

Click to process the target export in the background. View the status of
background processing on the *[Monitor](Monitor_Transform_H.htm)* page. 

**NOTE:**  If the Export Type is Integrate, this icon is disabled.

Advanced

Export Order By

Displays the order that the target is exported.
