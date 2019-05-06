# Plan Access Setup

<div class="use">

Use this page to [Set Plan Security](../Config/Set_Plan_Security.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Track \>
    </span>**Project** in *Navigation* pane.
2.  Click **Plans** for a project.
3.  Click **Vertical View** for a plan.
4.  Click the **Security** tab.
5.  Click **Setup**.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>USER ID</p></td>
<td><p>Displays the name of the user.</p></td>
</tr>
<tr class="odd">
<td><p>WRITE ACCESS</p></td>
<td><p>If enabled, the user can update the <em>Plan</em> page and the <em><span style="font-size: 11.0pt;">Plan Task</span></em> page, and all pages accessed from these pages, for the selected plan.</p></td>
</tr>
<tr class="even">
<td><p>READ ONLY</p></td>
<td><p>If enabled, the user can view the <em><span style="font-size: 11.0pt;">Plan</span></em> page and the <em><span style="font-size: 11.0pt;">Plan</span><span style="font-size: 11.0pt;">Task</span></em> page, and all pages accessed from these pages, for the selected plan. The user cannot update any pages.</p>
<p><strong>NOTE</strong>: The logged in user cannot set read only access for his or her own account and the READ ONLY check box is not available for the logged in user’s account.</p>
<p>If a user has read only access, that user cannot update any page in the plan, including the <span style="font-size: 11.0pt;font-style: italic;">Plan</span> <em><span style="font-size: 11.0pt;">Access Setup</span></em> page. Therefore, if the logged in user could set read only access for his or her own account, the logged in user could never change access for his or her own account back to Write Access.</p>
<p>For example, user BFranklin is logged in and has access to the Software Implementation plan as a member of the Sample Plan Level Role. BFranklin can change permissions to read only for any user on the <em><span style="font-size: 11.0pt;">Plan Access Setup</span></em> page, and restrict that user’s access to all pages in the Software Implementation plan to read only. However, BFranklin cannot change his own access to read only. It is set to Write Access by default.</p></td>
</tr>
<tr class="odd">
<td><p>IGNORE DURING SYNC PROCESS</p></td>
<td><p>If enabled, the READ ONLY setting for the user ID is ignored when the automatic synchronization procedure runs. The user's read only access is not updated during this procedure, which syncs the settings on the <span style="font-style: italic;">Plan Access Setup</span> page with the Security Role settings for dspTrack™.</p>
<p>Refer to <a href="../Config/Use_Template_Security_Roles.htm">Use Template Security Roles</a> for more information.</p>
<p><strong>NOTE</strong>: If a user is assigned to the Business User role only, this feature is not available, as users assigned to the security role only do not display on this page.</p></td>
</tr>
</tbody>
</table>
