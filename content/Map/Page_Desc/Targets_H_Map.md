# Targets H

[Targets V](#Targets_V)

<div class="use">

Use this page to:

  - [Sync Map and Target
    Design](../../Design/Use_Cases/Sync_Map_and_Target_Design_TD.htm)
  - [Build a Remediation
    Report](../Use_Cases/Build_a_Remediation_Report.htm)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspMigrate</span> in the
    *Navigation* pane.
2.  Click <span style="font-weight: bold;">Map </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](Process_Area_Launch_map.htm)* page.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Sync From Target Design</p></td>
<td><p>Click to sync Map with Target Design, updating tables, fields, Sources and lookup tables.</p>
<p>When Map and Target Design are out of sync, the message Pending Design Changes displays to the right of the page name</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the order in which Targets are mapped.</p></td>
</tr>
<tr class="even">
<td><p>OBJECT</p></td>
<td><p>Displays name of the object as defined in Console.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET ID</p></td>
<td><p>Displays name of the Target for Map and Transform.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays brief description of the Target table.</p></td>
</tr>
<tr class="odd">
<td><p>Sources</p></td>
<td><p>Click to open the <em><a href="Target_Sources_H_Map.htm">Target Sources</a></em> page to view Sources registered to the Target and to create Sources, to perform field mappings at the Source level, to auto map Sources, to view details about the Target Sources assigned to the current context and to assign relationships for Target Sources.</p></td>
</tr>
<tr class="even">
<td><p>Field Groups</p></td>
<td><p>Click to open the <em><a href="Target_Field_Groups.htm">Target Field Groups</a></em> page to manage field groups.</p>
<p>Field groups are assigned in Target Design, and allow users to apply filters for mapping based on certain values in a field. Refer to <a href="../../Design/Use_Cases/Work_with_Field_Groups.htm">Work with Field Groups</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Target Rules</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Field_Mappings_H.htm">Field Mappings</a></span> page. Accessed from this icon, the page displays mappings for Target rules only.</p></td>
</tr>
<tr class="even">
<td><p>Mappings</p></td>
<td><p>Click to open the <em><a href="Field_Mappings_H.htm">Field Mappings</a></em> page to submit and reset field mappings for all fields in the context, to view the history for a selected mapping, or to view mapping details. A number does not display on this button if no field mappings have been activated for the current context.</p></td>
</tr>
</tbody>
</table>

## <span id="Targets_V"></span>Targets V

[Targets H](Targets_H_Map.htm)

Use this page to:

<div class="use">

  - [Sync Map and Target
    Design](../../Design/Use_Cases/Sync_Map_and_Target_Design_TD.htm)
  - [Build a Remediation
    Report](../Use_Cases/Build_a_Remediation_Report.htm)

</div>

Field

Description

Copy To

Click to open the *[Target Source Copy To](Target_Source_Copy_To.htm)*
page to copy mappings from the current Target rule to another Target
rule combination.

Export Field Mappings

Click to open the [Export Field Mappings](Export_Field_Mappings.htm)
page to export Target rule mappings with a MAPPING STATUS and a RULE
STATUS of Complete on the Field Mappings page to the Common System
Tables to be imported into Waves and other Process Areas.

Import Field Mappings

Click to open the *[Import Field Mappings](Import_Field_Mappings.htm)*
page to review and import Target rule mappings approved in other Waves
to the current Target.

Reset

Click to reset the processing status if a process fails for any of the
Target’s actions.

Target Id

Displays name of Target for Map and Transform. This is a Target table in
the Transform Object database.

Relationships

Click to open the <span style="font-style: italic;">[Relationship
Joins](Relationship_Joins_H.htm)</span> page to add relationship joins
for Add Row and Update Row Source tables.

When a Target is synced with Target Design, relationships are loaded for
the Target based on the dependencies set in Target Design.

For example, the MARC table has a parent relationship with the MARD
table (as in, MARD is a child of MARC).

The key fields used in the relationship between the tables are MATNR and
WERKS.

A user can build a relationship between the two tables, but the
relationship join is only entered for the MARD table.

The MARA table is a parent of the MARC, MAKT, and MARM tables. The key
field for the relationship join in these cases is the MATNR field.

Relationships must be built at the child table level (as in, MARC, MAKT,
AND MARM).

ERP Table Name

Displays ERP table name where data will be loaded.

Data Source ID

Displays database name containing the Target table.

Create Target Details

Target Built By

Displays user ID of individual who last built the Target table.

Target Build On

Displays date and time when Target table was last built.
