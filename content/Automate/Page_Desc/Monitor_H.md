+++
title = ''
solution = 'Platform'
+++

# <span id="MonitorH"></span> Monitor H

[Monitor V](#MonitorV)

<div class="use">

Use this page to [Monitor Interfaces &
Events](../Use_Cases/Monitor_Interfaces_Events.htm).

</div>

To access this page, select **Monitor** in the *Navigation* pane.

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>TIME STARTED</p></td>
<td><p>Displays the time that the interface started running.</p></td>
</tr>
<tr class="odd">
<td><p>INSTANCE ID</p></td>
<td><p>Displays the ID of the instance that the interface ran against.</p></td>
</tr>
<tr class="even">
<td><p>INTERFACE</p></td>
<td><p>Displays the name of the interface.</p></td>
</tr>
<tr class="odd">
<td><p>EVENT ID</p></td>
<td><p>Displays a system-generated ID to uniquely identify the event.</p></td>
</tr>
<tr class="even">
<td><p>EVENT</p></td>
<td><p>Displays the event that executed.</p></td>
</tr>
<tr class="odd">
<td><p>STATUS</p></td>
<td><p>Displays the status of the event. Options are:</p>
<ul>
<li><strong>Completed -</strong>The event has completed</li>
<li><strong>Failed -</strong>The event has failed</li>
<li><strong>Running -</strong> The event is currently running</li>
<li><strong>NotComplete -</strong> The I/O file processing is currency running and is looping</li>
</ul></td>
</tr>
<tr class="even">
<td><p>NEXT RETRY DATE</p></td>
<td><p>Displays the next date on which to retry running the interface if the event failed. Refer to <a href="../Use_Cases/Set_Retry_Parameters.htm">Set Retry Parameters</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>RETRY COUNT</p></td>
<td><p>Displays how many times the interface was retried before it failed.</p></td>
</tr>
<tr class="even">
<td><p>CURRENT DURATION</p></td>
<td><p>Displays the time, in seconds, it has taken for the most current run of the interface to run. This duration is calculated from the time the job started to the current time.</p></td>
</tr>
<tr class="odd">
<td><p>AVERAGE DURATION</p></td>
<td><p>Displays the average time, in seconds, it takes for the interface to complete running.</p></td>
</tr>
<tr class="even">
<td><p>Events</p></td>
<td><p>Click to open the <a href="Monitor_Events.htm"><em>Monitor (Events)</em></a> page to view and interact with interface events that are currently running or that have failed.</p>
<p>The count on the icon is the total number of events registered to the selected interface.</p></td>
</tr>
<tr class="odd">
<td><p>Acknowledge</p></td>
<td><p>Click to acknowledge that the failed job has been debugged and fixed; the record is removed from the page.</p></td>
</tr>
</tbody>
</table>

# <span id="MonitorV"></span> Monitor V

[Monitor H](#MonitorH)

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>Instance ID</p></td>
<td><p>Displays the ID of the instance that the interface ran against.</p></td>
</tr>
<tr class="odd">
<td><p>Interface ID</p></td>
<td><p>Displays a system-generated unique ID to identify the interface.</p></td>
</tr>
<tr class="even">
<td><p>Active</p></td>
<td><p>If checked, the interface has been tested and is ready to be run.</p>
<p>If unchecked, the interface has not been tested and is not ready to be run.</p></td>
</tr>
<tr class="odd">
<td><p>Time Started</p></td>
<td><p>Displays the time that the interface started running.</p></td>
</tr>
<tr class="even">
<td><p>Completed</p></td>
<td><p>If checked, the event successfully completed.</p>
<p>If unchecked, the event is either currently running or failed.</p></td>
</tr>
<tr class="odd">
<td><p>Next Retry Date</p></td>
<td><p>Displays the next date on which to retry running the interface if it failed. Refer to <a href="../Use_Cases/Set_Retry_Parameters.htm">Set Retry Parameter</a>s for more information.</p></td>
</tr>
<tr class="even">
<td><p>Retry Count</p></td>
<td><p>Displays how many times the interface was retried before it failed.</p></td>
</tr>
<tr class="odd">
<td><p>Status</p></td>
<td><p>Displays the status of the interface. Options are:</p>
<ul>
<li><strong>Completed -</strong> the event has completed</li>
<li><strong>Failed -</strong> the event has failed</li>
<li><strong>Running -</strong> the event is currently running</li>
<li><strong>NotComplete -</strong> the I/O file processing is currency running and is looping</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Message</p></td>
<td><p>Displays the message that is displayed when the interface fails.</p></td>
</tr>
<tr class="odd">
<td><p>Events</p></td>
<td><p>Click to open the <em><a href="Monitor_Events.htm">Monitor (Events)</a></em> page to view and interact with interface events that are currently running or that have failed.</p>
<p>The count on the icon is the total number of events registered to the selected interface.</p></td>
</tr>
<tr class="even">
<td><p>Submit Retry</p></td>
<td><p>Click to re-submit the event to the job queue (i.e., run the event in the background)</p></td>
</tr>
<tr class="odd">
<td><p>Stop</p></td>
<td><p>Click to stop the running interface.</p></td>
</tr>
</tbody>
</table>
