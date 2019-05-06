# Service Queues

<div class="use">

Use this page to:[Add a service
queue](../Use_Cases/Add%20a%20Service%20Queue.htm) or update service
queue settings.

</div>

To access this page select **Admin \> Configuration \> Service \>
Service Providers \> Queues** from the *Navigation* pane.

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
<td><p>Displays the priority of the queue, which sets the display order on the page.</p></td>
</tr>
<tr class="odd">
<td><p>QUEUE ID</p></td>
<td><p>Displays the queue ID. Values are:</p>
<ul>
<li><strong>Background Events</strong> — Queue for running the standard background processing events</li>
<li><strong>Service Pages</strong> — Queue for executing pages defined as Service Pages on the schedule they are assigned</li>
<li><strong>General</strong> — All foreground events will run by default in the General Queue</li>
<li><strong>Indexing</strong> — The general indexing service page</li>
</ul></td>
</tr>
<tr class="even">
<td><p>MAXIMUM THREADS</p></td>
<td><p>Displays the maximum number of threads for the queue.</p>
<p>The Administrator can specify how many parallel processes can be actioned on the queue at any one time. The user must understand the underlying server architecture to set the number of queues based on the number of processor cores and threads available.</p>
<p><strong>NOTE</strong>: Setting this value too high could potentially block processing on the server by running the memory / processor at too high a value, causing contention.</p></td>
</tr>
</tbody>
</table>
