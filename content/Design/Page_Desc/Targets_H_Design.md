# Targets H

[Targets V](#Targets_V)

<div class="use">

Use this page to:

  - [Sync Map and Target
    Design](../Use_Cases/Sync_Map_and_Target_Design_TD.htm)
  - [Add a Basic Rule](../Use_Cases/Basic_Rules.htm)
  - [Set a Target's Design
    Status](../Use_Cases/Set_the_Design_Status.htm)
  - [Set Target Dependencies](../Use_Cases/Set_Target_Dependencies.htm)

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span>icon on the
    *[Design](Design.htm)* page.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Target Import</p></td>
<td><p>Click to open the <em><a href="Target_Object_Import.htm">Target Object Import</a></em> page, to begin the process of importing a System Type, database table or Excel file as the basis for a Target design.</p>
<p><strong>NOTE</strong>: When accessing the <span style="font-style: italic;">Target Object Import</span> page from the Target Import icon, the Object selected on the <span style="font-style: italic;"><a href="#">Targets</a></span> page is not carried over to the <span style="font-style: italic;">Target Object Import</span> page. The Object where the Target design is to be imported must be selected on the <span style="font-style: italic;">Target Object Import</span> page.</p></td>
</tr>
<tr class="odd">
<td><p>Import Fields</p></td>
<td><p>Click to load all fields found in the System Type for Target System Table Name into DSPTM.</p>
<p><strong>NOTE</strong>: The Import Fields icon on the Targets page works the same as the Execute Import icon on the <span style="font-style: italic;"><a href="System_Type_Import.htm">System Type Import</a></span> page. The user has the option to import one Target at a time on the Targets page or import one or more Targets on the System Type Import page.</p></td>
</tr>
<tr class="even">
<td><p>Sync to Map</p></td>
<td><p>Click to sync the selected Target to Map if the STATUS field displays &quot;Pending Design Changes.” If updates have been made in Target Design to Targets, Sources, Target fields, or lookup tables after they have been loaded into Map, this process syncs those updates with the data in Map.</p>
<p>Refer to <a href="../Use_Cases/Sync_Map_and_Target_Design_TD.htm">Sync Map and Target Design</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Object ID</p></td>
<td><p>Displays the Object to which the Target is assigned. Objects can have multiple Targets assigned. Objects are added in Console and assigned to a Wave-Process Area to create a context.</p>
<p>A Target design is imported into the Object selected on the <span style="font-style: italic;"><a href="Target_Object_Import.htm">Target Object Import</a></span> page.</p>
<p> A user can also select an Object when adding the Target manually.</p></td>
</tr>
<tr class="even">
<td><p>STATUS OF SYNC</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Target_Design_Pending_Changes.htm">Target Design Pending Changes</a></span> page to view the change to the Target that must be synced with Map.</p>
<p>If the field is blank, the Target is in sync in Map and Target Design.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the display order of the Target on the <em>Targets</em> page.</p>
<p>When a Wave-Process Area uses the Object, the Object priority cascades down to Target Design. Once the Target that belongs to the Object is synced with Map, the priority is also available in Map and displays on the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Objects_map.htm">Objects</a></span> page. The Priority field in Transform is not updated. To change the order the Object is processed, the Priority field can be updated manually in Transform on the <span style="font-style: italic;">Targets</span> page (Process Area Launch &gt; Targets).</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the Target name, which is the table name with tt appended to the front.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays a brief description of the Target table.</p></td>
</tr>
<tr class="even">
<td><p>DESIGN STATUS</p></td>
<td><p>Displays the status of the Target design.</p>
<p>Values are:</p>
<ul>
<li><span style="font-weight: bold;">In Design</span> – A Target is in this Design Status when it has been added and while the Target is being configured. All functionality that can be performed on a Target is available and the Sync to Map icon is enabled.</li>
<li><span style="font-weight: bold;">Design Finished</span> – When a Target is in this status, the design is locked down, and no changes are allowed. A Target can only move to this status if it is in sync with Map. The Sync to Map icon is enabled. Auto Generation in Data Services and in SQL is allowed.</li>
<li><span style="font-weight: bold;">Completed</span> When a Target is in this status, the design is locked down, and no changes are allowed. A Target can only move to this status if it is in sync with Map. Auto-generation in Data Services and in SQL is not allowed. The Sync to Map icon is disabled.</li>
<li><span style="font-weight: bold;">Inactive</span> A Target in Inactive status will not be pushed to Map for mapping and is not available in Transform. When a Target in this status is selected, the Sync to Map icon is disabled.</li>
</ul>
<p>Refer to <a href="../Use_Cases/Set_the_Design_Status.htm">Set a Target's Design Status</a>  for more information.</p></td>
</tr>
<tr class="odd">
<td><p>EXECUTION STATUS</p></td>
<td><p>This field is not currently used, but will be activated in a future release.</p></td>
</tr>
<tr class="even">
<td><p>USAGE</p></td>
<td><p>Displays how data in the Target table moves through the migration process.</p>
<ul>
<li><strong>Natural</strong> - The Target follows the standard migration process. The Target fields and Source must be entered or imported into Target Design and synced to Map. Map must have Source tables selected and fields mapped. SQL AutoGen creates the Target table, Source table, and rules Objects.</li>
<li><strong>Utility</strong> – The Target is not mapped in Map and SQL AutoGen does not create any Objects. A user must still enter the Target into Target Design and the Target’s fields and Sources. The Target tables, Source Tables and rule Objects must be created manually.</li>
</ul>
<p><strong>NOTE</strong>: If the client’s installation is upgraded from a version that did not use Waves and Process Areas, all Targets are set to Utility</p>
<p><strong>NOTE</strong>: A visibility can be set so that Utility fields can be mapped. Refer to <a href="../Use_Cases/Set_Field_Visibility_for_Mapping.htm">Set Field Visibility for Mapping</a> for more information.</p>
<p><strong>NOTE</strong>: By default, the visibility of a Utility field is set to NONE, with the exception of zLegacy keys. zLegacy key fields will default to Source visibility.  Refer to <a href="../Use_Cases/Allow_Mapping_of_Utility_Columns.htm">Allow Mapping of Utility Columns</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET SYSTEM TABLE NAME</p></td>
<td><p>Displays the name of the table in the Target system, which is the name in the NAME field without the tt appended to the front.</p></td>
</tr>
<tr class="even">
<td><p>SYSTEM TYPE ID</p></td>
<td><p>Displays the System Type that was imported to create the Target design, or the System Type that was selected for the Target.</p>
<p>Refer to <a href="../../../Platform/Common/Use_Cases/System_Types_Overview.htm">System Types</a>  for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Sources</p></td>
<td><p>Click to open the <em><a href="Target_Sources_H_Design.htm">Target Sources</a></em> page to add a Source to the Target.</p>
<p>Refer to <a href="../Use_Cases/Assign_a_Source_to_a_Target.htm">Assign a Source to a Target</a>  for more information.</p></td>
</tr>
<tr class="even">
<td><p>Fields</p></td>
<td><p>Click to open the <em><a href="Target_Fields_H_Target_Design.htm">Target Fields</a></em> page to add a field to the Target or activate or deactivate fields for mapping.</p>
<p>Refer to <a href="../Use_Cases/Add_Fields_to_a_Target.htm">Add Fields to a Target</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Basic Rules</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Rules_Basic_Rule_H.htm">Rules: Basic Rules</a></span> page to view all basic rules assigned to active fields in the Target.  Basic rules are logic conditions to apply to the data in the associated field.</p>
<p><strong>NOTE</strong>: If the field is a zLegacy field, this icon is disabled.</p>
<p>Refer to <a href="../Use_Cases/Basic_Rules.htm">Add a Basic Rule</a>  for more information.</p></td>
</tr>
<tr class="even">
<td><p>Mapping</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Targets_H_Map.htm">Targets</a></span>page in Map to view all field mappings for the selected Target.</p></td>
</tr>
<tr class="odd">
<td><p>Developers</p></td>
<td><p>Click to open the <em><a href="Target_Contacts.htm">Target Contacts</a></em> page to add Developers to the Target. Developers approve mappings submitted for this Source on the <em>Mapping Approval</em> page (Quick Panel &gt; Mapping Approval).</p>
<p>Refer to <a href="../Use_Cases/Add_Developers_and%20Business%20Contacts.htm">Add Developers and Business Contacts to a Target or Source</a>  and  <a href="../../Map/Use_Cases/Approve_or_Reject_Mappings.htm">Approve or Reject Field Mappings</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Business Contacts</p></td>
<td><p>Click to open the <em><a href="Target_Contacts.htm">Target Contacts</a></em> page to assign Business Contacts to the selected Target. Business Contacts are used for reporting purposes and automatically receive public reports for the Target–Source in Transform.</p>
<p>Refer to <a href="../Use_Cases/Add_Developers_and%20Business%20Contacts.htm">Add Developers and Business Contacts to a Target or Source</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Summary Construction</p></td>
<td><p>Click to open a dashboard that displays a summary of estimated records and completed records in Construct for the Target.</p>
<p>Refer to <a href="../../Construct/Use_Cases/View_Dashboard_in_Construct.htm">View the Dashboard in Construct</a>  for more information.</p></td>
</tr>
<tr class="even">
<td><p>Dependencies</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Target_Dependencies.htm">Target Dependencies</a></span> page to set a parent dependency for the selected Target table.</p>
<p>Refer to <a href="../Use_Cases/Set_Target_Dependencies.htm">Set Target Dependencies</a> for more information.</p></td>
</tr>
</tbody>
</table>

<div>

-----

</div>

 

## <span id="Targets_V"></span>Targets V

[Targets H](Targets_H_Design.htm)

<div class="use">

Use this page to [Set the Field Formats for Date, Time, and Decimal For
Use in Data Services
AutoGen](../Use_Cases/Set_Date_Time_and_Decimal_Format.htm).

</div>

Field

Description

Basic

Object Id

Displays the Object to which the Target is assigned. Objects can have
multiple Targets assigned. Objects are added in Console and assigned to
a Wave-Process Area to create a context.

A Target design is imported into the Object selected on
the<span style="font-style: italic;"> Target Object Import</span> page
(Design \> Target Import).  

A user can also select an Object when adding the Target manually.

Priority

Displays the display order of the Target on the *Targets* page.

When a Wave-Process Area uses the Object, the Object priority cascades
down to Target Design. Once the Target that belongs to the Object is
synced with Map, the priority is also available in Map and displays on
the <span style="font-style: italic;">Objects</span> page (Process Area
Launch \> Objects). The Priority field in Transform is not updated. To
change the order the Object is processed, the Priority field can be
updated manually in Transform on the
<span style="font-style: italic;">Targets</span> page (Process Area
Launch \> Targets).

Name

Displays the Target name, which is the table name with tt appended to
the front.

Description

Displays a brief description of the Target table.

Usage

Displays how fields in the Target are used.

Values are:

  - <span style="font-weight: bold;">Natural</span> – The fields exist
    in the Target system. The system adds a “z” to the front of the
    field name used in the Source table.
  - <span style="font-weight: bold;">Utility</span> – The fields do not
    exist in the Target system, but can be used to register rules and
    reports to in Transform. Fields of this type should be captured in
    Target Design. A utility field is added to the Target table to be
    used by the AutoGen process. Utility fields will be appended to BOTH
    the Target and Source table as is. No “z” field will be appended.

**NOTE**: A visibility can be set so that Utility fields can be mapped.
Refer to [Set Visibility for Mapping of Target and Source
Fields](../Use_Cases/Set_Field_Visibility_for_Mapping.htm)  for more
information.

**NOTE**: By default, the visibility of a Utility field is set to NONE,
with the exception of zLegacy keys. zLegacy key fields will default to
Source visibility. Refer to [Set Visibility for Appended Utility
Columns](../Use_Cases/Allow_Mapping_of_Utility_Columns.htm) for more
information.

Target System Table Name

Displays the name of the table in the Target system, which is the name
in the NAME field without the tt appended to the front.

System Type ID

Displays the System Type that was imported to create the Target design,
or the System Type that was selected for the Target.

Refer to [Import a Target Design from a System
Type](../Use_Cases/Import_from_a_System_Type.htm) and [System
Types](../../../Platform/Common/Use_Cases/System_Types_Overview.htm)
 for more information.

Details

Comments

Displays a user-entered comment about the Target.

This field is for documentation purposes only.

Instructions

Displays instructions about how to use the Target in mapping or other
functions.

This field is for documentation purposes only.

Documentation

Click Upload a file to upload documentation related to the Target field.
If documentation has been uploaded, the Download a File icon is active,
and the file can be downloaded. The Download a File icon is disabled if
no documentation has been uploaded for the Target.

Dependencies

Parent Targets

Click to open the <span style="font-style: italic;">[Target Dependency
(Parents)](Target_Dependency_Parents.htm)</span> page to view a list of
Target tables that have a parent dependency with the selected Target
(i.e., the selected Target is a child of the Targets that display on
this page).

The number on the icon represents the number of Targets that have a
parent dependency with the selected Target.

Refer to [Set Target
Dependencies](../Use_Cases/Set_Target_Dependencies.htm) for more
information.

Child Targets

Click to open the <span style="font-style: italic;">[Target Dependency
(Children)](Target_Dependency_Children.htm)</span> page to view a list
of Target tables that have a child dependency with the selected Target
(i.e., the selected Target is a parent of the Targets that display on
this page).

The number on the icon represents the number of Targets that have a
child dependency with the selected Target.

Refer to [Set Target
Dependencies](../Use_Cases/Set_Target_Dependencies.htm) for more
information.

Field Formats

Date Format

Displays the format to use for date fields when writing validation rules
in Data Services AutoGen.

The Date Format works in conjunction with the Field Format field on the
<span style="font-style: italic;">Target Fields</span> page's
<span style="font-style: italic;">Vertical</span> View, where the type
of format for data fields is stored.

For example, the Date Format for a Target is set in this field at
YYYYDDMM.

A  user selects Date in the Field Format list box on the
<span style="font-style: italic;">Target Fields Vertical</span> View for
the field Received By Date.

The data in the Received By Date field passes through the migration
process with a data type of NVARCHAR. When validation rules are written
for this field in Date Services AutoGen, the format of the data in the
Received By Date field is formatted as YYYYDDMM so that it can be loaded
into the Target with no errors.

Refer to [Set the Date, Time, and Decimal
Formats](../Use_Cases/Set_Date_Time_and_Decimal_Format.htm) for more
information.

Time Format

Displays the format to use for time fields when writing validation rules
in Data Services AutoGen.

The Time Format works in conjunction with the Field Format field on the
<span style="font-style: italic;">Target Fields</span> page's
<span style="font-style: italic;">Vertical</span> View, where the type
of format for data fields is stored.

For example, the Time Format for a Target is set in this field as
HH:MM:SS.

A  user selects Time in the Field Format list box on the
<span style="font-style: italic;">Target Fields Vertical</span> View for
the field Received By Time.

The data in the Received By Time field passes through the migration
process with a data type of NVARCHAR. When validation rules are written
for this field in Date Services AutoGen, the format of the Received By
Time field is set as HH:MM:SS so that it can be loaded into the Target
with no errors.

Refer to [Set the Field Formats for Date, Time, and Decimal For Use in
Data Services
AutoGen](../Use_Cases/Set_Date_Time_and_Decimal_Format.htm) for more
information.

Decimal Format

Displays the separator format (either "," or ".") to use for decimal
fields when writing validation rules in Data Services AutoGen.

The Decimal Format works in conjunction with the Field Format on the
<span style="font-style: italic;">Target Fields</span> page's
<span style="font-style: italic;">Vertical</span> View, where the type
of format for data fields is stored.  

Refer to [Set the Field Formats for Date, Time, and Decimal For Use in
Data Services
AutoGen](../Use_Cases/Set_Date_Time_and_Decimal_Format.htm) for more
information.

Advanced

Target Table Join

Click to open the *[Target Table
Join](Target_Table_Joins_Target_Design.htm)* page to view or enter
information about joins in Target tables for the selected Target. This
information is for documentation purposes only.
