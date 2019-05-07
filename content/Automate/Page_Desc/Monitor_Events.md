+++
title = ''
solution = 'Platform'
+++

# <span id="MonitorEventsH"></span> Monitor (Events) H

[Monitor (Events) V](#MonitorEventsV)

<div class="use">

Use this page to [Monitor Interfaces &
Events](../Use_Cases/Monitor_Interfaces_Events.htm). 

</div>

To access this page:

1.  Select **Monitor** in the *Navigation* pane.

2.  Click the **Events** icon for the desired interface.
    
    Or

3.  Select **Interfaces** in the *Navigation* pane to monitor a single
    interface.

4.  Click **Vertical View** for the desired interface.

5.  Click the **Monitor** icon.

6.  Click the **Events** icon for the desired interface.

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>INTERFACE</p></td>
<td><p>Displays the name of the interface to which the event was added.</p></td>
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
<td><p>OBJECT</p></td>
<td><p>Displays the name of the workflow view (with the naming convention wf:[WorkflowView])or the stored procedure (with the naming convention sp:[StoredProcedureName])</p>
<p><strong>NOTE:</strong> This field is only populated for Workflow and Stored Procedure events.</p></td>
</tr>
<tr class="even">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the page for which the event runs. This value is pulled from the PAGE ID field on the <em><a href="Interface_Events.htm">Interface Events</a></em> page</p>
<p><strong>NOTE:</strong> This field only applies to WebApp events. </p></td>
</tr>
<tr class="odd">
<td><p>INSTANCE ID</p></td>
<td><p>Displays the ID of the instance that the event ran against.</p></td>
</tr>
<tr class="even">
<td><p>TIME STARTED</p></td>
<td><p>Displays the time that the event started running.</p></td>
</tr>
<tr class="odd">
<td><p>TIME COMPLETED</p></td>
<td><p>Displays the time that the event finished running.</p>
<p><strong>NOTE:</strong> This field is not populated if the event failed.</p></td>
</tr>
<tr class="even">
<td><p>DURATION</p></td>
<td><p>Displays the time, in seconds, it took for the event to run. </p></td>
</tr>
<tr class="odd">
<td><p>COMPLETED</p></td>
<td><p>If checked, the event successfully completed.</p>
<p>If unchecked, the event failed.</p></td>
</tr>
<tr class="even">
<td><p>STATUS</p></td>
<td><p>Displays the status of the event. Options are:</p>
<ul>
<li><strong>Completed -</strong> The event has completed</li>
<li><strong>Failed -</strong> The event has failed</li>
<li><strong>Running -</strong> The event is currently running</li>
<li><strong>NotComplete -</strong> The I/O file processing is currency running and is looping</li>
</ul></td>
</tr>
</tbody>
</table>

 

# <span id="MonitorEventsV"></span> Monitor (Events) V

[Monitor (Events) H](#MonitorEventsH)

<table>
<tbody>
<tr class="odd">
<td><p><strong>Field</strong></p></td>
<td><p><strong>Description</strong></p></td>
</tr>
<tr class="even">
<td><p>Interface</p></td>
<td><p>Displays the name of the interface to which the event was added.</p></td>
</tr>
<tr class="odd">
<td><p>Event ID</p></td>
<td><p>Displays a system-generated ID to uniquely identify the event.</p></td>
</tr>
<tr class="even">
<td><p>Event</p></td>
<td><p>Displays the event that executed.</p></td>
</tr>
<tr class="odd">
<td><p>OBJECT</p></td>
<td><p>Displays the name of the workflow view (with the naming convention wf:[WorkflowView])or the stored procedure (with the naming convention sp:[StoredProcedureName])</p>
<p><strong>NOTE:</strong> This field is only populated for Workflow and Stored Procedure events.</p></td>
</tr>
<tr class="even">
<td><p>Description</p></td>
<td><p>Displays the page for which the event runs. This value is pulled from the PAGE ID field on the <em><a href="Interface_Events.htm">Interface Events</a></em> page</p>
<p><strong>NOTE:</strong> This field only applies to WebApp events. </p></td>
</tr>
<tr class="odd">
<td><p>Comment</p></td>
<td><p>Displays a description of the event.</p></td>
</tr>
<tr class="even">
<td><p>Instance ID</p></td>
<td><p>Displays the ID of the instance that the event ran against.</p></td>
</tr>
<tr class="odd">
<td><p>Time Started</p></td>
<td><p>Displays the time that the event started running.</p></td>
</tr>
<tr class="even">
<td><p>Time Completed</p></td>
<td><p>Displays the time that the event finished running.</p>
<p><strong>NOTE:</strong> This field is not populated if the event failed.</p></td>
</tr>
<tr class="odd">
<td><p>Completed</p></td>
<td><p>If checked, the interface completed without failing.</p>
<p>If unchecked, the interface is either currently running or failed.</p></td>
</tr>
<tr class="even">
<td><p>Status</p></td>
<td><p>Displays the status of the event. Options are:</p>
<ul>
<li><strong>Completed -</strong> The event has completed</li>
<li><strong>Failed -</strong> The event has failed</li>
<li><strong>Running -</strong> The event is currently running</li>
<li><strong>NotComplete -</strong> The I/O file processing is currency running and is looping</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>Message</p></td>
<td><p>Displays the message that is displayed when the event fails.</p></td>
</tr>
<tr class="even">
<td><p>Retry Step</p></td>
<td><p>This field is not used.</p></td>
</tr>
</tbody>
</table>
