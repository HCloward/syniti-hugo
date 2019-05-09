+++
title = 'Database: Current Connections'
solution = 'Platform'
+++

# Database: Current Connections

<div class="use">

Use this page to view databases currently connected to the DSP because
of file reads, writes, executing processes or other factors.

</div>

To access this page, select **Admin \> Resources \> SQL Server Health \>
Database: Current Connections** in the *Navigation* pane.

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
<td><p>CLIENT IP</p></td>
<td><p>Displays the IP address of the client connecting to the database.</p></td>
</tr>
<tr class="even">
<td><p>CLIENT PORT</p></td>
<td><p>Displays the port number used by the client for the database connection.</p>
<p><strong>NOTE:</strong> If the client IP is &lt;local machine&gt;, this field is blank.</p></td>
</tr>
<tr class="odd">
<td><p>MINUTES CONNECTED</p></td>
<td><p>Displays the number of minutes since the connection was established.</p></td>
</tr>
<tr class="even">
<td><p>READS</p></td>
<td><p>Displays the number of records read since the latest connection was established.</p></td>
</tr>
<tr class="odd">
<td><p>WRITES</p></td>
<td><p>Displays the number of records written to the database since the latest connection was established.</p></td>
</tr>
</tbody>
</table>
