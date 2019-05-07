+++
title = 'Page Validation Rules H'
solution = 'Platform'
+++

# Page Validation Rules H

[Page Validation Rules V](#Page_Validation_Rules_V)

<div class="use">

Use this page to [Register a Validation Rule to a
Page](../../WebApp_Dev/ValidationRules.htm).

</div>

To access this page:

1.  Select **Admin \> WebApps** in the *Navigation* pane.
2.  Click the **Pages** icon for a **WEB APP NAME**.
3.  Click the **Events** icon for a page.
4.  Click the **Validation Rules** icon for an event.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SQL</p></td>
<td><p>This icon is not used.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays order in which the validations are executed.</p></td>
</tr>
<tr class="even">
<td><p>VALIDATION TYPE</p></td>
<td><p>Displays the type of validation for the selected page.</p>
<p>Options are:</p>
<ul>
<li><p><strong>External Page –</strong> Validation plugins can be created internally right now, but points to code that will execute against the record and return validation results if they exist.</p></li>
<li><p><strong>Stored Procedure –</strong> This setting executes a procedure to determine whether the associated record is valid. Returning a non-zero result will result in failing the validation.</p></li>
<li><p><strong>View –</strong> This setting binds the view against the current column key to determine validity. If the view returns any results, the validation rule is considered failed.</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p>NAME</p></td>
<td><p>Displays the name of the name of the validation which is computed based on the type of the validation and the entity chosen (whether it’s a view, procedure, or plugin), for example, webdcsMARA_FullConstruct_DSP9587DupKeyVal.</p></td>
</tr>
<tr class="even">
<td><p>SEVERITY</p></td>
<td><p>Displays the severity level for the validation type for the selected page.</p>
<p>Options are:</p>
<ul>
<li><p><strong>Error –</strong> If the record fails this validation, the status will be marked as invalid. Business rules not marked to “Run on Fail” will not run. If this is a row level validation, an inline red bordered text box will appear with the validations text.</p></li>
<li><p><strong>Message –</strong> This severity is an informative validation rule which works the same as other validation types but will not negatively affect (for example, failing a message will not fail the record validation) the validity of the record itself. This will show in the UI with a blue border.</p></li>
<li><p><strong>Warning –</strong> If the record fails this type of validation they will be prompted to click Yes or No on whether to pass or fail the record. If passed, all business rules set to “Run on Pass” will run. If not, only the ones set to “Run on fail” will run and the record will be marked accordingly. This type of validation will show with a yellow border.</p></li>
<li><p><strong>Workflow Only –</strong> Deprecated.</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p>COMMENT</p></td>
<td><p>Displays the text when records fail this validation.</p></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If checked, the Validation rule is executed. If not checked, the Validation rule is not executed.</p></td>
</tr>
</tbody>
</table>

## <span id="Page_Validation_Rules_V"></span>Page Validation Rules V

[Page Validation Rules H](#Page_Validation_Rules_H)

<div class="use">

Use this page to [Register a Validation Rule to a
Page](../../WebApp_Dev/ValidationRules.htm).

</div>

Field

Description

Validation Rule Properties

PRIORITY

Displays order in which the validations are executed.

View

Displays the name of the SQL view associated with the validation.

Active

If checked, the Validation rule executes.

If not checked, the Validation rule does not execute.

Severity

Displays the severity level for the validation type for the selected
page.

Options are:

  - **Error –** If the record fails this validation, the status will be
    marked as invalid. Business rules not marked to “Run on Fail” will
    not run. If this is a row level validation, an inline red bordered
    text box will appear with the validations text.

  - **Message –** This severity is an informative validation rule which
    works the same as other validation types but will not negatively
    affect (for example, failing a message will not fail the record
    validation) the validity of the record itself. This will show in the
    UI with a blue border.

  - **Warning –** If the record fails this type of validation they will
    be prompted to click Yes or No on whether to pass or fail the
    record. If passed, all business rules set to “Run on Pass” will run.
    If not, only the ones set to “Run on fail” will run and the record
    will be marked accordingly. This type of validation will show with a
    yellow border.

  - **Workflow Only –** Deprecated.

COMMENT

Displays the text that displays when records fail this validation.

Advanced

Conditional Column

Displays the column name in the view that allows for a 0 (disabled) or 1
(enabled) value to determine whether this Validation rule executes. This
can be useful when, for example, ensuring a field has a non-NULL value
when another column is enabled.

Duplicate Detection View

Displays the name of the view that is used for the validation view used
to select the duplicates in the Duplicate Detection process. This view
allows the developer to customize the columns displayed and reduce the
rows returned.

When the duplicate detection is run as part of validation and a possible
duplicate is returned, the user can click the in-line validation message
to view the possible duplicates.

If this field is blank, the underlying table is used for the validation
view, and all columns in the table are searched for duplicate. In this
case, the result set is larger. The primary key and duplicate detection
columns are included in the result.

Refer to [Manage Duplicate
Detection](../Use_Cases/Manage%20Duplicate%20Detection.htm) for more
information.
