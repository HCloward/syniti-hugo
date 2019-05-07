+++
title = 'Task Final Finish Tables H'
solution = 'Master Data Management'
+++

# Task Final Finish Tables H

[Task Final Finish Tables
V](Task_Final_Finish_Tables_H.htm#ask_Final_Finish_Tables_V)

<div class="use">

Use this page to:

  - [Configure Data Download During the Final Finish Process to use a
    Data Services
    Job](../Use_Cases/Configure_Data_Download_During_the_Final_Finish_Process_to_use_a_Data_Services_Job.htm)
  - [Configure Data Download During the Final Finish Process to use a
    CranPort
    Package](../Use_Cases/Configure_Data_Download_During_the_Final_Finish_Process_to_use_a_CranPort_Package.htm)
  - [Configure Data Download During the Final Finish Process to use a
    DBMoto Package](../Use_Cases/Configure_FinalFinish_DBMoto.htm)

</div>

To access this page:

1.  Click **dspConduct \> Design** in the *Navigation* pane.
2.  Click the **Tasks** icon for a category.
3.  Click the **Final Finish Tables** icon for a main parent task.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>FINISH TYPE</p></td>
<td><p>Displays whenever tables:</p>
<ul>
<li>Are downloaded (CranPort)</li>
<li>If the Finish Type is CranPort, then a corresponding table definition must exist in Collect.</li>
<li>Use a Data Services Job that runs to download the tables (DataServices) to pull data from the source environment and add it to the target environment.</li>
</ul>
<p><strong>NOTE:</strong> If the Finish Type is DataServices, the Data Services Job must exist in the Data Services Data Source.</p>
<ul>
<li>Use DBMoto® to keep the target table synchronized with the source table.</li>
</ul>
<p><strong>NOTE:</strong> If the Finish Type is DBMoto, then a corresponding table definition must exist in Collect.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays the execution order of CranPort packages or Data Services jobs.Does not apply to DBMoto packages.</p>
<p>The execution order of packages is by priority of the role (specified on the <em><a href="Role_H_dspConduct.htm">Role</a></em> page) to which the task is assigned, and then the order is specified by the order in which the package is added on the <span style="font-style: italic;"><a href="Task_Final_Finish_Tables_H.htm">Task Final Finish Tables</a></span> page.</p></td>
</tr>
<tr class="even">
<td><p>DATA SERVICES JOB NAME</p></td>
<td><p>Displays the name of the job written in Data Services that is used to pull data from the source environment and add it to the target environment.</p>
<p><strong>NOTE:</strong> This field is not available for Finish Type of CranPort or DBMoto®.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE</p></td>
<td><p>Displays name of the source database registered in Collect where tables are downloaded from.</p>
<p><strong>NOTE:</strong> This field is not used when registering a Data Services job</p></td>
</tr>
<tr class="even">
<td><p>TARGET</p></td>
<td><p>Displays name of the target database registered in Collect where table data is refreshed from the source database.</p>
<p><strong>NOTE:</strong> This field is not used when registering a Data Services job.</p></td>
</tr>
<tr class="odd">
<td><p>TABLE NAME</p></td>
<td><p>Displays name of table downloaded from the source database when the Finish role is processed for the assigned role.</p></td>
</tr>
</tbody>
</table>

## <span id="ask_Final_Finish_Tables_V"></span>Task Final Finish Tables V

[Task Final Finish Tables H](Task_Final_Finish_Tables_H.htm)

**NOTE:** The fields that display on this page are determined by the
selected Finish Type.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Finish Type</p></td>
<td><p>Displays whenever tables:</p>
<ul>
<li>Are downloaded (CranPort)</li>
</ul>
<p><strong>NOTE:</strong> If the Finish Type is CranPort, then a corresponding table definition must exist in Collect.</p>
<ul>
<li>Use a Data Services Job that runs to download the tables (DataServices) to pull data from the source environment and add it to the target environment.</li>
</ul>
<p><strong>NOTE:</strong> If the Finish Type is DataServices, the Data Services Job must exist in the Data Services Data Source.</p>
<ul>
<li>Use DBMoto® to keep the target table synchronized with the source table.</li>
</ul>
<p><strong>NOTE:</strong> If the Finish Type is DBMoto, then a corresponding table definition must exist in Collect.</p></td>
</tr>
<tr class="odd">
<td><p>Priority</p></td>
<td><p>Displays the execution order of CranPort packages or Data Services jobs. Does not apply to DBMoto packages.</p>
<p>The execution order of packages is by priority of the role (specified on the <a href="Role_H_dspConduct.htm"><em>Role</em></a> page) to which the task is assigned, and then the order is specified by the order in which the package is added on the <a href="Task_Final_Finish_Tables_H.htm"><em>Task Final Finish Tables</em></a> page.</p></td>
</tr>
<tr class="even">
<td><p>Source</p></td>
<td><p>Displays name of the source database registered in Collect where tables are downloaded from.</p>
<p><strong>NOTE:</strong> This field is not used when registering a Data Services job.</p></td>
</tr>
<tr class="odd">
<td><p>Target</p></td>
<td><p>Displays name of the target database registered in Collect where table data is refreshed from the source database.</p>
<p><strong>NOTE:</strong> This field is not used when registering a Data Services job.</p></td>
</tr>
<tr class="even">
<td><p>Table Name</p></td>
<td><p>Displays name of table downloaded from the source database when the Finish role is processed for the assigned role and used only for a Finish Type of CranPort.</p></td>
</tr>
<tr class="odd">
<td><p>Run Rules After Download</p></td>
<td><p>This option determines the Collect rules to run on a table after download when a user with the Post role clicks Finish for the request on the <em><a href="Request_Role_H.htm">Request Role</a></em> page. Options are:</p>
<ul>
<li><strong>All – Run all of the rules:</strong> If multiple rules are registered to the table in Collect, dspConduct™ runs them on the table after download in the order the rules were added on the Collect <span style="font-style: italic;"><a href="../../../Platform/Collect/Page_Desc/Table_Rule_H.htm">Table (Rule)</a></span> page.</li>
<li><strong>None – Do not run any rules:</strong> Though rules are registered to the table in Collect, dspConduct™ does not run those rules on the downloaded table.</li>
<li><strong>NoParametersOnly</strong> – Run only Collect rules that do not contain input parameters, such as an Insert rule.</li>
<li><strong>ParametersOnly</strong> – Run Collect rules that contain input parameters, such as an Update rule.</li>
</ul>
<p><strong>NOTE:</strong> The rule(s) must have already been registered and activated in Collect.</p>
<p><strong>NOTE:</strong> This field does not display if the finish type is Data Services or DBMoto®.</p></td>
</tr>
<tr class="even">
<td><p>Data Services Data Source</p></td>
<td><p>Displays the name of the data source that stores the Data Services job.</p>
<p><strong>NOTE:</strong> This field is not available for Finish Type of CranPort.</p></td>
</tr>
<tr class="odd">
<td><p>Data Services Job Name</p></td>
<td><p>Displays the name of the job written in Data Services that is used to pull data from the Source environment and add it to the target environment.</p>
<p><strong>NOTE:</strong> This field is not available for Finish Type of CranPort.</p></td>
</tr>
<tr class="even">
<td><p>Where Clause Builder</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Task_Final_Finish_Where_Clause.htm">Task Final Finish Where Clause</a></span> page. Where Clauses should be specified for Finish Type of CranPort.</p>
<p><strong>NOTE:</strong> This field does not display if the finish type is Data Services.</p></td>
</tr>
<tr class="odd">
<td><p>Global Variables</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Data_Services_Global_Variables_Setup_in_dspConduct.htm">Data Services Global Variables Setup</a></span> page if the Data Services job is to run on one table only.</p>
<p><strong>NOTE:</strong> This field is not available for Finish Type of CranPort.</p></td>
</tr>
</tbody>
</table>
