+++
title = 'Bulk Execution Panel'
solution = 'Platform'
+++

# Bulk Execution Panel

<div class="use">

Use this page to [Perform Bulk
Execution](../../Bulk_Exec/Perform_Bulk_Execution).

</div>

**NOTE:** The title that displays on the Bulk Execution panel is the
same as the name of the page from which it is launched.

This panel contains the following tabs:

  - [Control Panel](#Control_Panel)

  - [Action on Warning](#Action_on_Warning)

  - [Results](#Results)

### <span id="Control_Panel"></span>Control Panel

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Event</p></td>
<td><p>Displays the page event to be executed. Validate is the only event supported by Bulk Execution.</p></td>
</tr>
<tr class="odd">
<td><p>Exclude Business Rules</p></td>
<td><p>If checked, the OnValidate event runs the validation rules without running any business rules registered to the OnValidate event. If unchecked, both the Validation and Business rules run.</p>
<p><strong>NOTE:</strong> This option cannot be updated if the Exclude Business Rule Option check box is checked for the page event. Refer to <a href="../Use_Cases/Configure_Business_Rule_Settings">Configure Business Rule Settings</a> for more information.</p></td>
</tr>
</tbody>
</table>

### <span id="Action_on_Warning"></span>Action on Warning

Field

Description

Update All

Displays whether all records that fail for validations with a type of
warning for the OnValidate event will automatically pass, fail or
whether no action will be taken during the Bulk Execution process.

Validation Warnings

Displays the warnings that belong to the validation.

 

Pass

Select to indicate that a record that fails the validation should pass
during the Bulk Execution process.

Fail

Select to indicate that a record that fails the validation should fail
during the Bulk Execution process.

No Action

Select to indicate that a record that fails the validation should not be
failed or passed, but will have a validation status of Unknown.

Start

Click to start the Bulk Execution
process.

### <span id="Results"></span>Results

|              |                                                                                                                                                                                                                                     |
| ------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field        | Description                                                                                                                                                                                                                         |
| Expand All   | Click to expand all validation results lists.                                                                                                                                                                                       |
| Collapse All | Click to collapse all validation results lists.                                                                                                                                                                                     |
| Filter       | Click to filter the DSP page on the selected record’s key(s). Filter on multiple records using Ctrl+click.                                                                                                                          |
| Key          | Click to view the primary key of the current record. The key is useful for advanced users who have a working knowledge of the current database and table. The Key's column name and value display at the bottom of the Results tab. |
