+++
title = 'Target Sources (Update Row) H'
solution = 'Migration'
+++

# Target Sources (Update Row) H

[Target Sources (Update Row)
V](Target_Sources_Update_Row#Target_Sources__Update_Row__V)

<div class="use">

Use this page to:

  - [Add Add Row Sources](../Use_Cases/Add_an_Add_Row_Source)
  - [Add Update Row Sources](../Use_Cases/Add_Update_Row_Sources)
  - [Add an External Source](../Use_Cases/Add_an_External_Source)
  - [Add Relationship Joins to
    Sources](../Use_Cases/Add_Relationship_Joins_to_Source)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Map </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](Process_Area_Launch_map)* page.
4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.
5.  Click the <span style="font-weight: bold;">Update Row Sources</span>
    icon for a Source.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Auto Map</p></td>
<td><p>Click to create a copy of the rule mappings for fields that exist in the Target table and the source database object. The fields in the Target table and the source database object must match for rule mappings to be created.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE ID</p></td>
<td><p>Displays the source name.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE DATABASE OBJECT</p></td>
<td><p>Displays name of the source table or view, or indicates if the source is an Update Row source.</p>
<p><strong>NOTE:</strong> When a user sets the source database object and clicks Save, Map validates that the source database object exists in the System Type. If the source database object does not exist:</p>
<p>If the user imported a System Type in Target Design for the Target Source, the source database object is imported into the System Type.</p>
<p>If the user did not import a System Type in Target Design (as in, an Excel file import, database table import, or manual entry was used for the Target Design), Map displays an error message that the user must set a System Type before field mapping can be performed. Add a System Type to a Target in Target Design (Design &gt; Targets &gt;Vertical View for a Target &gt; System Type ID).</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If checked, the source is active for the Wave.</p></td>
</tr>
<tr class="even">
<td><p>Mappings</p></td>
<td><p>Click to open the <em><a href="Field_Mappings_H">Field Mappings</a></em> page to create and reset field mappings for all fields in the selected Update Row source, to view the history for a selected mapping, or to view mapping details. A number does not display on this icon if no field mappings have been activated for the current context.</p></td>
</tr>
<tr class="odd">
<td><p>Relationships</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Relationship_Joins_H">Relationship Joins</a></span> page to add relationship joins for Add Row and Update Row source tables.</p>
<p>When a Target is synced with Target Design, relationships are loaded for the Target based on the dependencies set in Target Design.</p>
<p>For example, the MARC table has a parent relationship with the MARD table (as in, MARD is a child of MARC).</p>
<p>The key fields used in the relationship between the tables are MATNR and WERKS.</p>
<p>A user can build a relationship between the two tables, but the relationship join is only entered for the MARD table.</p>
<p>The MARA table is a parent of the MARC, MAKT, and MARM tables. The key field for the relationship join in these cases is the MATNR field.</p>
<p>Relationships must be built at the child table level (as in, MARC, MAKT, and MARM).</p></td>
</tr>
</tbody>
</table>

 

## <span id="Target_Sources__Update_Row__V"></span>Target Sources (Update Row) V

[Target Sources (Update Row) H](Target_Sources_Update_Row)

Field

Description

Copy To

Click to open the *[Target Source Copy To](Target_Source_Copy_To)*
page to copy source mappings from the current Target Source to another
Target Source combination.

Export Field Mappings

Click to export all field mappings with a MAPPING STATUS and a RULE
STATUS of Complete on the *[Field Mappings](Field_Mappings_H)* page
to the Common System Tables to be imported into Waves and other Process
Areas.

Import Field Mappings

Click to open the*[Import Field
Mappings](Import_Field_Mappings)*page to review and import all
available mappings approved in other Waves to the current source.

Auto Update Not Used

Click to set all blank Actions to “NotUsed” for the Target Source
mappings.

Basic Details

Mapping Required

If checked, the Update Row source must be mapped.

Track Changes

If checked, workflow notifications are sent to users who are set up to
receive mapping changes. Refer to [Set up User
Notifications](../Config/Setup_User_Notifications) for more
information.

Comment

Displays a brief, user-defined comment about the source.

Relationships

Click to open the <span style="font-style: italic;">[Relationship
Joins](Relationship_Joins_H)</span> page to add relationship joins
for Add Row and Update Row source tables.

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
and MARM).

Source Schema

Source ID

Displays the name of the source.

Source Database Object

Displays name of source table or view, or indicates if the source is an
Update Row source.

Schema Columns

Click to open the <span style="font-style: italic;">[Target Source
Schema](Target_Source_Schema_H)</span> page to reset Target Source
schema field lengths. If a source was added in Target Design during a
System Type import, and the System Type tables for a source contained an
invalid length for a column, use the Reset functionality to update a
source table with the column’s correct length.

System Type Table Fields

Click to open the <span style="font-style: italic;">[System Types Tables
Fields](../../../Platform/Common/Page_Desc/System_Types_Table_Fields_H)</span>
page to view the fields in the source table.

ST Table Settings

ST Object Type

Displays table or view.

A view in the Transform database contains the rule that processes
against the data in the source database.

A table allows a user to pull data from the same source database that
the rule processes against, but to convert the data before it is
processed in a rule for the Target Source table. Using mappings, SQL
AutoGen can create these pre-processing rules that are run prior to the
main source rules.

Update Row Source

Displays the name of the source table for the update row source.

Add Row Source

Displays the name of the Add Row source added in Map and populated by
the system. This field must be populated for SQL AutoGen to generate
rules

**NOTE:** If the Add Row source has an Add Row Source Override field
entered on the <span style="font-style: italic;">Vertical V</span>iew of
the <span style="font-style: italic;">[Target
Sources](Target_Sources_H_Map)</span> page, then the Update Row
source’s Update Row Source Override field on this page must match the
Add Row Source Override field.

Update Row Source Override

Displays the user-selected table name that overrides the St Table in the
Add Row source, which is used to download data from another table or
view.

**NOTE:** If the Add Row source has an Add Row Source Override field
entered on the <span style="font-style: italic;">Vertical V</span>iew of
the <span style="font-style: italic;">[Target
Sources](Target_Sources_H_Map)</span> page, then the Update Row
source’s Update Row Source Override field on this page must match the
Add Row Source Override field.

Table Details

**NOTE:** This label and the icons below it do not display if a source
database object has not been set. This is set on the
<span style="font-style: italic;">Horizontal</span> View of the
<span style="font-style: italic;">[Target Source (Add
Row](Target_Sources_Add_Row))</span> or [Target Sources (Update
Row)](Target_Sources_Update_Row) page.

Profile

Click to profile the source data source which gathers information about
the tables and fields such as record counts, unique values, or field
data types.

View Data

Click to open the [Target Sources](Target_Sources_H_Map) page to
view the source data.

View Fields

Click to open the <span style="font-style: italic;">[Table Field
(Results)](../../../Platform/Common/Page_Desc/Table_Field_Results_H)</span>
page to view profile results such as field data type, length, the
percentage of fields that do not have data, and the percentage of fields
that have unique values.
