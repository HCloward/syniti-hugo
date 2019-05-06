# Target Dashboard Stats H

[Target Dashboard Stats V](#Target_Dashboard_Stats_V)

<div class="use">

Use this page to [View Metrics](../Use_Cases/View_Metrics_Map.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Map</span> in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Metrics</span> icon on
    the *[Process Area Launch](Process_Area_Launch_map.htm)* page
4.  Click the <span style="font-weight: bold;">Metrics</span> icon on
    the <span style="font-style: italic;">[Metrics and Reports
    Landing](Metrics_and_Reports_Landing.htm)</span> page.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Daily</p></td>
<td><p>Click to open the <em><a href="Target_Metrics_Daily_H.htm">Target Metrics Daily</a></em> page to view a daily snap shot summary of field mappings for the selected Target. These values will not change once the snap shot has been taken.</p>
<p>Refer to <a href="../Use_Cases/Capture_Statistics_for_Wave_Gate_Metrics.htm">Capture Statistics for Wave Gate Metrics</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Weekly</p></td>
<td><p>Click to open the <em><a href="Targets_Metrics_Weekly_H.htm">Target Metrics Weekly</a></em> page to view a weekly snap shot summary of the field mappings for the selected Target taken at the end of the week.  These values will not change once the snap shot has been taken.</p>
<p>Refer to <a href="../Use_Cases/Capture_Statistics_for_Wave_Gate_Metrics.htm">Capture Statistics for Wave Gate Metrics</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Monthly</p></td>
<td><p>Click to open the<a href="Targets_Metrics_Monthly_H.htm"><em>Target Metrics Monthly</em></a> page to view a monthly snap shot summary of the field mappings for the selected Target taken on the 1<sup>st</sup> of each month.  These values will not change once the snap shot has been taken.</p>
<p>Refer to <a href="../Use_Cases/Capture_Statistics_for_Wave_Gate_Metrics.htm">Run the Snap Shot Process to Capture Statistics for Wave Gate Metrics</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the object name defined in Console.Click the link to open the</p></td>
</tr>
<tr class="even">
<td><p>TARGET</p></td>
<td><p>Displays the Target name defined in Target Design. Click the link to open the <span style="font-style: italic;"><a href="Targets_H_Map.htm">Targets</a></span> page to view details about the Target.</p></td>
</tr>
<tr class="odd">
<td><p>PERCENTAGE SOURCE NON FIELD GROUP</p></td>
<td><p>Displays the percent complete of Non Field Group field mappings (as in, field mappings that belong to the default mapping group (*)).</p>
<p><strong>NOTE:</strong> It is a requirement that all fields be mapped in a Source even if the field mapping has an action of Not Used. Field Groups are assigned in Target Design, and allow users to apply filters for mapping based on certain values in a field.</p></td>
</tr>
<tr class="even">
<td><p>PERCENTAGE SOURCE FIELD GROUP</p></td>
<td><p>Displays the percent complete of Field Group field mappings (as in, field mappings that do not belong to the default Field group (*)).</p>
<p>Field Groups and their associated Metric Groups are optional mappings to create data-driven filter updates.</p></td>
</tr>
<tr class="odd">
<td><p>PERCENTAGE TARGET RULE NON FIELD GROUP</p></td>
<td><p>Displays the percent complete of Target Rule Non Field Group field mappings (as in, field mappings that display {Target Rules} in TARGET SOURCE DETAILS on the <em><a href="Field_Mappings_H.htm">Field Mappings</a></em> page, and that belong to the default Field group (*)).</p>
<p><strong>NOTE:</strong> A field mapping of {Target Rules} is not required for any fields but may be necessary. The value uses those mappings of {Target Rules} where ACTION is not blank.</p></td>
</tr>
<tr class="even">
<td><p>PERCENTAGE TARGET RULE FIELD GROUP</p></td>
<td><p>Displays the percent complete of Target Rule Field Group field mappings (as in, field mappings that display {Target Rules} in TARGET SOURCE DETAILS on the <em>Field Mappings</em> page, and that do not belong to the default Field group (*)).</p>
<p><strong>NOTE</strong>: A field mapping of {Target Rules} is not required for any fields but may be necessary. The value uses those mappings of {Target Rules} where ACTION is not blank.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE FIELDS</p></td>
<td><p>Displays the number of active fields for the selected Target.</p></td>
</tr>
<tr class="even">
<td><p>ALL FIELDS</p></td>
<td><p>Displays the total field count in the Target ERP table.</p></td>
</tr>
<tr class="odd">
<td><p>MAPPING SOURCE COMPLETED</p></td>
<td><p>Displays the number of field mappings that have MAPPING STATUS and RULES STATUS set to <strong>Complete</strong> on the <em>Field Mappings</em> page.</p></td>
</tr>
<tr class="even">
<td><p>MAPPING SOURCE TOTAL</p></td>
<td><p>Displays the number of fields that have been mapped for the Source.</p></td>
</tr>
</tbody>
</table>

## <span id="Target_Dashboard_Stats_V"></span>Target Dashboard Stats V

[Target Dashboard Stats H](Target_Dashboard_Stats_H.htm)

<div class="use">

Use this page to [View Metrics](../Use_Cases/View_Metrics_Map.htm).

</div>

Field

Description

Name

Displays the object name defined in Console. Click the link to open the
*[Objects](../../Console/Page_Desc/Objects_H.htm)* page to view details
about the object.

Target

Displays the Target table name. Click the link to open the
*[Targets](Targets_H_Map.htm)* page to view details about the Target.

Percentages

Percentage Source Non Field Group

Displays the percent complete of Non Field group field mappings (as in,
field mappings that belong to the default field group (\*)).

**NOTE:** It is a requirement that all fields be mapped in a Source even
if the field mapping has an action of Not Used.

Field groups are assigned in Target Design, and allow users to apply
filters for mapping based on certain values in a field.

Refer to [Work with Field
Groups](../../Design/Use_Cases/Work_with_Field_Groups.htm) for more
information.

Percentage Source Field Group

Displays the percent complete of Field group field mappings (as in,
field mappings that do not belong to the default field group (\*)).

Field groups and their associated Field Groups are optional mappings to
create data-driven filter updates.

Refer to [Work with Field
Groups](../../Design/Use_Cases/Work_with_Field_Groups.htm) for more
information.

Percentage Target Rule Non Field Group

Displays the percent complete of Target Rule Non Field group field
mappings (as in, field mappings that display {Target Rules} in TARGET
SOURCE DETAILS on the *[Field Mappings](Field_Mappings_H.htm)* page, and
that belong to the default field group (\*)).

**NOTE:** A field mapping of {Target Rules} is not required for any
fields but may be necessary. The value uses those mappings of {Target
Rules} where ACTION is not blank.

Percentage Target Rule Field Group

Displays the percent complete of Target Rule Field group field mappings
(as in, field mappings that display {Target Rules} in TARGET SOURCE
DETAILS on the *Field Mappings* page, and that do not belong to the
default field group (\*)).

**NOTE:** A field mapping of {Target Rules} is not required for any
fields but may be necessary. The value uses those mappings of {Target
Rules} where ACTION is not blank.

Refer to [Work with Field
Groups](../../Design/Use_Cases/Work_with_Field_Groups.htm) for more
information.

Field Counts

Active Fields

Displays the number of active field that have to be mapped for the
selected Target.

All Fields

Displays the total field count in the Target table.

Source Mappings

Mapping Source Completed

Displays the number of field mapping that have MAPPING STATUS and RULE
STATUS set to Complete on the *Field Mappings* page for the selected
Target.

Mapping Source Total

Displays the number of fields that have been mapped for the Source.

Field Group Completed

Displays the number of field groups that have all mappings completed.

Field Group Total

Displays the number of field groups created in the Source.

Target Mappings

Target Rule Non Field Group Completed

Displays the number of completed Target Rule Non Field group field
mappings (those field mappings that display {Target Rules} in TARGET
SOURCE DETAILS on the *Field Mappings* page, and that belong to the
default field group (\*).

Target Rule Non Field Group Total

Displays the number of Target Rule Non Field group field mappings (those
field mappings that display {Target Rules} in TARGET SOURCE DETAILS on
the *Field Mappings* page, and that belong to the default field group
(\*).

Target Rule Field Group Completed

Displays the number of completed Target Rule Field group field mappings
(those field mappings that display {Target Rules} in TARGET SOURCE
DETAILS on the *Field Mappings* page, and that do not belong to the
default field group (\*).

Target Rule Field Group Total

Displays the number of Target Rule Field group field mappings (those
field mappings that display {Target Rules} in TARGET SOURCE DETAILS on
the *Field Mappings* page, and that do not belong to the default field
group (\*).
