+++
title = 'Task Page H'
solution = 'Data Quality'
+++

# Task Page H

[Task Page V](Task_Page_H.htm#Task_Page_V)

<div class="use">

Use this page to [View all Pages for a
Task](../Use_Cases/View_all_Pages_for_a_Task.htm).

</div>

To access this page

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    category.
3.  Click the <span style="font-weight: bold;">Pages</span> icon for a
    task.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Update Page List</p></td>
<td><p>Click to update the list of child pages assigned to the selected page and to update all the scenario role tasks to which that task is assigned.</p>
<p>A Designer uses this feature if new Content WebApp pages are added.</p>
<p>Refer to <a href="../Use_Cases/Update_the_List_of_Pages_Assigned_to_a_Task.htm">Update the List of Pages Assigned to a Task</a> for more information.</p>
<p><strong>NOTE</strong>: This icon is disabled if multiple tasks are selected. The page list can be updated for one task at a time.</p></td>
</tr>
<tr class="odd">
<td><p>PAGE ID</p></td>
<td><p>Displays the name of the WebApp and the page within that WebApp that is used by the task selected on the <span style="font-style: italic;"><a href="Task_H.htm">Task</a></span> page. Task pages can be dspConduct™ pages or pages developed in the Content WebApp.</p></td>
</tr>
<tr class="even">
<td><p>PAGE TYPE</p></td>
<td><p>Displays the type of page. DCVs and PCVs can only be built for pages with a page type of Dynamic.</p></td>
</tr>
<tr class="odd">
<td><p>PAGE LEVEL</p></td>
<td><p>Displays the level of the page for the selected task. For example, a header page, which can be linked to directly from another page, icon, or through another means, has a page level of 0. A detail page, with a level of 1, 2 and so on, is accessed from a header page and is not directly linked to from any other page.</p></td>
</tr>
<tr class="even">
<td><p>PARENT PAGE ID</p></td>
<td><p>Displays the name of the page that allows a user to access the selected page.</p>
<p>If the page is a header page that is not accessed from another page, the field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>LINK COLUMN</p></td>
<td><p>Displays the name of the column on the parent page that allows access to the page.</p>
<p>If the page is a header page that is not accessed from another page, the field is blank.</p></td>
</tr>
</tbody>
</table>

## <span id="Task_Page_V"></span>Task Page V

[Task Page H](Task_Page_H.htm)

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Update Page List</p></td>
<td><p>Click to update the list of child pages assigned to the selected page and to update all the scenario role tasks to which that task is assigned.</p>
<p>A Designer uses this feature if new Content WebApp pages are added.</p>
<p>Refer to <a href="../Use_Cases/Update_the_List_of_Pages_Assigned_to_a_Task.htm">Update the List of Pages Assigned to a Task</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Page ID</p></td>
<td><p>Displays the name of the WebApp and the page within that WebApp that is used by the task selected on the <span style="font-style: italic;"><a href="Task_H.htm">Task</a></span> page. Task pages can be dspConduct™ pages or pages developed in the Content WebApp.</p></td>
</tr>
<tr class="even">
<td><p>Parent Page ID</p></td>
<td><p>Displays the name of the page that allows a user to access the selected page.</p></td>
</tr>
<tr class="odd">
<td><p>Page Level</p></td>
<td><p>Displays the level of the page for the selected task. For example, a header page, which can be linked to directly from another page, icon, or through another means, has a page level of 0. A detail page, with a level of 1, 2 and so on, is accessed from a header page and is not directly linked to from any other page.</p></td>
</tr>
<tr class="even">
<td><p>Link Column</p></td>
<td><p>Displays the name of the column on the parent page that allows a user to access the selected page.</p>
<p>If the page is a header page that is not accessed from another page, the field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>Page Type</p></td>
<td><p>Displays the type of page, such as Header/Detail or Dynamic.</p>
<p>A page type, along with other factors, determines how a page is used. For example,  a Header/Detail page sets a split panel layout. Detail records display for a selected header record.</p></td>
</tr>
<tr class="even">
<td><p>Control Table Prefix</p></td>
<td><p>Displays the prefix in the table name when a table is generated for a scenario &gt; role &gt; task combination that uses this page.</p>
<p>When a table is generated, it follows the naming convention [Control table prefix]_[Page View’s Root Name]_[variant column name or required].</p>
<p>For example, a content page named “Address” has a Horizontal View webRequestAddressHor. The control tables prefix configured for this Category is &quot;ttSRTC_&quot;. The task has an active variant configured for the “Country” field. On this page, for “Address”, the Control Table Prefix is “ttSRTC_RequestAddress_”. When created, the Control View table name is ttSRTC_RequestAddress_Country.</p>
<p>Refer to <a href="../Use_Cases/Create_Tables_and_Views_for_Content_WebApp_Pages_Overview.htm">Create Tables and Views for Content WebApp Pages</a> and <a href="../Use_Cases/Activate_Configure_Column_Variants.htm">Activate and Configure Column Variants</a> for more information.</p></td>
</tr>
</tbody>
</table>
