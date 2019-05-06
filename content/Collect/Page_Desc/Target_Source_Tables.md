# Target Source Tables H

[Target Source Tables V (All Tabs)](#Target_Source_Tables_V__All_Tabs_)

<div class="use">

Use this page to [Build and Refresh Tables for a Schedule
Group](../Use_Cases/Build_and_Refresh_Tables_for_a_Schedule_Group.htm).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Collect \> Targets</span> in
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Sources</span> for target.
3.  Click <span style="font-weight: bold;">Tables</span> for source.
4.  Click the <span style="font-weight: bold;">Tables</span> icon for a
    schedule group.

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
<td><p>Build And Refresh</p></td>
<td><p>Click to build the package and download active tables from the source. If the package already exists, the table is refreshed (i.e., data is downloaded from the source database). If the package does not exist, a package is immediately scheduled to be built and the table is refreshed. The Refresh icon is disabled for DBMoto® package types because the refresh is run by DBMoto® instead of by Collect.</p></td>
</tr>
<tr class="odd">
<td><p>Reset</p></td>
<td><p>Click to reset a running refresh. This process activates the Refresh icon and triggers batch job schedule to calculate new run dates for next scheduled refresh. Reset source if the download process backs up due to network problems.</p></td>
</tr>
<tr class="even">
<td><p>Build Package</p></td>
<td><p>Click to build a package to download active tables from the source.</p></td>
</tr>
<tr class="odd">
<td><p>Refresh</p></td>
<td><p>Click to manually extract a copy of data from the source and load into the target.</p></td>
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
<p><strong>NOTE:</strong> When the package type is CranPort package, the package name is hyperlinked to the CranPort package in Assemble in the view.</p>
<p><strong>NOTE:</strong> If source has an SAPAPPSERVER connection type, only the following RFC package types are available in the Package Type list box:</p>
<ul>
<li><p>BOA RFC</p></li>
<li><p>SAP Data Services using RFC</p></li>
<li><p>SAP RFC</p></li>
<li><p>SAP Text</p></li>
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

## <span id="Target_Source_Tables_V__All_Tabs_"></span>Target Source Tables V (All Tabs)

[Target Source Tables H](Target_Source_Tables.htm)

This page contains the following tabs:

  - [General tab](#General_Tab)
  - [Advanced Settings tab](#Advanced_Settings_Tab)
  - [General Information tab](#General_Information_Tab)
  - [Action
tab](#Action_Tab)

## <span id="General_Tab"></span>General tab

|               |                                                                                                                                                                                                                                         |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field         | Description                                                                                                                                                                                                                             |
| Build Package | Click to build a package to download active tables from the source.                                                                                                                                                                     |
| Reset         | Click to reset a running refresh. This process activates the Refresh icon and triggers batch job schedule to calculate new run dates for next scheduled refresh. Reset source if the download process backs up due to network problems. |
| Refresh       | Click to manually extract a copy of data from the source and load into the target.                                                                                                                                                      |
| Target        | Displays the target database where tables are refreshed with source data.                                                                                                                                                               |
| Source        | Displays the database where data is refreshed from and stored in the target.                                                                                                                                                            |
| Table         | Displays table in the source database.                                                                                                                                                                                                  |
| Active        | If enabled, table is active. Only active tables are downloaded from the source during refresh. Default value is Active.                                                                                                                 |
| Description   | Displays information about table, e.g., data contained within table.                                                                                                                                                                    |

## <span id="Advanced_Settings_Tab"></span>Advanced Settings tab

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
<td><p>Table Rename</p></td>
<td><p>Displays the table name of the renamed table in target database. New table name must contain [TableName]. At run time, [TableName] is replaced with processing table name.</p></td>
</tr>
<tr class="odd">
<td><p>Where Clause Override</p></td>
<td><p>Displays a Where Clause that is used to limit data downloaded during a refresh process.</p></td>
</tr>
<tr class="even">
<td><p>Table Schema Owner</p></td>
<td><p>Displays the database’s schema for the table.</p></td>
</tr>
<tr class="odd">
<td><p>NextRun</p></td>
<td><p>Displays next date and time when the refresh process is scheduled to run.</p></td>
</tr>
<tr class="even">
<td><p>Package Type</p></td>
<td><p>Displays package type to refresh the target table with source data. Default value is <strong>CranPort</strong>.</p></td>
</tr>
<tr class="odd">
<td><p>Package Name</p></td>
<td><p>Displays name of package that refreshes target table with source data.</p>
<p><strong>NOTE:</strong> The package name is set automatically and displays after the package is built for the package types CranPort, SSIS, or Data Services. The package must be manually built and the package name must be entered into Collect for package types ManualCranPort, ManualSSIS or Manual Data Services.</p>
<p><strong>NOTE:</strong> The package name must follow the naming convention #Database#%#Source#%. Refer to <a href="../../Assemble/Create_Packages.htm">Create Packages</a> for more information.</p>
<p><strong>NOTE:</strong> For Manual Data Services package types, the default package name can be accepted, or it can be edited as needed</p></td>
</tr>
<tr class="even">
<td><p>Schedule ID</p></td>
<td><p>Displays schedule for when target tables are refreshed with source data. Options are controlled in Common &gt; Configuration &gt; Schedules. Default value is <strong>Use Source Schedule setting. No Table Override Requested</strong>.</p></td>
</tr>
<tr class="odd">
<td><p>Schedule Group</p></td>
<td><p>Displays schedule to build packages, refresh or filter on tables in a group. Schedule Groups are managed in Configuration &gt; Schedule Groups. Default value is <strong>No Group</strong>.</p>
<p><strong>NOTE: </strong> If building a group with a DBMoto® package the following applies<br />
If Schedule Group is set to NO GROUP, both Download and Mirror package will be built as an individual replication in DBMoto®. <br />
If Schedule Group is set to AUTO and if it is a Download package, the replication will be part of a group named &lt;GroupPrefix&gt;_Downloads. Otherwise, if it is a Mirror package the replication will be part of a group called &lt;GroupPrefix&gt;_&lt;number&gt; where number is an incremental value to count the number of groups. Groups cannot contain more than &lt;Group_Size&gt; replications. <br />
If Schedule Group is set to &quot;existing group name&quot; with no restriction to the &lt;Group_Size&gt; parameter the replication is built into that group. </p>
<p><strong>NOTE:</strong> The Replication Mode must be consistent with the Replication Group Mode (e.g a download package cannot be grouped with a mirror package).  </p></td>
</tr>
<tr class="even">
<td><p>Schedule Single Thread</p></td>
<td><p>If enabled, table is downloaded from the source in a queue with all other single-threaded tables. Default value is <span style="font-weight: bold;">Disabled</span>.</p></td>
</tr>
<tr class="odd">
<td><p>Pooled Table Name</p></td>
<td><p>Displays name of SAP pooled table. Collect automatically changes the download RFC for pooled tables (i.e., SAP tables that store a list of tables, for example, ATAB stores 200 tables within a single table). Refer to SAP documentation for more information about pooled tables.</p></td>
</tr>
<tr class="even">
<td><p>Rfc Records Per Call</p></td>
<td><p>Displays number of records returned in a single block for Collect background process to parse and insert into database. Default value is <strong>5000</strong>.</p></td>
</tr>
<tr class="odd">
<td><p>Encrypted Columns</p></td>
<td><p>Click to open the <span style="font-style: italic;">Target Source Table Column Encryption</span>page to edit column encryption for the table.</p></td>
</tr>
</tbody>
</table>

### <span id="General_Information_Tab"></span>General Information tab

|                    |                                                                                                                                                                                                             |
| ------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field              | Description                                                                                                                                                                                                 |
| Job ID             | Displays unique identifier of with the Platform job that ran the package.                                                                                                                                   |
| Completed          | Displays date and time when manual refresh completed.                                                                                                                                                       |
| Record Count       | Displays number of records in the table. This field is protected and updated by Collect when the table refresh process completes.                                                                           |
| Table Record Count | Displays number of records currently in the table. Ideally, this count is the same as Record Count.  If there is no primary key or unique index, this count may display zero but the table could have data. |
| Duration           | Displays amount of time (in seconds) the table took to download from the source during the refresh process.                                                                                                 |
| Refresh Message    | Displays last process that ran against table, e.g., build package, download or reset.                                                                                                                       |
| View Design        | Click to open the <span style="font-style: italic;">[Data Source Tables](Data_Source_Tables_H.htm)</span> page to view, edit and delete details about the table.                                            |
| View Metrics       | Click to open the <span style="font-style: italic;">[Download Metrics](../Use_Cases/Download_Metrics.htm)</span> page to view and download metrics for table.                                               |
| View Job Tasks     | Click to open the <span style="font-style: italic;">[Table Download Task List](Table_Download_Task_List.htm)</span> page to view job tasks used to download table.                                          |

## <span id="Action_Tab"></span>Action tab

|                |                                                                                                                                                                                                                                       |
| -------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field          | Description                                                                                                                                                                                                                           |
| Truncate Table | Click to delete all data in the table. Table can then be deactivated if it is no longer required.                                                                                                                                     |
| Options        | Click to open the <span style="font-style: italic;">[Table (Rfc Options)](Table_Rfc_Options.htm)</span> page to configure RFC options used by RFC download process. The icon  is only active if Package Type = BOA RFC using Options. |
