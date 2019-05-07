+++
title = 'Scenario Role Task Column H'
solution = 'Data Quality'
+++

# Scenario Role Task Column H

[Scenario Role Task Column V](#ScenarioRoleTaskColumn)

<div class="use">

Use this page to:

  - [Activate and Configure Column
    Variants](../Use_Cases/Activate_Configure_Column_Variants.htm)
  - [Update a Scenario Role Task Column
    List](../Use_Cases/Update_a_Scenario_Role_Task_Column_List.htm)
  - [Copy Settings to Other
    Variants](../Use_Cases/Copy_Settings_to_Other_Variants.htm)
  - [Configure Column Status for a Task for a Scenario Role
    Combination](../Use_Cases/Configure_Column_Status_for_a_Scenario_Role_Task.htm)
  - [Configure the Required Setting for a Scenario Role Task
    Column](../Use_Cases/Configure_Required_Setting_Scenario_Role_Task_Column.htm)
  - [Create Validation Views for a Content WebApp Task
    Page](../Use_Cases/Create_ValidationViews_Content_Page.htm)

</div>

To access this page:

1.  Select <span style="font-weight: bold;">dspConduct
    \></span>**Design** in the *Navigation* pane.
2.  Click the **Scenarios** icon.
3.  Click the **Roles** icon.
4.  Click the **Tasks** icon on the *Scenario (Roles)* page.
5.  Click the <span style="font-weight: bold;">Columns</span> icon.

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Update Column List</p></td>
<td><p>Click to refresh the column settings with the settings in the Content WebApp.</p>
<p>If columns are added to or removed from the content page, the column list must be refreshed to capture the column additions or subtractions,</p>
<p><strong>NOTE:</strong> This option only adds and removes column settings. Existing settings are not changed. Refer to <a href="../Use_Cases/Update_Control_Table_Data.htm">Update Control Table Data</a> for more information.</p>
<p><strong>NOTE:</strong> When the update adds a column for which there is no column property on the page, the columns status and required settings default to hidden and not required respectively. The Designer must configure the settings. </p></td>
</tr>
<tr class="odd">
<td><p>Create Required Column Validations For All Columns</p></td>
<td><p>Click to create required column validation views for all pages in this task.</p>
<p>Refer to <a href="../Use_Cases/Create_Valid_Views_Task_Pages.htm">Create Validation Views for Content WebApp Task Pages</a> for more information.</p>
<p>To create validation views for a single page in a task, refer to <a href="../Use_Cases/Create_ValidationViews_Content_Page.htm">Create Validation Views for a Content WebApp Task Page</a>.</p></td>
</tr>
<tr class="even">
<td><p>Enable Selected Columns</p></td>
<td><p>Click to update the default control status value to disabled for one or more selected columns.</p></td>
</tr>
<tr class="odd">
<td><p>Disable Selected Columns</p></td>
<td><p>Click to update the default control status value to disabled for one or more selected columns.</p></td>
</tr>
<tr class="even">
<td><p>Hide Selected Columns</p></td>
<td><p>Click to update the default control status value to hide for one or more selected columns.</p></td>
</tr>
<tr class="odd">
<td><p>Require Selected Columns</p></td>
<td><p>Click to enable the required check box for one or more selected columns.</p></td>
</tr>
<tr class="even">
<td><p>Not Require Selected Columns</p></td>
<td><p>Click to disable the required check box for one or more selected columns.</p></td>
</tr>
<tr class="odd">
<td><p>Copy Setting to Other Variants</p></td>
<td><p>Click to copy a change to the control status or required setting for one variant condition to copy to all of the other variants conditions for the column.</p></td>
</tr>
<tr class="even">
<td><p>VARIANT</p></td>
<td><p>Displays the variant that this column setting is a part of.</p></td>
</tr>
<tr class="odd">
<td><p>COLUMN PAGE ID</p></td>
<td><p>Displays the ID of the page on which the column displays.</p>
<p><strong>NOTE:</strong> A variant is only applied to the parent page columns, not child level page columns associated with the parent page.</p></td>
</tr>
<tr class="even">
<td><p>COLUMN</p></td>
<td><p>Displays the column business name.</p></td>
</tr>
<tr class="odd">
<td><p>COLUMN DISPLAY NAME</p></td>
<td><p>Displays the translated column name if the column has a translation in the SAP Catalog or any user-defined catalogs for the page.</p></td>
</tr>
<tr class="even">
<td><p>CONTROL STATUS</p></td>
<td><p>Displays the control status setting of the column on a task page for the scenario &gt; role &gt; task combination.</p>
<p>Values are:</p>
<ul>
<li><strong>Disabled</strong> – Column displays but is not editable.</li>
<li><strong>Enabled</strong> – Column displays and is editable.</li>
<li><strong>Hide</strong> – Column does not display.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>REQUIRED</p></td>
<td><p>If enabled, indicates that this is defined as a required column within the scenario &gt; role &gt; task combination. If disabled, indicates that this is not defined as a required column within the scenario &gt; role &gt; task combination.</p></td>
</tr>
</tbody>
</table>

## <span id="ScenarioRoleTaskColumn"></span>Scenario Role Task Column V

[Scenario Role Task Column H](#)

<table>
<colgroup>
<col style="width: 50%" />
<col style="width: 50%" />
</colgroup>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Update Column List</p></td>
<td><p>Click to refresh the column settings with the settings in the Content WebApp.</p>
<p><strong>NOTE:</strong> This option only adds and removes column settings. Existing settings are not changed.</p></td>
</tr>
<tr class="odd">
<td><p>Create Required Column Validations For All Columns</p></td>
<td><p>Click to create required column validation views for all pages in this task.</p>
<p>Refer to <a href="../Use_Cases/Create_Valid_Views_Task_Pages.htm">Create Validation Views for Content WebApp Task Pages</a> for more information.</p>
<p>To create validation views for a single page in a task, refer to <a href="../Use_Cases/Create_ValidationViews_Content_Page.htm">Create Validation Views for a Content WebApp Task Page</a>.</p></td>
</tr>
<tr class="even">
<td><p>Column Page ID</p></td>
<td><p>Displays the ID of the page on which the column displays.</p></td>
</tr>
<tr class="odd">
<td><p>Page Level</p></td>
<td><p>Displays the order of  the columns in the Scenario Role Task Column <span style="font-style: italic;">Horizontal</span> View for views with parent and child pages. A 0 indicates parent page column, 1, 2, etc. indicates child level page columns.</p>
<p><strong>NOTE:</strong> A variant is only applied to the parent page columns, not child level page columns associated with the parent page.</p></td>
</tr>
<tr class="even">
<td><p>Column</p></td>
<td><p>Displays the column business name.</p></td>
</tr>
<tr class="odd">
<td><p>Control Status</p></td>
<td><p>Displays the status setting of the column on the page for the scenario &gt; role &gt; task combination.</p>
<p>Values are:</p>
<ul>
<li><strong>Disabled</strong> – Column displays but is not editable.</li>
<li><strong>Enabled</strong> – Column displays and is editable.</li>
<li><strong>Hide</strong> – Column does not display.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Required</p></td>
<td><p>If enabled, indicates that this is defined as a required column within the scenario &gt; role &gt; task combination. If disabled, indicates that this is not defined as a required column within the scenario &gt; role &gt; task combination.</p></td>
</tr>
<tr class="odd">
<td><p>Required Validation View Created</p></td>
<td><p>If enabled, the validation views for required columns have been generated for this column.</p>
<p>If disabled, the validation views for required columns have not been generated for this column.</p></td>
</tr>
</tbody>
</table>
