# Scenario Role Task Page

<div class="use">

Use this page to:

  - [Generate a Control Table for Content WebApp
    Pages](../Use_Cases/Generate_a_Control_Table_for_Content_WebApp_Pages.htm)
  - [Update Control Table
    Data](../Use_Cases/Update_Control_Table_Data.htm)
  - [Generate Control Views for Content WebApp
    Pages](../Use_Cases/Generate_Control_Views_for_Content_WebApp_Pages.htm)
  - [Create Validation Views for a Content WebApp Task
    Page](../Use_Cases/Create_ValidationViews_Content_Page.htm)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Scenarios</span> icon for
    a category.
3.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    scenario.
4.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    role.
5.  Click the <span style="font-weight: bold;">Pages</span> icon for a
    scenario \> role \> task combination.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Refresh Page List</p></td>
<td><p>Click to refresh the list of pages for the scenario &gt; role &gt; task combination if pages are added or deleted.</p></td>
</tr>
<tr class="odd">
<td><p>Create Control Table</p></td>
<td><p>Click to create a table used to store data to be used as the basis when dspConduct™ builds a Data Control View (DCV) or a Page Control View (PCV) for one or more selected records..</p>
<p>The table is built using the control status information configured on the <a href="Scenario_Role_Task_Column_H.htm#ScenarioRoleTaskColumn">Scenario Role Task Column</a> page for the task.</p></td>
</tr>
<tr class="even">
<td><p>Create Control View</p></td>
<td><p>Click to create a DCV or PVC based on the data in the control table for one or more selected records. If there is a variant assigned to the page, then a DCV should be generated. If not, a PCV will be generated.</p>
<p><strong>NOTE:</strong> These views are not automatically assigned to the page and the WebApp Designer should explicitly decide whether or not they want to use the auto-generated views or create and assign their own.</p></td>
</tr>
<tr class="odd">
<td><p>Update Control Data</p></td>
<td><p>Click to update the table generated for the selected page using the control status information from the <a href="Scenario_Role_Task_Column_H.htm#ScenarioRoleTaskColumn">Scenario Role Task Column</a> page for the task for one or more selected records..</p></td>
</tr>
<tr class="even">
<td><p>Create Validation Views</p></td>
<td><p>Click to create a validation view for each required column on the page for one or more selected records..</p>
<p>Refer to <a href="../Use_Cases/Create_ValidationViews_Content_Page.htm">Create Validation Views for a Content WebApp Task Page</a> for more information.</p>
<p>To create validation views for all pages in a task, refer to <a href="../Use_Cases/Create_Valid_Views_Task_Pages.htm">Create Validation Views for Content WebApp Task Pages</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>PAGE ID</p></td>
<td><p>Displays the name of the WebApp and the page within that WebApp that is used by the task selected on the <span style="font-style: italic;"><a href="Task_H.htm">Task</a></span> page. Task pages can be dspConduct™ pages or pages developed in the Content WebApp.</p></td>
</tr>
<tr class="even">
<td><p>PAGE TYPE</p></td>
<td><p>Displays the type of page. Objects can be built for Dynamic page types only.</p></td>
</tr>
<tr class="odd">
<td><p>CONTROL VIEW TYPE</p></td>
<td><p>Displays the control view type (DCV or PVC) for the selected page.</p>
<p><strong>NOTE</strong>: Layout and static pages do not have a control view type.</p></td>
</tr>
<tr class="even">
<td><p>PARENT PAGE ID</p></td>
<td><p>Displays the name of the page that allows a user to access the selected page.</p></td>
</tr>
<tr class="odd">
<td><p>PAGE LEVEL</p></td>
<td><p>Displays the level of the page for the selected task. For example, a header page, which can be linked to directly from another page, icon, or through another means, has a page level of 0. A detail page, with a level of 1, 2 and so on, is accessed from a header page and is not directly linked to from any other page.</p></td>
</tr>
<tr class="even">
<td><p>LINK COLUMN</p></td>
<td><p>Displays the name of the column on the parent page that allows access to the page.</p>
<p>If the page is a header page that is not accessed from another page, the field is blank.</p></td>
</tr>
</tbody>
</table>
