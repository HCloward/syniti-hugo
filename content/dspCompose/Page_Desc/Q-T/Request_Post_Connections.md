# Request Post Connections

<div class="use">

Use this page to view the target system connections for each Integrate
process template associated with the request while [posting request data
to a target
system](../Use_Cases/Post_Request_Data_to_a_Target_ERP_System.htm).

</div>

To access this page:

1.  Select **dspCompose \> Requests** in the *Navigation* pane.
2.  Click **Roles** for a request.
3.  Locate **Post Role ID.**
4.  Click **Request (Post)** for the Post ROLE ID.
5.  Click the **Connections** icon.

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
<td><p>PRIORITY</p></td>
<td><p>Displays the order the templates run.</p></td>
</tr>
<tr class="odd">
<td><p>TEMPLATE NAME</p></td>
<td><p>Displays the name of the process template that is used to post data to the target system identified in the Connection ID field.</p>
<p><strong>NOTE</strong>: The Process Templates for which a connection can be set are based on:</p>
<ul>
<li>The Integrate template type. Refer to <a href="../../../Platform/Integrate/Use_Cases/Create_a_Basic_Template.htm">Create a Basic Template</a> in Integrate for more information.</li>
<li>The &quot;Allowed Connections&quot; configured at the Integrate Process Template level. Refer to <a href="../../../Platform/Integrate/Use_Cases/Set_Connections_at_the_Process_Template_Level.htm">Set Available Connections at the Process Template Level</a> in integrate for more information.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>CONNECTION ID</p></td>
<td><p>Displays the connection ID to the target system where request data is posted.</p></td>
</tr>
<tr class="odd">
<td><p>CREDENTIALS DETECTED</p></td>
<td><p>If enabled, the user name and password have been detected based on the user credentials setting.</p>
<p>If disabled, the credentials have not been detected and must be added for the request to post successfully.</p>
<p>Refer to <a href="../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm">Establish a Connection to a Target System</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>User Credentials</p></td>
<td><p>Click to open the <em><a href="../../../Platform/Common/Page_Desc/User_Credentials_H.htm">User Credentials</a></em> page to add Login credentials for the current user to track that user's updates posted to the target system related to this request.</p></td>
</tr>
</tbody>
</table>
