+++
title = ''
solution = 'Migration'
+++

# <span id="Target_Sources_H"></span>Target Sources H

[Target Sources V](#Target_Sources_V)

<div class="use">

Use this page to:

  - [Set a Source Database
    Object](../Use_Cases/Perform_Field_Mapping.htm#Set_a_Source_Database_Object)
  - [Add ZActive Fields](../Use_Cases/Add_ZActive.htm)
  - [Update Client and Language for all
    Sources](../Use_Cases/Update_Client_and_Language_for_all_Sources.htm)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Map </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span> icon on
    the *[Process Area Launch](Process_Area_Launch_map.htm)* page.
4.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Sync from Target Design</p></td>
<td><p>Click to sync Map with Target Design, updating tables, fields, Sources and lookup tables.</p>
<p>When Map and Target Design are out of sync, the message Pending Design Changes displays to the right of the page name.</p></td>
</tr>
<tr class="odd">
<td><p>Auto Map</p></td>
<td><p>Click to create a copy of the rule mappings for fields that exist in the target table and the Source database object. The fields in the target table and the Source database object must match in order for rule mappings to be created.</p>
<p><strong>NOTE:</strong> The Auto Map feature sets the Action on the mapping to Copy and the Mapping Status to In Progress.</p></td>
</tr>
<tr class="even">
<td><p>SOURCE ID</p></td>
<td><p>Displays name of the Source database as defined in Target Design.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE DATABASE OBJECT</p></td>
<td><p>Displays name of the Source table or view, or indicates if the Source is an Update Row Source.</p>
<p><strong>NOTE:</strong> When a user sets the Source database object and clicks Save, Map validates that the Source database object exists in the System Type. If the Source database object does not exist:</p>
<p>If the user imported a System Type in Target Design for the Target Source, the Source database object is imported into the System Type.</p>
<p>If the user did not import a System Type in Target Design (as in, an Excel file import, database table import, or manual entry was used for the target design), Map displays an error message that the user must set a System Type before field mapping can be performed. Add a System Type to a target in Target Design (Design &gt; Targets &gt;Vertical View for a target &gt; System Type ID).</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If checked, the Source is active for the Wave.</p></td>
</tr>
<tr class="odd">
<td><p>Update Row Sources</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Target_Sources_Add_Row.htm">Target Sources (Add Row)</a></span> page to add an Update Row Source to the selected Add Row.</p>
<p>Add an Update Row when data from another Source table is needed to update the Add Row Source.</p>
<p>Refer to <a href="../Use_Cases/Add_Update_Row_Sources.htm">Add Update Row Sources</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Mappings</p></td>
<td><p>Click to open the <em><a href="Field_Mappings_H.htm">Field Mappings</a></em> page to create and reset field mappings for all fields in the context, to view the history for a selected mapping, or to view mapping details. A number does not display on this icon if no field mappings have been activated for the current context.</p></td>
</tr>
</tbody>
</table>

## <span id="Target_Sources_V"></span>Target Sources V

[Target Sources H](#Target_Sources_H)

<div class="use">

Use this page to:

  - [Add ZActive](../Use_Cases/Add_ZActive.htm)
  - [Update Unmapped Add Row and Update Row Source Fields to
    NotUsed](../Use_Cases/Update_Unmapped_Fields_to_NotUsed.htm#Update_Add_Row_and_Update_Row_Source_Fields)
  - [Add Update Row Sources](../Use_Cases/Add_Update_Row_Sources.htm)
  - [Update Client and Language for all
    Sources](../Use_Cases/Update_Client_and_Language_for_all_Sources.htm)
  - [Add an Assemble Where
    Clause](../Use_Cases/Add_Assemble_Where_Clause.htm)

</div>

Field

Description

Copy To

Click to open the <span style="font-style: italic;">[Target Source Copy
To](Target_Source_Copy_To.htm)</span> page to copy Source mappings from
the current Target Source to another Target Source combination.

Export Field Mappings

Click to export all field mappings with a MAPPING STATUS and a RULE
STATUS of Complete on the *[Field Mappings](Field_Mappings_H.htm)* page
to the Common System Tables to be imported into Waves and other Process
Areas.

Import Field Mappings

Click to open the <span style="font-style: italic;">[Import Field
Mappings](Import_Field_Mappings.htm)</span> page to review and import
all available mappings approved in other Waves to the current Source.

Auto Update Not Used

Click to set all blank Actions to “NotUsed” for the Target Source
mappings.

Reset

Click to reset the <span style="font-style: italic;">[Target Source
Schema](Target_Source_Schema_H.htm) </span>page.

Resetting re-imports any additional fields for this Add Row Source from
the System Type.

Basic Details

Track Changes

If checked, workflow notifications are sent to users who are set up to
receive mapping changes. Refer to [Set up User
Notifications](../Config/Setup_User_Notifications.htm) for more
information.

Comment

Displays a brief, user-defined comment about the Source.

Source Schema

Source ID

Displays name of the Source database as defined in Target Design.

Source Database Object

Displays name of Source table or view, or indicates if the Source is an
Update Row Source.

Source Type

Displays the Source type: Add Row or Update Row. Update Row is used if
an Update Row Source is used to update the values. Default value is
Update Row. Add Row is used when there are two Source data tables within
the same Source.

Schema Columns

Click to view a list of Source schema columns used to build the Source
table.

System Type Table Fields

Click to display the [System Types
Tables](../../../Platform/Common/Page_Desc/System_Types_Tables_H.htm)
page to view or update the System Type table & fields.

ST Table Settings

St Object Type

Displays the type of object in the Source: Table or View. Default value
is Table.

St Table

Displays the name of the Map-generated table that rules are created
against.

Add Row Source Override

Displays the user-selected table name that overrides the St Table in the
Add Row Source, which is used to download data from another table or
view.

Active Field

Displays user-defined value to filter data in a Source table that is
loaded into a target table.

z Source

Displays the name of Source where data is being created. This field is
set in Target Design.

z Source Override

Displays user-entered Source that overrides the ZSource for the target
configured in Target Design.

Assemble Where Clause

Displays the Assemble Where Clause to be added to the CranPort package.
The Assemble Where Clause is used to filter Source data when importing
or refreshing a target. The Where Clause must consist of a column name,
an operator and a value. For example, Country = 'US'.

Table Details

**NOTE:** This label and the icons below it do not display if a Source
database object has not been set. This is set on the
<span style="font-style: italic;">Horizontal</span> View of the [Target
Source (Add Row)](Target_Sources_Add_Row.htm) or [Target Sources (Update
Row)](Target_Sources_Update_Row.htm) page.

Profile

Click to profile the Source data source which gathers information about
the tables and fields such as record counts, unique values, or field
data types.

View Data

Click to open the [Target Sources](Target_Sources_H_Map.htm) page to
view the Source data.

View Fields

Click to open the <span style="font-style: italic;">[Table Field
(Results)](../../../Platform/Common/Page_Desc/Table_Field_Results_H.htm)</span>
page to view profile results such as field data type, length, the
percentage of fields that do not have data, and the percentage of fields
that have unique values.

Value Mapping Settings

Client

Displays the name of the field that contains ERP system client
information.

This value is entered in Target Design on the *Vertical* View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.

Language

Displays the name of the field that contains the ERP system client
information.

This value is entered in Target Design on the *Vertical* View of the
*[Target Lookup
Table](../../Design/Page_Desc/Target_Lookup_Table_H.htm)* page.
