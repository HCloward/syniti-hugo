+++
title = 'Wave Process Area Gate Metrics (Field Mapping) H'
solution = 'Migration'
+++

# Wave Process Area Gate Metrics (Field Mapping) H

[Wave Process Area Gate Metrics (Field Mapping)
V](#Wave_Gate_Metrics_Field)

<div class="use">

Use this page to [Set up Wave Gate Metrics for
Map](../Use_Cases/Evaluate_Mapping_with_Wave_Gate_Metrics).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane, or select
    <span style="font-weight: bold;">Console</span> in the Context bar.
2.  Click <span style="font-weight: bold;">Waves</span> in the
    Navigation pane.
3.  Click the <span style="font-weight: bold;">Process Areas</span> icon
    for a Wave.
4.  Click the <span style="font-weight: bold;">Metrics</span> icon for a
    Process Area.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>GATE NAME</p></td>
<td><p>Displays the gate name. A gate is a point in the project where a percentage of field mappings should be completed.</p></td>
</tr>
<tr class="odd">
<td><p>GATE DATE</p></td>
<td><p>Displays the date by which the percentage set in the <strong>GATE PERCENTAGE</strong> field should be finished.</p></td>
</tr>
<tr class="even">
<td><p>GATE PERCENTAGE</p></td>
<td><p>Displays the percent of field mappings in the migration project that should be completed by the <strong>GATE DATE</strong>.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPING PERCENT COMPLETE</p></td>
<td><p>Displays the actual percent complete of the field mappings, as generated by the Snap Shot process in Map. This process is run automatically once daily, but can be run at any time by accessing Map, clicking <strong>Metrics</strong> on the <em><a href="../../Transform/Page_Desc/Process_Area_Launch">Process Area Launch</a></em> page, and then clicking <strong>Process</strong>. </p>
<p><strong>NOTE:</strong> If the current date is later than the <strong>GATE DATE</strong>, the Snap Shot process will not update the percent complete.</p></td>
</tr>
<tr class="even">
<td><p>MAPPING COMPLETED</p></td>
<td><p>Displays the number of field mappings with a <strong>MAPPING STATUS</strong> set to <strong>Complete</strong> and a <strong>RULE STATUS</strong> set to <strong>Complete</strong> on the <em>Field Mappings</em> page in Map.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPING TOTAL</p></td>
<td><p>Displays the total number of field mappings on the <em>Field Mappings</em> page in Map for Targets and Sources.</p></td>
</tr>
<tr class="even">
<td><p>FIELD ACTIVE</p></td>
<td><p>Displays the total number of active fields to be mapped in Map.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD TOTAL</p></td>
<td><p>Displays the number of active and inactive fields in Map.</p></td>
</tr>
<tr class="even">
<td><p>LAST UPDATE DATE</p></td>
<td><p>Displays the last date the Snap Shot process was run in Map.</p></td>
</tr>
</tbody>
</table>

## <span id="Wave_Gate_Metrics_Field"></span>Wave Process Area Gate Metrics (Field Mapping) V

[Wave Process Area Gate Metrics (Field Mapping) H](#top)

<div class="use">

Use this page to [Set up Wave Gate Metrics for
Map](../Use_Cases/Evaluate_Mapping_with_Wave_Gate_Metrics).

</div>

Field

Description

Gate Name

Displays the gate name. A gate is a point in the project where a
percentage of value mappings should be completed.

Description

Displays the gate description.

Gate Settings

Gate Date

Displays the date by which the percentage set in **Gate Percentage**
should be finished.

Gate Percentage

Displays the percent of field mappings in the migration project that
should be completed by the **Gate Date**.

Project Details

Field Active

Displays the number of fields that have the **ACTIVE** check box enabled
on the *Target Fields* page in Map.

Field Total

Displays the total number of fields on the *Target Fields* page in Map.

Mapping Completed

Displays the number of fields that have a **MAPPING STATUS** and a
**RULE STATUS** set to **Complete** on the *Fields Mappings* page in
Map.

Mapping Total

Displays the total number of mappings, regardless of the mapping status.

Percent Completed

Displays the actual percent complete of the field mappings, as generated
by the Snap Shot process in Map. This process is run automatically once
daily, but can be run at any time by accessing Map, clicking **Metrics**
on the *Process Area Launch* page, then clicking **Process**. 

**NOTE:** If the current date is later than the **Gate Date**, the Snap
Shot process will not update the percent complete.

Last Update Date

Displays the last date the Snap Shot process was run in Map.

Source Rule Mappings

Source Rule Completed

Displays the number of Source rules with a **RULE STATUS** of
**Complete** on the *Field Mappings* page in Map.

Source Rule Total

Displays the number of Source rules on the *Field Mappings* page in Map.

Source Rule Field Group Completed

Displays the number of completed Source rule mapping group field
mappings (those fields that belong to the default mapping group ‘\*’).

Source Rule Field Group Total

Displays the total number of Source rule mapping groups on the *Mapping
Groups* page in Map.

Target Rules Mappings

Target Rule Completed

Displays the number of Target rules with a **RULE STATUS** of
**Complete** on the *Field Mappings* page in Map for all Targets in the
context.

Target Rule Total

Displays the number of Target rules on the *Field Mappings* page in Map
for all Targets in the context.

Target Rule Field Group Completed

Displays the number of fields in the Target rule mapping group with a
**RULE STATUS** of **Complete** on the *Field Mappings* page in Map.

Target Rule Field Group Total

Displays the total number of Target rule mapping groups on the *Mapping
Groups* page in Map.
