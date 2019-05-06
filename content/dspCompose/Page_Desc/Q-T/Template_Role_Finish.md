# Template Role (Finish)

<div class="use">

Use this page to:

  - [Register Tables for Download as a Finish Process using
    Collect](../Use_Cases/Register_Tables_to_Download_as_a_Finish_Process_Using_Collect.htm)
  - [Register Tables for Download through Data
    Services](../Use_Cases/Register_Tables_for_Download_through_Data_Services.htm)

</div>

To access this page:

1.  Click <span style="font-weight: bold;">dspCompose \>
    Team</span> on *Navigation *pane.
2.  Click <span style="font-weight: bold;">Templates</span> for a team.
3.  Click <span style="font-weight: bold;">Roles</span> for a template.
4.  Click <span style="font-weight: bold;">Vertical View</span> for the
    Post role.
5.  Click the <span style="font-weight: bold;">Approve and Finish
    Settings</span> tab.
6.  Click <span style="font-weight: bold;">Finish Tables</span>.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>SOURCE</p></td>
<td><p>Displays name of the source database registered in Collect where tables are downloaded from.</p>
<p><strong>NOTE:</strong> This field is not used when registering a Data Services job.</p></td>
</tr>
<tr class="odd">
<td><p>TARGET</p></td>
<td><p>Displays name of the target database registered in Collect where table data is refreshed from the source database.</p>
<p><strong>NOTE:</strong> This field is not used when registering a Data Services job.</p></td>
</tr>
<tr class="even">
<td><p>TABLE NAME</p></td>
<td><p>Displays name of table downloaded from the source database when the Finish role is processed for the assigned role.</p>
<p><strong>NOTE:</strong> This field is not used when registering a Data Services job.</p></td>
</tr>
<tr class="odd">
<td><p>RUN RULES AFTER DOWNLOAD</p></td>
<td><p>This option determines the Collect rules to run on a table after download when a user with the Post role clicks Finish for the request on the <em>Request (Roles)</em> page. Options are:</p>
<ul>
<li><strong>All – Run all of the rules</strong>: If multiple rules are registered to the table in Collect, dspCompose™ will run them on the table after download in the priority order set on the <em>Collect Table (Rule)</em> page.</li>
<li><strong>None – Do not run any rules:</strong> Though rules are registered to the table in Collect, dspCompose™ will not run those rules on the downloaded table.</li>
<li><strong>NoParametersOnly –</strong> Run only Collect rules that do not contain input parameters, such as an Insert rule.</li>
<li><strong>ParametersOnly –</strong> Run Collect rules that contain input parameters, such as an Update rule.</li>
</ul>
<p><strong>NOTE:</strong> The rule(s) must have already been registered and activated in Collect.</p>
<p><strong>NOTE:</strong> This field is not used when registering a Data Services job.</p></td>
</tr>
<tr class="even">
<td><p>DATA SERVICES DATA SOURCE</p></td>
<td><p>Displays the name of the data source that stores the Data Services job.</p>
<p><strong>NOTE:</strong> This field is not used when registering tables for download as a Finish Process using Collect.</p></td>
</tr>
<tr class="odd">
<td><p>DATA SERVICES JOB NAME</p></td>
<td><p>Displays the name of the job written in Data Services that will be used to pull data from the SAP environment and add it the database dgSAP, the working snapshot of the SAP data.</p>
<p><strong>NOTE:</strong> This field is not used when registering tables for download as a Finish Process using Collect.</p></td>
</tr>
<tr class="even">
<td><p>Source Filter Columns</p></td>
<td><p>Click to open the <em><a href="Template_Role_Finish_Columns_H.htm"><em>Template Role (Finish-Columns)</em></a></em> page to add, edit and delete a list of columns used to form the where clause for selecting values from the source database. If no columns are set up, the entire table is downloaded.</p>
<p><strong>NOTE:</strong> This field is not used when registering a Data Services job.</p></td>
</tr>
<tr class="odd">
<td><p>Target Filter Columns</p></td>
<td><p>Click to open the <em><a href="Template_Role_Finish_Columns_H.htm"><em>Template Role (Finish-Columns)</em></a></em> page to add, edit and delete a list of columns used to form the where clause for selecting values to delete from the target database before data is refreshed from the source database. If no columns are set up, the entire table is downloaded.</p>
<p><strong>NOTE:</strong> This field is not used when registering a Data Services job.</p></td>
</tr>
<tr class="even">
<td><p>Global Variables</p></td>
<td><p>Click to open the <em><a href="Data_Services_Global_Variables_Setup.htm"><em>Data Services Global Variables Setup</em></a></em> page to add, edit or delete global variables for the Data Services job.</p>
<p><strong>NOTE:</strong> The RequestID variable is automatically populated and does not need to be registered.</p>
<p><strong>NOTE:</strong> This icon is not used when registering tables for download as a Finish Process using Collect.</p></td>
</tr>
</tbody>
</table>
