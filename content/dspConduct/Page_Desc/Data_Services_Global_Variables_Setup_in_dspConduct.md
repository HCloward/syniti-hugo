+++
title = 'Data Services Global Variables Setup'
solution = 'Master Data Management'
+++

# Data Services Global Variables Setup

<div class="use">

Use this page to [Configure Data Download During the Final Finish
Process to use a Data Services
Job](../Use_Cases/Configure_Data_Download_During_the_Final_Finish_Process_to_use_a_Data_Services_Job.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the *Navigation* pane.
2.  Click the **Tasks** icon for a category.
3.  Click the **Final Finish Tables** icon for a main parent task.
4.  Click **Vertical View** for a record with the Finish Type of
    DataServices.
5.  Click the **Global Variables** icon.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>NAME</p></td>
<td><p>Displays the variable name.</p>
<p>The RequestID global variable does not need to be registered. It is always passed to the Data Services job during the Finish process.</p></td>
</tr>
<tr class="odd">
<td><p>CONSTANT</p></td>
<td><p>Displays the value for the variable.</p>
<p>This value will be passed to the Data Services job at runtime. The job is executed based on the parameters specified.</p></td>
</tr>
</tbody>
</table>
