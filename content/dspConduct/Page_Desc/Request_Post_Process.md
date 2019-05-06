# Request Post Process

<div class="use">

Use this page to [Post a Request](../Use_Cases/Post_a_Request.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspConduct \> Requests</span>
    in the *Navigation* pane.
2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.
3.  Click the <span style="font-weight: bold;">Tasks</span> icon for the
    post role.
4.  Click the name of the task used to post requests.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PRIORITY</p></td>
<td><p>Displays the order the process runs when posting if the request has multiple processes.</p></td>
</tr>
<tr class="odd">
<td><p>INTEGRATE PROCESS ID</p></td>
<td><p>Displays the name of the Integrate process that is used to post the request.</p>
<p>This process is set at the Scenario level. Refer to <a href="../Use_Cases/Add_an_Integrate_Process_to_a_Scenario.htm">Add a Process to a Scenario f</a>or more information.</p></td>
</tr>
<tr class="even">
<td><p>POSTING STATUS</p></td>
<td><p>Displays the name of the posting status set by the system.</p>
<p>Values are Success, Failed and Unposted.</p>
<p><strong>NOTE:</strong> A Designer can configure users to receive workflow notifications when the posting status is updated to Success or Failed. Refer to <a href="../Config/Send_Workflow_Notifications_when_a_Post_Fails_or_Succeeds.htm">Send Workflow Notifications when a Post Fails or Succeeds</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>POSTED BY</p></td>
<td><p>Displays:</p>
<ul>
<li>The user ID of the user who clicked the Group Post icon on this page or</li>
<li>The user ID of the user who clicked Post icon on the <span style="font-style: italic;"><a href="Request_Post_Process.htm">Request Post Process</a></span> page or</li>
<li>&quot;Process&quot; if the Post role is set to Auto Post</li>
</ul>
<p>Refer to <a href="../Use_Cases/Post_a_Request.htm#Auto_Post_a_Request">Auto Post a Request</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>POSTED ON</p></td>
<td><p>Displays the date the request was last posted.</p></td>
</tr>
<tr class="odd">
<td><p>CREDENTIALS DETECTED</p></td>
<td><p>If enabled, credentials have been detected for the connection used by the Integrate process.</p>
<p>If disabled, the Integrate process does not have credentials set.</p>
<p>Credentials must be set for connection to post. Refer to <a href="../../../Data_Quality/dspCompose/Config/Add_Stored_Credentials_as_a_User_on_a_Page_in_Integrate_or_dspCompose.htm">Add Stored Credentials as a User on a Page in Integrate</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Post</p></td>
<td><p>Click to post the data in the request to the target system.</p></td>
</tr>
<tr class="odd">
<td><p>Messages</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Request_Post_Message.htm">Request Post Message</a></span> page to view the messages returned from the target system after posting request data.</p></td>
</tr>
</tbody>
</table>
