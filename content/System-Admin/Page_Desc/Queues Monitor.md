# Queues (Monitor)

<div class="use">

Use this page to:

  - [Start, Stop or Clear
    Queues](../Use_Cases/Start%20Stop%20or%20Clear%20Queues.htm)
  - [Acknowledge Failed Jobs](../Use_Cases/Acknowledge_Failed_Jobs.htm)

</div>

To access this page, select **Admin \> Resources \> Queues** in the
*Navigation* pane.

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
<td><p>SERVICE PROVIDER</p></td>
<td><p>Displays the name of the service that the queue is attached to.</p>
<p>Installations can have multiple services installed to help split the load.</p></td>
</tr>
<tr class="odd">
<td><p>SERVER</p></td>
<td><p>Displays the name of the server that the associated Service Provider is running on.</p></td>
</tr>
<tr class="even">
<td><p>QUEUE</p></td>
<td><p>Displays the type of queue.</p></td>
</tr>
<tr class="odd">
<td><p>ACTIVE</p></td>
<td><p>If enabled, the queue is active (i.e., jobs in this queue run).</p>
<p>A user can choose to deactivate a queue under certain conditions. Some governance installations add multiple queues to organize Collect jobs or dgSAP refreshes by Waves. If a Wave is on hold AND all its refreshes are assigned to one queue, this queue could be deactivated.</p></td>
</tr>
<tr class="even">
<td><p>STOP</p></td>
<td><p>Click to stop the job currently running in the queue. Subsequent jobs will not start until the queue is started again.</p></td>
</tr>
<tr class="odd">
<td><p>START</p></td>
<td><p>Click to start jobs running in the queue.</p></td>
</tr>
<tr class="even">
<td><p>CLEAR QUEUE</p></td>
<td><p>Click to clear the Recent Service Activity log.</p></td>
</tr>
<tr class="odd">
<td><p>LOG</p></td>
<td><p>Click to open the <a href="Recent%20Service%20Activity.htm">Recent Service Activity</a> log to view completed jobs.</p></td>
</tr>
<tr class="even">
<td><p>ACKNOWLEDGE FAILURES</p></td>
<td><p>Click to acknowledge failed jobs to indicate that the issue that caused the job to fail has been debugged and fixed, and there is no longer a need to keep the failed record.</p></td>
</tr>
</tbody>
</table>
