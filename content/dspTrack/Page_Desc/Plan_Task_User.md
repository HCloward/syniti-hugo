# Plan Task User

<div class="use">

Use this page to [Add Users to Plan
Tasks.](../Use_Cases/Add_Users_to_Plan_Tasks_Manually.htm)

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Track \>
    </span>**Project** in the Navigation pane.
2.  Click **Plans** for a project.
3.  Click **Tasks** for a plan.
4.  Click **Users** for a task.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>USER ID</p></td>
<td><p>Displays the name of a user assigned to the task.</p></td>
</tr>
<tr class="odd">
<td><p>PRIMARY CONTACT</p></td>
<td><p>If enabled, the user is the primary contact for the task.</p>
<p><strong>NOTE</strong>: Only one user can be assigned as a primary contact per task.</p>
<p>Use this setting for reporting purposes or to indicate the single source of contact for the task.</p></td>
</tr>
<tr class="even">
<td><p>PINNED</p></td>
<td><p>If enabled, the user is pinned to the task.</p>
<p><strong>NOTE</strong>: If the <strong>PINNED</strong> check box is enabled for a user, and the user is added to a task using a Security tag, that user will not be removed from the task if the Security tag is removed from the task.</p>
<p>Users can be assigned to tasks in two ways. Multiple users can be assigned to a task using a Security tag (Configuration &gt; Tag Type &gt; Security &gt; Registrations &gt; Users), or individual users can be added using the <em>Plan Task User</em> page (Project &gt; Plans &gt; Tasks &gt; Users).</p>
<p>Users assigned to a task using a Security tag can only be added or removed from the task via the <em>SecurityTagUser</em> page, but if the PINNED setting is enabled for a user, that user will not be removed from a task, even if the Security tag is removed from a task.</p>
<p><strong>NOTE</strong>: The PINNED setting is enabled by default for users added to a task directly on the <em>Plan Task User</em> page. However, if a user is added to a task using a Security tag, the PINNED check box is not enabled by default for the user and must be manually enabled on the <em>Plan Task User</em> page.</p>
<p>Refer to <span><a href="../Use_Cases/Use_Tags.htm">Use Tags</a></span> and <span><a href="../Use_Cases/Configure_Security_Tags.htm">Configure Security Tags</a></span> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>TAGS</p></td>
<td><p>Displays the tag assigned to the user if the user was assigned to the task using a Security tag.</p>
<p>Refer to <a href="../Use_Cases/Configure_Security_Tags.htm">Configure Security Tags</a> for more information.</p></td>
</tr>
</tbody>
</table>
