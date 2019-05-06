# Database: Current Requests

<div class="use">

Use the *Database: Current Requests* page to view information about each
database request per session ID that is executing within the SQL server
environment.

</div>

To access this chart in System Administration, select **Admin \>
Resources \> SQL Server Health \> Database: Current Requests** in the
*Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SESSION ID</p></td>
<td><p>Displays the unique identifier for the session.</p></td>
</tr>
<tr class="odd">
<td><p>REQUEST ID</p></td>
<td><p>Displays a unique identifier for the request.</p></td>
</tr>
<tr class="even">
<td><p>START TIME</p></td>
<td><p>Displays the timestamp when the request arrived. This value cannot be NULL.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays the status of the request. This can be one of the following:</p>
<ul>
<li>Background</li>
<li>Running</li>
<li>Runnable</li>
<li>Sleeping</li>
<li>Suspended</li>
</ul>
<p>This value cannot be NULL.</p></td>
</tr>
<tr class="even">
<td><p>COMMAND</p></td>
<td><p>Displays the current type of command that is being processed. Common command types include the following:</p>
<ul>
<li>SELECT</li>
<li>INSERT</li>
<li>UPDATE</li>
<li>DELETE</li>
<li>BACKUP LOG</li>
<li>BACKUP DATABASE</li>
<li>DBCC</li>
<li>FOR</li>
</ul>
<p>The text of the request can be retrieved by using sys.dm_exec_sql_text with the corresponding sql_handle for the request. Internal system processes set the command based on the type of task they perform. Tasks can include the following:</p>
<ul>
<li>LOCK MONITOR</li>
<li>CHECKPOINTLAZY</li>
<li>WRITER</li>
</ul>
<p>This value cannot be NULL.</p></td>
</tr>
<tr class="odd">
<td><p>WAIT TIME</p></td>
<td><p>Displays the duration in milliseconds of the current wait, if the request is currently blocked. This value cannot be NULL.</p></td>
</tr>
</tbody>
</table>
