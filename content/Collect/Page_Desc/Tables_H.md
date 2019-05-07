+++
title = 'Tables H'
solution = 'Platform'
+++

# Tables H

[Tables V (All Tabs](#Tables_V_All_Tabs))

<div class="use">

Use this page to:

  - [Set up Schedule Groups](../Config/Set_Up_Schedule_Groups.htm)
  - [Manually Register Tables to
    Source](../Use_Cases/Manually_Register_Tables_to_Source.htm)
  - [Schedule Table
    Refresh](../Use_Cases/Schedule_Updates_to_Tables.htm)
  - [Set up Download with CranPort
    Package](../Use_Cases/Set_Up_Table_Download_with_a_CranPort_Package.htm#Set_up_Download_with_CranPort_Package)
  - [Set up Download with ManualCranPort
    Package](../Use_Cases/Set_Up_Table_Download_with_a_CranPort_Package.htm#Set_up_Download_with_ManualCranPort_Package)
  - [Download sdb Tables in
    Collect](../../../Migration/Map/Use_Cases/Download_Tables_Map.htm)
  - [Download dgSAP Tables in
    Collect](../../../Migration/Map/Use_Cases/Download_Tables_Map.htm)

</div>

<span style="font-weight: bold;">NOTE:</span> Bulk Execution has been
enabled on this page. Refer to [Use Bulk
Execution](../../Bulk_Exec/Use_Bulk_Execution.htm) for more information.

**NOTE:** To receive a workflow email that a table download has failed
in Collect, a user must be assigned to a security role that has the
Collect WebApp group WorkFlowFailureAll or WorkFlowFaiureByTargetAccess
assigned. Refer to [Set
Security](../../Sys_Admin/Use_Cases/Setting_security.htm) in System
Administration for more information.

To access this page:

1.  Click <span style="font-weight: bold;">Collect \> Targets</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click the <span style="font-weight: bold;">Sources</span> icon for a
    target.
3.  Click the <span style="font-weight: bold;">Tables</span> icon for a
    source.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Build And Refresh</p></td>
<td><p>Click to build the package and download active tables from the source. If the package already exists, the table is refreshed (i.e., data is downloaded from the source database). If the package does not exist, a package is immediately scheduled to be built and the table is refreshed. The Refresh icon is disabled for DBMoto® package types because the refresh is run by DBMoto® instead of by Collect.</p>
<p><strong>NOTE:</strong> If the data in the table has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance.htm#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset a running refresh. This process activates the Refresh icon and triggers batch job schedule to calculate new run dates for next scheduled refresh. Reset source if the download process backs up due to network problems.</p></td>
</tr>
<tr class="even">
<td><p>Build Package</p></td>
<td><p>Click to build a package to download active tables from the source.</p>
<p><strong>NOTE:</strong> If the data in the table has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance.htm#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Refresh</p></td>
<td><p>Click to manually extract a copy of data from the source and load into the target.</p>
<p><strong>NOTE:</strong> If the Target Source uses an IG Universal Connect data source, clicking Refresh executes the Boomi Process.</p>
<p><strong>NOTE:</strong> If the data in the table has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance.htm#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>TARGET</p></td>
<td><p>Displays the database where tables are refreshed with source data.</p></td>
</tr>
<tr class="odd">
<td><p>SOURCE</p></td>
<td><p>Displays the database where data is refreshed from and stored in the target.</p></td>
</tr>
<tr class="even">
<td><p>TABLE</p></td>
<td><p>Displays table name in the source database.</p></td>
</tr>
<tr class="odd">
<td><p>PACKAGE TYPE</p></td>
<td><p>Displays package type to refresh target table with source data. Default value is <strong>CranPort</strong>. Refer to <a href="../Use_Cases/Package_Types.htm">Package Types</a> for a description of each package type available.</p>
<p><strong>NOTE</strong>: The component is referred to as Assemble in the help. The package type is still CranPort.</p>
<p><strong>NOTE:</strong> When the package type is CranPort package, the package name is hyperlinked to the CranPort package in Assemble in the view.</p>
<p><strong>NOTE:</strong> If source has an SAPAPPSERVER connection type, only the following RFC package types are available in the Package Type list box:</p>
<ul>
<li>BOA RFC</li>
<li>SAP Data Services using RFC</li>
<li>SAP RFC</li>
<li>SAP Text</li>
</ul></td>
</tr>
<tr class="even">
<td><p>ACTIVE</p></td>
<td><p>If enabled, table is active. Only active tables are downloaded from the source during refresh. Default value is Active.</p></td>
</tr>
<tr class="odd">
<td><p>BUILT</p></td>
<td><p>If enabled, package for table has been built. This setting cannot be updated from within Collect.</p></td>
</tr>
<tr class="even">
<td><p>DURATION</p></td>
<td><p>Displays amount of time (in seconds) it took for the table to download from the source. This field is protected and updated by Collect when the table refresh process completes.</p></td>
</tr>
<tr class="odd">
<td><p>UOM</p></td>
<td><p>Displays the Unit of Measure used for measure the duration.</p></td>
</tr>
<tr class="even">
<td><p>RECORD COUNT</p></td>
<td><p>Displays number of records in the table. This field is protected and updated by Collect when the table refresh process completes.</p></td>
</tr>
<tr class="odd">
<td><p>PRIORITY</p></td>
<td><p>Displays order that tables are refreshed with source data and sorted on the page. Default value is <strong>99999</strong>.</p></td>
</tr>
<tr class="even">
<td><p>COMPLETED</p></td>
<td><p>Displays date and time when the manual refresh completed.</p></td>
</tr>
<tr class="odd">
<td><p>NEXTRUN</p></td>
<td><p>Displays next scheduled date and time when the refresh process is scheduled to run.</p></td>
</tr>
<tr class="even">
<td><p>Rules</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Table_Rule_H.htm">Table (Rule)</a></span> page to register rules to table.</p></td>
</tr>
<tr class="odd">
<td><p>Indices</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Table_Indices_H.htm">Table (Indices)</a></span> page to register indices to table.</p></td>
</tr>
<tr class="even">
<td><p>View Data</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Tables_H.htm">Tables</a></span> page to view table data downloaded from source.</p></td>
</tr>
</tbody>
</table>

## <span id="Tables_V_All_Tabs"></span>Tables V (All Tabs)

[Tables H](Tables_H.htm)

<div class="use">

Use this page to:

  - [Manually Register Tables to
    Source](../Use_Cases/Manually_Register_Tables_to_Source.htm)
  - [Schedule Table
    Refresh](../Use_Cases/Schedule_Updates_to_Tables.htm)
  - [Set up Download with CranPort
    Package](../Use_Cases/Set_Up_Table_Download_with_a_CranPort_Package.htm#Set_up_Download_with_CranPort_Package)
  - [Set up Download with ManualCranPort
    Package](../Use_Cases/Set_Up_Table_Download_with_a_CranPort_Package.htm#Set_up_Download_with_ManualCranPort_Package)

</div>

This page contains the following tabs:

  - [General tab](#General_Tab1)
  - [Advanced Settings tab](#Advanced_Settings_Tab1)
  - [General Information tab](#General_Information_Tab)
  - [Action tab](#Action_Tab1)
  - [Data Protection tab](#Data)

## <span id="General_Tab1"></span>General tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Build Package</p></td>
<td><p>Click to build a package to download active tables from the source.</p>
<p><strong>NOTE:</strong> If the data in the table has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance.htm#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset a running refresh. This process activates the Refresh icon and triggers batch job schedule to calculate new run dates for next scheduled refresh. Reset source if the download process backs up due to network problems.</p></td>
</tr>
<tr class="even">
<td><p>Refresh</p></td>
<td><p>Click to manually extract a copy of data from the source and load into the target.</p>
<p><strong>NOTE:</strong> If the Target Source uses an IG Universal Connect data source, clicking Refresh executes the Boomi Process.</p>
<p><strong>NOTE:</strong> If the data in the table has been purged manually, or the retention expiration date for that object has passed, it cannot be refreshed and this icon is inactive. Refer to <a href="../Use_Cases/Support_Regulatory_Compliance.htm#Purge_Data">Purge Data</a> for more information.</p></td>
</tr>
<tr class="odd">
<td><p>Target</p></td>
<td><p>Displays the target database where tables are refreshed with source data.</p></td>
</tr>
<tr class="even">
<td><p>Source</p></td>
<td><p>Displays the database where data is refreshed from and stored in the target.</p></td>
</tr>
<tr class="odd">
<td><p>Table</p></td>
<td><p>Displays table in the source database.</p></td>
</tr>
<tr class="even">
<td><p>Active</p></td>
<td><p>If enabled, table is active. Only active tables are downloaded from the source during refresh. Default value is Active.</p></td>
</tr>
<tr class="odd">
<td><p>Description</p></td>
<td><p>Displays information about table, for example, data contained within table.</p></td>
</tr>
</tbody>
</table>

## <span id="Advanced_Settings_Tab1"></span>Advanced Settings tab

Field

Description

Table Rename

Displays the table name of the renamed table in target database. New
table name must contain \[TableName\]. At run time, \[TableName\] is
replaced with processing table name.

Where Clause Override

Displays a Where Clause that is used to limit data downloaded during a
refresh process.

Table Schema Owner

Displays the database’s schema for the table.

NextRun

Displays next date and time when the refresh process is scheduled to
run.

Package Type

Displays package type to refresh the target table with source data.
Default value is **CranPort**.

Package Name

Displays name of package that refreshes target table with source data.

**NOTE:** The package name is set automatically and displays after the
package is built for the package types CranPort, SSIS, or Data Services.
The package must be manually built and the package name must be entered
into Collect for package types ManualCranPort, ManualSSIS or Manual Data
Services.

**NOTE:** The package name must follow the naming convention
\#Database\#%\#Source\#%. Refer to [Create
Packages](../../Assemble/Create_Packages.htm) for more information.

**NOTE:** For Manual Data Services package types, select from the list
of available jobs in the Data Services Repository assigned to the target
on the *[Targets](Targets_H_Collect.htm#Targets_V)* page’s *Vertical*
View.

Schedule ID

Displays schedule for when target tables are refreshed with source data.
Options are controlled in Common \> Configuration \> Schedules. Default
value is **Use Source Schedule setting. No Table Override Requested**.

Schedule Group

Displays schedule to build packages, refresh or filter on tables in a
group. Schedule Groups are managed in Configuration \> Schedule Groups.
Default value is **No Group**.

**NOTE:** If building a group with a DBMoto® package the following
applies:   
If Schedule Group is set to NO GROUP, both Download and Mirror package
will be built as an individual replication in DBMoto®.   
If Schedule Group is set to AUTO and if it is a Download package, the
replication will be part of a group named \<GroupPrefix\>\_Downloads.
Otherwise, if it is a Mirror package the replication will be part of a
group called \<GroupPrefix\>\_\<number\> where number is an incremental
value to count the number of groups. Groups cannot contain more than
\<Group\_Size\> replications.   
If Schedule Group is set to "existing group name" with no restriction to
the \<Group\_Size\> parameter the replication is built into that group. 

**NOTE:** The Replication Mode must be consistent with the Replication
Group Mode (e.g a download package cannot be grouped with a mirror
package). 

Synchronous

If enabled, packages for Data Services jobs execute synchronously.

If disabled, packages for Data Services jobs execute asynchronously.

With synchronous execution, the build package jobs respect the queue and
wait until jobs are finished before starting another job.

This option applies to the Data Services [Package
Types](../Use_Cases/Package_Types.htm).

Schedule Single Thread

If enabled, table is downloaded from the source in a queue with all
other single-threaded tables. Default value is
<span style="font-weight: bold;">Disabled</span>.

Pooled Table Name

Displays name of SAP pooled table. Collect automatically changes the
download RFC for pooled tables (i.e., SAP tables that store a list of
tables, for example, ATAB stores 200 tables within a single table).
Refer to SAP documentation for more information about pooled tables.

Rfc Records Per Call

Displays number of records returned in a single block for Collect
background process to parse and insert into database. Default value is
**5000**.

Encrypted Columns

Click to open the <span style="font-style: italic;">Target Source Table
Column Encryption</span> page to edit column encryption for the table.

Boomi

Boomi Process

Displays the name of the Boomi Process that runs when the Target Source
is refreshed.

**NOTE**: A Boomi Process must be selected for each table.

**NOTE**: This field only displays if the source is an IG Universal
Connect data source.

## <span id="General_Information_Tab"></span>General Information tab

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Job ID</p></td>
<td><p>Displays unique identifier of with the Platform job that ran the package.</p></td>
</tr>
<tr class="odd">
<td><p>Completed</p></td>
<td><p>Displays date and time when manual refresh completed.</p></td>
</tr>
<tr class="even">
<td><p>Record Count</p></td>
<td><p>Displays number of records in the table. This field is protected and updated by Collect when the table refresh process completes.</p>
<p>If the number of sources registered exceeds the Max Record Sources For Union View parameter threshold set on the <em>Parameters – Collect</em> page, no Record Count is calculated and the field is set to 0.</p></td>
</tr>
<tr class="odd">
<td><p>Table Record Count</p></td>
<td><p>Displays number of records currently in the table. Ideally, this count is the same as Record Count.  If there is no primary key or unique index, this count may display zero but the table could have data.</p></td>
</tr>
<tr class="even">
<td><p>Duration</p></td>
<td><p>Displays amount of time (in seconds) the table took to download from the source during the refresh process.</p></td>
</tr>
<tr class="odd">
<td><p>Refresh Message</p></td>
<td><p>Displays last process that ran against table, e.g., build package, download or reset.</p></td>
</tr>
<tr class="even">
<td><p>View Design</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Data_Source_Tables_H.htm">Data Source Tables</a></span> page to view, edit and delete details about the table.</p></td>
</tr>
<tr class="odd">
<td><p>View Metrics</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="../Use_Cases/Download_Metrics.htm">Download Metrics</a></span> page to view and download metrics for table.</p></td>
</tr>
<tr class="even">
<td><p>View Job Tasks</p></td>
<td><p>Click to open the <span style="font-style: italic;"><a href="Table_Download_Task_List.htm">Table Download Task List</a></span> page to view job tasks used to download table.</p></td>
</tr>
</tbody>
</table>

## <span id="Action_Tab1"></span>Action tab

<div class="use">

Use this tab to [purge
data](../Use_Cases/Support_Regulatory_Compliance.htm#Purge_Data) for
tables.

</div>

|                |                                                                                                                                                                                                             |
| -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field          | Description                                                                                                                                                                                                 |
| Truncate Table | Click to delete all data in the table. Table can then be deactivated if it is no longer required.                                                                                                           |
| Options        | Click to open the <span style="font-style: italic;">Table (Rfc Options)</span>page to configure RFC options used by RFC download process. The icon  is only active if Package Type = BOA RFC using Options. |

<span id="Data_Protection_Tab"></span>

## <span id="Data"></span>Data Protection tab

<div class="use">

Use this tab to:

  - [Configure Data
    Protection](../Use_Cases/Support_Regulatory_Compliance.htm#Configure_Data_Protection)
  - [Update the Retention Expiration
    Date](../Use_Cases/Support_Regulatory_Compliance.htm#Update_the_Retention_Expiration_Date)

</div>

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>Data Controller</p></td>
<td><p>Displays the user responsible for the processing of personal data in the table</p>
<p>Any user or group who is assigned the Data Controller role must have a user account in the DSP. Data Controller must have access to the target based on their assigned security role and security key.</p>
<p><strong>NOTE:</strong> The Collect Administrator must check the WORK FLOW SUMMARY check box for the target and Data Controller on the <em><a href="Workflow_Summary_User_Settings.htm">Workflow Summary User Settings</a></em> page. The Data Controller is added to this page automatically. If the check box is not checked, the Data Controller will not receive a warning email that data is going to be purged.</p></td>
</tr>
<tr class="odd">
<td><p>Data Classification</p></td>
<td><p>Displays the nature of the data in the table, identifying whether it contains personal data and so must be purged for regulatory compliance.</p>
<p>Options included with the DSP are:</p>
<ul>
<li><strong>Personal</strong> — This object contains data that must be purged by a certain date. The Retention Expiration Date field must be completed for this object (for example, Customer Addresses, Employee Records, Business Partner Tax IDs).</li>
<li><strong>Public</strong> —This object contains data that does not need to be purged (for example, Units of Measure, Material Descriptions, Country Codes).</li>
<li><strong>Restricted</strong> — This data does not need to be purged, but is marked as restricted access (for example, Company Chart of Accounts, Recipes, Work Orders).</li>
</ul>
<p><strong>NOTE:</strong> These options are delivered with the DSP and cannot be updated; however, a Common Administrator can create custom classifications on the Data Classification page in Common. Refer to <a href="../../Common/Use_Cases/Add%20Custom%20Data%20Classifications%20and%20Information%20Types.htm">Add Custom Data Classifications and Information Types</a> for more information.</p></td>
</tr>
<tr class="even">
<td><p>Retention Expiration Date</p></td>
<td><p>Displays the date when the data in the table will be automatically purged when a Service page runs.</p>
<p>A Collect Administrator must enter a date for a table with a data classification of Personal or for any custom classification with the Retention Period Warning feature enabled.</p>
<p>A different retention expiration date can be set at the target and target source level.</p>
<p>If no date is set for the object, the data is not purged.</p>
<p><strong>NOTE:</strong> Updates to this field are audited. An e-signature is required.</p>
<p><strong>NOTE:</strong> Once this data has passed, the Refresh and Build and Refresh icons on the <em><a href="Targets_H_Collect.htm">Targets</a></em>, <a href="Target_Sources_H_Collect.htm">Target Sources</a>, and this page are inactive. The table can no longer be refreshed either manually or automatically.</p></td>
</tr>
<tr class="odd">
<td><p>Data Collection Reason</p></td>
<td><p>Displays reason for extracting the data. Any time the table is processed, the data should only be used for the reason identified in this field.</p></td>
</tr>
</tbody>
</table>
