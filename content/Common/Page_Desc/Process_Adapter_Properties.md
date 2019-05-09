+++
title = 'Process Adapter Properties'
solution = 'Platform'
+++

# Process Adapter Properties

<div class="use">

Use this page to [Modify the Process Adapter
Properties](../Use_Cases/Process_Adapters#Modify_the_Process_Adapter_Properties).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Common \> Configuration \>
    Process Adapters</span> in the
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Properties</span> icon
    for a process.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PROPERTY NAME</p></td>
<td><p>Displays the property name. This field is not editable.</p>
<p>The available property names are:</p>
<ul>
<li><strong>OperationTimeoutMinutes</strong> - This is the timeout value to wait for the Data Services Web service to respond or for the job import utility to complete the import process. If the timeout is exceeded, this generally indicates a problem with execution. This value must be at least 1.</li>
<li><strong>PollTimeOut</strong> - This is a timeout value used by 'JobPolling_' prefixed Process Adapter entries and is the overall time to wait for a requested Data Services Job to execute. The default value for this property is 480 minutes (8 hours) as some DS jobs run for a long period of time. This property is editable. This value must be at least 10 and is in minutes.</li>
<li><strong>PollTimerWait</strong> - This is a value used by 'JobPolling_' prefixed Process Adapter entries that is the time interval to wait between making web service calls to check if a Data Services job has completed or not. This defaults to 60 seconds but is also editable as needed. This value must be at least 30 and is in seconds.</li>
</ul></td>
</tr>
<tr class="odd">
<td><p>TYPE NAME</p></td>
<td><p>Displays the type of the property. This field is not editable.</p></td>
</tr>
<tr class="even">
<td><p>VALUE</p></td>
<td><p>Displays the operation timeout in minutes for the OperationTimeoutMinutes and PollTimeOut properties and operation timeout in seconds for the PollTimerWait property.</p></td>
</tr>
<tr class="odd">
<td><p>DESCRIPTION</p></td>
<td><p>Displays the description of the property.</p></td>
</tr>
</tbody>
</table>
