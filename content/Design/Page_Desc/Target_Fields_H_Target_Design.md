+++
title = 'Target Fields H'
solution = 'Migration'
+++

# Target Fields H

[Target Fields V](Target_Fields_H_Target_Design#Target_Fields_V)

<div class="use">

Use this page to

  - [Add Fields to a Target](../Use_Cases/Add_Fields_to_a_Target)
  - [Activate or Deactivate Target Fields for
    Mapping](../Use_Cases/Activate_Fields_for_Map)
  - [Extend Fields to Field
    Groups](../Use_Cases/Extend_a_Field_to_a_Field_Group)

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. Refer to [Use Bulk
Execution](../../../Platform/Bulk_Exec/Use_Bulk_Execution) for more
information.

To access this page:

1.  Select <span style="font-weight: bold;">dspMigrate</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Select <span style="font-weight: bold;">Design </span>in the Context
    bar.
3.  Click the <span style="font-weight: bold;">Targets</span>icon on the
    *[Design](Design)* page.
4.  Click the <span style="font-weight: bold;">Fields</span> icon for a
    Target.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Extend To Field Groups</p></td>
<td><p>Click to add the selected field to all field groups in the object.</p>
<p>Field groups are filters used to create subsets of data in a Target field. Rules, requirement settings, criticality levels and other settings can then be applied to these subsets of data.</p>
<p>A field can be extended to all field groups assigned to the object allowing this field to have a filter applied for every field group.</p>
<p><strong>NOTE</strong>: If the Target's Design Status is Design Finished, Complete or Inactive, this icon is disabled.</p>
<p>This icon is disabled if the selected field is a zLegacy field.</p></td>
</tr>
<tr class="odd">
<td><p>Activate</p></td>
<td><p>Click to activate the selected field(s) for mapping.</p>
<p>When adding a field manually, the field is active by default.</p>
<p>When importing fields via a System Type import, all fields are configured as Inactive unless they are marked for active in the System Type.</p>
<p>Refer to <a href="../Use_Cases/Activate_Fields_for_Map">Activate or Deactivate Target Fields for Mapping</a> for more information.</p>
<p><strong>NOTE</strong>: If the Target's Design Status is Design Finished, Complete or Inactive, this icon is disabled.</p></td>
</tr>
<tr class="even">
<td><p>Deactivate</p></td>
<td><p>Click to deactivate the selected field(s) from mapping.</p>
<p>If a field is a key field and has the KEY FIELD check box enabled on the <span style="font-style: italic;">Target Fields</span> page, the field cannot be deactivated. Uncheck the KEY FIELD check box before deactivating the field.</p>
<p>Refer to <a href="../Use_Cases/Activate_Fields_for_Map">Activate or Deactivate Target Fields for Mapping</a> for more information.</p>
<p><strong>NOTE</strong>: If the Target's Design Status is Design Finished, Complete or Inactive, this icon is disabled.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD GROUP ID</p></td>
<td><p><span>Displays the name of the field group to which the field belongs. All fields are assigned to the default field group (*). Field groups are used to organize data to be able to apply different rules, criticality levels, requirements settings against each group depending on the values of data in a related field..</span></p>
<p>Refer to <a href="../Use_Cases/Work_with_Field_Groups">Work with Field Groups</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>METRIC GROUP ID</p></td>
<td><p>Displays the name of the metric group to which the field is assigned. Metric groups are a subset of field groups. Metric groups are delineated into logical sets of fields that relate to a screen within the Target system. For SAP-related objects, the metric groups can represent the tabs within an SAP screen or TCode (for example, Customer Basic, Sales, Company and Accounting).</p>
<p>Refer to <a href="../Use_Cases/Work_with_Metric_Groups">Work with Metric Groups</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>FIELD ORDER</p></td>
<td><p>Displays the order of the field entered on the <span style="font-style: italic;">Target Fields</span> page.</p>
<p>The order is used to sort the <span style="font-style: italic;"><a href="../../Map/Page_Desc/Field_Mappings_H">Field Mappings</a></span> page in Map. Key and required fields are given a lower number (as in, a higher priority) than optional fields.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If checked, the field is active and can be used for mapping. If unchecked, the field cannot be used in mapping, and will not be pushed to Map when the Target design is synced.</p>
<p>When adding a field manually, the field is active by default.</p>
<p>When importing fields via a System Type import, all fields are configured as Inactive unless they are marked for active in the System Type.</p></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the field name.</p>
<p>This field cannot be edited for zLegacy fields.</p></td>
</tr>
<tr class="even">
<td><p>DISPLAY NAME</p></td>
<td><p>Displays a description of the field that is provided by the ERP system.</p></td>
</tr>
<tr class="odd">
<td><p>USAGE</p></td>
<td><p>Displays how the field is used. Values are:</p>
<ul>
<li><span style="font-weight: bold;">Natural</span> – The field exists in the Target system. The system adds a “z” to the front of the field name used in the Source table.</li>
<li><span style="font-weight: bold;">Utility</span> – The field does not exist in the Target system, but can be used to register rules and reports to in Transform. Fields of this type should be captured in Target Design.  The user can choose whether this field should be mapped by using the Visibility field on the <span style="font-style: italic;">Vertical</span> view.  A utility field is added to the Target table to be used by the AutoGen process.  Utility fields will be appended to BOTH the Target and Source table as is. No “z” field will be appended.</li>
</ul>
<p><strong>NOTE</strong>: A visibility can be set so that Utility fields can be mapped. Refer to <a href="../Use_Cases/Set_Field_Visibility_for_Mapping">Set Field Visibility for Mapping</a>  for more information.</p>
<p><strong>NOTE</strong>: By default, the visibility of a Utility field is set to NONE, except for zLegacy keys. zLegacy key fields will default to Source visibility. Refer to <a href="../Use_Cases/Allow_Mapping_of_Utility_Columns">Allow Mapping of Utility Columns</a> for more information.</p>
<p><strong>NOTE</strong>: If the field is Natural, the Verify Post Load check box is enabled by default when a user clicks the Activate icon on the Page toolbar.</p></td>
</tr>
<tr class="even">
<td><p>LOOKUP TABLE</p></td>
<td><p>Displays the name of the check table to which a field belongs. Click the link to open the <em><a href="Target_Lookup_Table_H">Target Lookup Table</a></em> page to configure check table values.</p>
<p>Refer to <a href="../Use_Cases/Set_up_Lookup_Tables">Set up Lookup Tables</a> for more information.</p>
<p><strong>NOTE</strong>: This field cannot be edited for zLegacy fields.</p></td>
</tr>
<tr class="odd">
<td><p>CRITICALITY</p></td>
<td><p>Displays the Criticality level, which is used for reporting purposes. The platform is delivered with the values High, Medium, and Low. These values cannot be edited or deleted.</p>
<p>Custom criticality levels can be added, edited, and deleted.</p>
<p>Refer to <a href="../Config/Add_Custom_Criticality_Levels">Add Custom Criticality Levels</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>REQUIRED</p></td>
<td><p>Displays the Requirement setting used for reporting. The platform is delivered with the following settings that cannot be edited or deleted.</p>
<ul>
<li><strong>Technical Required</strong>—the ERP System cannot run without a value.</li>
<li><strong>Business Required</strong>—the Business requires this field to have a value.</li>
<li><strong>Conditional Required</strong>—based upon other field settings this field may or may not be required.</li>
<li><strong>Optional</strong>—this view is not required by ERP system or Business users.</li>
</ul>
<p>This value displays on the Target Fields page (Design &gt; Targets &gt; Fields) in the REQUIRED list box.</p></td>
</tr>
<tr class="odd">
<td><p>KEY FIELD</p></td>
<td><p>If checked, the field is a key field on the table. If a field is a key field, the REQUIRED field is set to Technical Required, ACTIVE check box is enabled, and the CRITICALITY is set to High.</p>
<p>Key fields are created during field mapping. Key(s) on the Target table are created by using the key(s) from the Target system and the zLegacy field. For example, the MATNR field identified as the key field in Target Design is used to create the key field zLegacyMATNR on the Target table.</p>
<p><strong>NOTE</strong>: This field cannot be edited for zLegacy fields.</p>
<p>The key field is added to the Target table when the table is created during SQL AutoGen.</p></td>
</tr>
<tr class="even">
<td><p>VERIFY POST LOAD</p></td>
<td><p>If checked, the data should be verified after it is loaded into the Target system. This option is used with Natural fields only.</p>
<p><strong>NOTE</strong>: The check box is automatically enabled for:</p>
<ul>
<li>A Natural field marked as a Key field on import</li>
<li>A Natural field that is updated to have the KEY FIELD check box enabled</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Basic Rules</p></td>
<td><p>Click to open the <a href="Rules_Basic_Rule_H"><em>Rules: Basic Rules</em></a> page to add basic rules, logic conditions to apply to the data in the field. Basic rules are automatically generated and include binding criteria. Multiple basic rules can be added and are combined with AND.</p>
<p>This icon is disabled if the Target’s Design Status is Design Finished, Complete or Inactive.</p>
<p>Refer to <a href="../Use_Cases/Basic_Rules">Add a Basic Rule</a> for more information.</p>
<p>If the field is a zLegacy field, Basic rules cannot be configured.</p></td>
</tr>
<tr class="even">
<td><p>Complex Rules</p></td>
<td><p>Click to open the <a href="Rules_Field_Complex_Rules"><em>Rules: Field Complex Rules</em></a> page to add the documentation for a complex rule. Complex rules are not automatically generated.</p>
<p>Complex rules provide information that the Data Services developer uses when writing the rule. When an AutoGen request is processed, a placeholder where complex rules can be developed is created.</p>
<p>This icon is disabled if the Target’s design status is Design Finished, Complete or Inactive.</p>
<p>Refer to <a href="../Use_Cases/Complex_Rules">Add a Complex Rule</a>  for more information.</p>
<p><strong>NOTE</strong>: If the field is a zLegacy field, Complex rules cannot be configured.</p></td>
</tr>
</tbody>
</table>

## <span id="Target_Fields_V"></span>Target Fields V

[Target Fields H](Target_Fields_H_Target_Design)

<div class="use">

Use this page to

  - [Add Fields to a Target](../Use_Cases/Add_Fields_to_a_Target)
  - [Activate or Deactivate Target Fields for
    Mapping](../Use_Cases/Activate_Fields_for_Map)
  - [Extend Fields to Field
    Groups](../Use_Cases/Extend_a_Field_to_a_Field_Group)
  - [Set Visibility for Mapping of Target and Source
    Fields](../Use_Cases/Set_Field_Visibility_for_Mapping)

</div>

This page has the following tabs:

  - [General](#General_Tab)
  - [Additional Information](#Advanced_Information_Tab)

### <span id="General_Tab"></span>General tab

Field

Description

Basic

Name

Displays the field name.

**NOTE**: This field cannot be edited for zLegacy fields.

Description

Displays a brief description of the field that was either provided on
import or entered manually.

Usage

Displays how the field is used. Values are:

  - <span style="font-weight: bold;">Natural</span> – The field exists
    in the Target system. The system adds a “z” to the front of the
    field name used in the Source table.
  - <span style="font-weight: bold;">Utility</span> – The field does not
    exist in the Target system, but can be used to register rules and
    reports to in Transform. Fields of this type should be captured in
    Target Design.  The user can choose whether this field should be
    mapped by using the Visibility field on the
    V<span style="font-style: italic;">ertical</span> view.  A utility
    field is added to the Target table to be used by the AutoGen
    process.  Utility fields will be appended to BOTH the Target and
    Source table as is.  No “z” field will be appended.

**NOTE**: A visibility can be set so that Utility fields can be mapped.
Refer to [Set Visibility for Mapping of Target and Source
Fields](../Use_Cases/Set_Field_Visibility_for_Mapping)  for more
information.

**NOTE**: By default, the visibility of a Utility field is set to NONE,
with the exception of zLegacy keys. zLegacy key fields will default to
Source visibility.  Refer to [Set Visibility for Appended Utility
Columns](../Use_Cases/Allow_Mapping_of_Utility_Columns) for more
information.

**NOTE**: If the field is Natural, the Verify Post Load check box is
checked by default when a user clicks the Activate icon on the Page
toolbar.

Criticality

Displays the Criticality level, which is used for reporting purposes.
The platform is delivered with the values High, Medium, and Low. These
values cannot be edited or deleted.

Custom criticality levels can be added, edited, and deleted.

Refer to [Add Custom Criticality
Levels](../Config/Add_Custom_Criticality_Levels) for more
information.

Required

Displays the field’s requirement status.

Values are:

  - **Business Required**—Required to meet a business rule or otherwise
    meet a business need.
  - **Technical Required**—Required by the system
  - **Conditional**—Required depending on certain conditions
  - **Optional**—Not required.

Application Screen

Displays the name of the screen in the ERP system that contains the
field. The value “Not Specified” indicates that the name of the
application screen has not been entered.

**NOTE:** If using Target Design with Full Construction and the option
to generate a *Vertical* View is selected in the Construct AutoGen Build
View field on the *[Target
Sources](Target_Sources_H_Design#Target_Sources_V)* page’s
*Vertical* View, this field is used to as the tab name on the *Vertical*
View.

Refer to [Use Target Design with Full
Construction](../../Construct/Use_Cases/Use_Target_Design_with_Full_Construction)
for more information.

Display Name

Displays the label of the field as it appears on the screens in the ERP
system.

Metric Group ID

Displays the name of the metric group to which the field is assigned.
Metric groups are a subset of field groups. Metric groups are delineated
into logical sets of fields that relate to a screen within the Target
system. For SAP-related objects, the metric groups can represent the
tabs within an SAP screen or TCode (for example, Customer Basic, Sales,
Company and Accounting).

Refer to [Work with Metric
Groups](../Use_Cases/Work_with_Metric_Groups) for more information.

Field Oder

Displays the order the field displays on the screen in the ERP system.

**NOTE:** If using Target Design with Full Construction and the option
to generate a *Vertical* View is selected in the Construct AutoGen Build
View field on the [Target
Sources](Target_Sources_H_Design#Target_Sources_V) page’s *Vertical*
View, this field is used to determine the order of the fields on the
*Vertical* View.

Refer to [Use Target Design with Full
Construction](../../Construct/Use_Cases/Use_Target_Design_with_Full_Construction)
for more information.

Active

If checked, the field is active and can be used for mapping. If
unchecked, the field cannot be used in mapping, and will not be pushed
to Map when the Target design is synced.

When adding a field manually, the field is active by default.

When importing fields via a System Type import, all fields are
configured as Inactive unless they are marked for active in the System
Type.

Key Field

If checked, the field is a key field on the table. If a field is a key
field, the REQUIRED field is set to Technical Required, the ACTIVE check
box is enabled, and the CRITICALITY is set to High.

Key fields are created during field mapping. Key(s) on the Target table
are created by using the key(s) from the Target system and the zLegacy
field. For example, the MATNR field identified as the key field in
Target Design is used to create the key field zLegacyMATNR on the Target
table.  

**NOTE**: This field cannot be edited for zLegacy fields.

The key field is added to the Target table when the table is created
during SQL AutoGen.

**NOTE:** If using Target Design with Full Construction and the option
to generate a *Vertical* View is selected in the Construct Auto Gen
Build View field on the *[Target
Sources](Target_Sources_H_Design#Target_Sources_V)* page’s
*Vertical* View, this field determines the key fields on the *Vertical*
view.

Refer to [Use Target Design with Full
Construction](../../Construct/Use_Cases/Use_Target_Design_with_Full_Construction)
for more information.

Verify Post Load

If checked, the data should be verified after is loaded into the Target
system. This option is used with Natural fields only.

The check box is automatically enabled for:

  - A Natural field marked as a Key field on import
  - A Natural field that is updated to have the KEY FIELD check box
    enabled

Derived from Source

If checked, the field is included in the insert rule built by SQL
AutoGen that copies the field from the Source to the Target. This field
is enabled by default for Utility fields added during the sync process.

If unchecked, during the sync process, this field is added to the Target
and Source tables but is not included in the insert rule. For example,
the zDuplicate field may need to be added to the Source or Target table,
but not included in the insert rule.

**NOTE**: This check box displays for Utility fields only.

If checked, the data came from the Source. If unchecked, it did not come
from the Source.

**NOTE**: It is checked by default.

**NOTE**: This field is for documentation purposes only.

Visibility

Displays how the field is used in mapping and whether it displays on the
<span style="font-style: italic;">[Field
Mappings](../../Map/Page_Desc/Field_Mappings_H)</span> page in Map.

Values are:

  - **Both**—Mapping for Source and Target
  - **None**—No mapping required for the field
  - **Source**—Source only mapping
  - **Target**—Target only mapping

**NOTE**: If the field is Natural, the visibility is set to Both –
Mapping for Source and Target by default. If the field is a key  zLegacy
field, the visibility is set to Source – Source only mapping by default.
If the zLegacy field is not a key field, the visibility is set to None
by default.

**NOTE**: Visibility can only be set if the field’s Target is in a
Design Status of In Design.

Details

Lookup Table

Displays the name of the check table to which a field belongs. Click the
link to open the *[Target Lookup Table](Target_Lookup_Table_H)* page
to configure check table values.

Refer to [Set up Lookup Tables](../Use_Cases/Set_up_Lookup_Tables)
for more information.

**NOTE**: This field cannot be edited for zLegacy fields.

Data Type

Displays the field’s data type, such as NVARCHAR or DECIMAL

**NOTE**: The data type of a field determines whether the Length and
Decimal fields on this page are required. When the following data types
are selected, the Length field is required:

  - NVARCHAR
  - DECIMAL
  - NCHAR
  - NVARCHAR

When the field’s data type is DECIMAL or DATETIME, the Decimal field is
required.

Length

Displays the field length, or the maximum allowable characters/numbers
that the field can store. This field is required when the field’s data
type is:

  - NVARCHAR
  - DECIMAL
  - NCHAR
  - NVARCHAR

Decimals

Displays the decimal places allowed in the field.

When the DECIMAL or DATETIME data types are selected, the Decimal field
is required.

Field Format

Displays the format of the field used to validate the data in this field
during Data Services AutoGen. Values are Date, Time and Decimal.

The Field Format works in conjunction with the Date Format, Time Format,
and Decimal Format fields on the
[<span style="font-style: italic;">Targets</span>](Targets_H_Design)
page's <span style="font-style: italic;">Vertical</span> View, where the
actual format for data fields is stored.

For example, the Date Format for a Target is set at YYYYDDMM.

A user selects Date in the Field Format list box for the field Received
By Date.

The data in the Received By Date field passes through the migration
process with a data type of NVARCHAR. When validation rules are written
for this field in Data Services AutoGen, the format of the Received By
Date field is set as YYYYDDMM so that it can be loaded into the Target
with no errors.  Refer to [Set the Date, Time, and Decimal
Formats](../Use_Cases/Set_Date_Time_and_Decimal_Format) for more
information.

<div style="mso-element: comment-list;">

-----

</div>

 

### <span id="Advanced_Information_Tab"></span>Additional Information tab

Field

Description

Help and Documentation

Help Text

Displays help text imported from the ERP system.

Comment

Displays a user-entered comment about the Target field.

This field is for documentation purposes only.

Instructions

Displays instructions about how to use the field in mapping or other
functions.

This field is for documentation purposes only.

Documentation

Click Upload a file to upload documentation related to the Target field.
If documentation has been uploaded, the Download a File icon is active,
and the file can be downloaded. The Download a File icon is disabled if
no documentation has been uploaded for the Target field.

Basic Rules

Click to open the [*Rules: Basic Rules*](Rules_Basic_Rule_H) page to
add basic rules, logic conditions to apply to the data in the field.
Basic rules are autogenerated during Data Services AutoGen and include
binding criteria, Multiple basic rules can be added and are combined
with AND.

This icon is disabled if the Target’s Design Status is Design Finished,
Complete or Inactive.

**NOTE**: If the field is a zLegacy field, Basic rules cannot be
configured.

Complex Rules

Click to open the [*Rules: Field Complex
Rules*](Rules_Field_Complex_Rules) page to add the documentation for
a complex rule. Complex rules are not generated.

**NOTE**: Complex Rules are for documentation purposes only to describe
what the Data Services developer needs to do. A placeholder will be
created when an AutoGen request is processed. This is where complex
rules can be developed.

This icon is disabled if the Target’s Design Status is Design Finished,
Complete or Inactive.

**NOTE**: If the field is a zLegacy field, Complex rules cannot be
configured.
