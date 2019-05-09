+++
title = 'Schedule Groups'
solution = 'Platform'
+++

# Schedule Groups

<div class="use">

Use this page to [Set up Schedule
Groups](../Config/Set_Up_Schedule_Groups).

</div>

To access this page, select <span style="font-weight: bold;">Collect \>
Administrative \> Schedule Groups</span> in
<span style="font-style: italic;">Navigation</span> pane.

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
<td><p>SCHEDULE GROUP</p></td>
<td><p>Displays unique name of the schedule group.</p>
<p><strong>NOTE:</strong> If building a group with a DBMoto package the following applies: </p>
<ul>
<li>If Schedule Group is set to NO GROUP, both Download and Mirror package will be built as an individual replication in DBMoto. </li>
<li>If Schedule Group is set to AUTO and if it is a Download package, the replication will be part of a group named &lt;GroupPrefix&gt;_Downloads. Otherwise, if it is a Mirror package the replication will be part of a group called &lt;GroupPrefix&gt;_&lt;number&gt; where number is an incremental value to count the number of groups. Groups cannot contain more than &lt;Group_Size&gt; replications. </li>
<li>If Schedule Group is set to &quot;existing group name&quot; with no restriction to the &lt;Group_Size&gt; parameter the replication is built into that group.</li>
</ul>
<p><strong>NOTE:</strong> The Replication Mode must be consistent with the Replication Group Mode (e.g., a download package cannot be grouped with a mirror package). </p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays brief description of the schedule group.</p></td>
</tr>
</tbody>
</table>
