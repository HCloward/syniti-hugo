+++
title = 'Request Connections'
solution = 'Data Quality'
+++

# Request Connections

<div class="use">

Use this page to set the connection for the Integrate process template
when [creating a request](../Use_Cases/Create_Requests.htm).

</div>

To access this page:

1.  Select **dspCompose \> Requests** in the *Navigation* pane.
2.  Click the **Vertical View** icon.
3.  Click the **Connections** icon.

<table>
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
<td><p>Displays the name of the Integrate process template used to post request data to the target system.</p>
<p><strong>NOTE:</strong> The Process Templates for which a connection can be set are based on:</p>
<ul>
<li>The Integrate template type. Refer to <a href="../../../Platform/Integrate/Use_Cases/Create_a_Basic_Template.htm">Create a Basic Template</a> in Integrate for more information.</li>
<li>The &quot;Allowed Connections&quot; configured at the Integrate Process Template level. Refer to <a href="../../../Platform/Integrate/Use_Cases/Set_Connections_at_the_Process_Template_Level.htm">Set Available Connections at the Process Template Level</a> in integrate for more information.</li>
</ul></td>
</tr>
<tr class="even">
<td><p>CONNECTION ID</p></td>
<td><p>Displays the connection to the target system that was set for the user credentials for this template.</p>
<p>Refer to <a href="../../../Platform/Common/Use_Cases/Establish_a_Connection_to_a_target_system_Overview.htm">Establish a Connection to a Target System</a> for more information.</p>
<p><strong>NOTE:</strong> If a user adds a request based on this template and does not select a connection ID, the default connection assigned to the Integrate Template is used for the request.</p></td>
</tr>
</tbody>
</table>
