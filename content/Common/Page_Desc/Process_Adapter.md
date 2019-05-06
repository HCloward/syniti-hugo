# Process Adapter

<div class="use">

Use this page to [Modify the Process Adapter
Entries](../Use_Cases/Process_Adapters.htm#Modify_the_Process_Adapter_Entries).

</div>

To access this page, select <span style="font-weight: bold;">Common \>
Configuration \> Process Adapters</span> in the
<span style="font-style: italic;">Navigation</span> pane.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>PROCESS NAME</p></td>
<td><p>Displays the name of the external process being accessed via the Process Queue. The names are derived from the name of the Data Services entry in the <span style="font-style: italic;">Data Source Registry</span> page (the Name column from the ttDataSourceRegistry table in the DSPCommon database) with a prefix based on the operation the processes  perform. This is necessary to create separate queues for each Data Services instance that is registered. The names for Execute and Polling processes have the following naming convention:</p>
<ul>
<li>JobExecute_&lt;Data Source Registry Name&gt;</li>
<li>JobPolling_&lt;Data Source Registry Name&gt;</li>
</ul>
<p>The entries with the prefix of 'JobExecute_' and 'JobPolling_' are used to make the calls to Data Services to execute and wait for a job to complete.</p>
<p>These processes can have different properties set on the <span style="font-style: italic;">Process Adapters Properties</span> page as they are different types of processes that are being called.</p></td>
</tr>
<tr class="odd">
<td><p>ASSEMBLY FILE</p></td>
<td><p>Displays the full name of the .NET DLL file that is the wrapper for code that calls the external process.</p></td>
</tr>
<tr class="even">
<td><p>TYPE NAME</p></td>
<td><p>Displays the Type (class) name in the .NET DLL that acts as a proxy to call the external process.</p></td>
</tr>
<tr class="odd">
<td><p>TYPE FULL NAME</p></td>
<td><p>Displays the long name for the Type (class). This is required for loading the code to call the external process.</p></td>
</tr>
<tr class="even">
<td><p>MAX INSTANCE COUNT</p></td>
<td><p>Displays the maximum number of calls that can be made simultaneously for all users for the given process. This would either be active calls to a Data Services instance or Job Imports to a Data Services instance.</p>
<p>This value cannot be less than 1.</p></td>
</tr>
<tr class="odd">
<td><p>Properties</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Process_Adapter_Properties.htm">Process Adapter Properties</a></span> page to modify process adapter properties.</p></td>
</tr>
</tbody>
</table>
