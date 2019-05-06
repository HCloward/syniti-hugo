# Table Errors H

[Table Errors V (All Tabs](#Table_Errors_V_All_Tabs))

<div class="use">

Use this page to [view when an error occurred with table
downloads](../Use_Cases/View_Summary.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Summary \> Target
    Summary</span> in the Navigation pane.
2.  Click the <span style="font-weight: bold;">ERROR TABLES</span>
link.

|                 |                                                                                                                                                                                                  |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field           | Description                                                                                                                                                                                      |
| TABLE           | Displays table where error exists.                                                                                                                                                               |
| PACKAGE TYPE    | Displays package type (to refresh target table with source data) for erroneous table. Refer to [Package Types](../Use_Cases/Package_Types.htm) for a description of each package type available. |
| ACTIVE          | If enabled, table is active in source                                                                                                                                                            |
| DURATION        | Displays amount of time (in seconds) for table to be downloaded from source. If set to **-1**, the table failed to download.                                                                     |
| RECORD COUNT    | Displays number of records in the erroneous table.                                                                                                                                               |
| PACKAGE BUILT   | If enabled, package has been built for the erroneous table. This setting cannot be updated from within Collect.                                                                                  |
| REFRESH MESSAGE | Displays error message from the Platform job queue.                                                                                                                                              |
| RULES           | Click to open the <span style="font-style: italic;">[Table (Rule)](Table_Rule_H.htm)</span> page to add, edit and delete rules assigned to the erroneous table.                                  |
| INDICES         | Click to open the <span style="font-style: italic;">[Table (Indices)](Table_Indices_H.htm)</span> page to add, edit and delete indices assigned to the erroneous table.                          |

## <span id="Table_Errors_V_All_Tabs"></span>Table Errors V (All Tabs)

[Table Errors H](Table_Errors_H.htm)

<div class="use">

Use this page to [view when an error occurred with table
downloads](../Use_Cases/View_Summary.htm).

</div>

This page contains the following tabs:

  - [General tab](#General_Tab3)
  - [Advanced Settings tab](#Advanced_Settings_Tab3)
  - [General Information tab](#General_Information_Tab2)
  - [Action
tab](#Action_Tab3)

### <span id="General_Tab3"></span>General tab

|             |                                                                                                                     |
| ----------- | ------------------------------------------------------------------------------------------------------------------- |
| Field       | Description                                                                                                         |
| Table       | Displays erroneous table in the source database.                                                                    |
| Active      | If enabled, table is active. Only active tables are downloaded from source during refresh. Default value is Active. |
| Description | Displays information about table, e.g., data contained within table.                                                |

### <span id="Advanced_Settings_Tab3"></span>Advanced Settings tab

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
<td><p>Displays table name of renamed table in the target database. The new table name must contain [TableName]. At run time, [TableName] is replaced with the processing table name.</p></td>
</tr>
<tr class="odd">
<td><p>Where Clause Override</p></td>
<td><p>Displays a Where Clause that is used to limit data downloaded during the refresh process.</p></td>
</tr>
<tr class="even">
<td><p>Table Schema Owner</p></td>
<td><p>Displays the database’s schema for the table.</p></td>
</tr>
<tr class="odd">
<td><p>Next Schedule Run Date</p></td>
<td><p>Displays next date and time when the refresh process is scheduled to run.</p></td>
</tr>
<tr class="even">
<td><p>Package Type</p></td>
<td><p>Displays name of package that refreshes the target table with the source data.</p></td>
</tr>
<tr class="odd">
<td><p>Package Name</p></td>
<td><p>Displays name of package that refreshes the target table with the source data.</p>
<p><strong>NOTE:</strong> This field is displayed for the following package types:</p>
<ul>
<li>CranPort</li>
<li>ManualCranPort</li>
<li>Manual Data Services</li>
<li>SAP Data Services</li>
<li>ManualSSIS</li>
<li>BOA RFC</li>
<li>SAP RFC</li>
<li>SAP Data Services using RFC</li>
<li>SSIS</li>
</ul></td>
</tr>
<tr class="even">
<td><p>Schedule ID</p></td>
<td><p>Displays schedule for when target tables are refreshed with source data. Options are controlled in Common &gt; Configuration &gt; Schedules.</p></td>
</tr>
<tr class="odd">
<td><p>Schedule Group</p></td>
<td><p>Displays schedule to build packages, refresh or filter on tables in a group. Schedule Groups are managed in Configuration &gt; Schedule Groups.</p></td>
</tr>
<tr class="even">
<td><p>Schedule Single Thread</p></td>
<td><p>If enabled, table is downloaded from the source in a queue with all other single-threaded tables. Default value is Disabled.</p></td>
</tr>
<tr class="odd">
<td><p>Pooled Table Name</p></td>
<td><p>Displays name of SAP pooled table. Collect automatically changes the download RFC for pooled tables (i.e., SAP tables that store a list of tables, for example, ATAB stores 200 tables within a single table). Refer to SAP documentation for more information about pooled tables.</p></td>
</tr>
<tr class="even">
<td><p>RFC Records Per Call</p></td>
<td><p>Displays number of records returned in a single block for Collect background process to parse and insert into the database.</p></td>
</tr>
<tr class="odd">
<td><p>Encrypted Columns</p></td>
<td><p>Click to manage column encryption for the table.</p></td>
</tr>
</tbody>
</table>

### <span id="General_Information_Tab2"></span>General Information tab

|                      |                                                                                                                                                                                                                     |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field                | Description                                                                                                                                                                                                         |
| Job ID               | Displays the unique identifier associated with the Platform job that ran the package.                                                                                                                               |
| Refresh Completed On | Displays date and time when the manual refresh completed.                                                                                                                                                           |
| Record Count         | Displays number of records in the table of the target database at the time the table was refreshed by the source data.                                                                                              |
| Table Record Count   | Displays number of records currently in the target table. Ideally, this count is the same as Record Count.  If there is no primary key or unique index, this count may display zero, but the table could have data. |
| Duration             | Displays amount of time (in seconds) the table took to download from the source.                                                                                                                                    |
| Refresh Message      | Displays last process run against the table, e.g., build package, download or reset.                                                                                                                                |
| View Design          | Click to view additional details about the table.                                                                                                                                                                   |
| View Metrics         | Click to view and download metrics for table.                                                                                                                                                                       |
| View Job Tasks       | Click to view job tasks used to download table.                                                                                                                                                                     |

### <span id="Action_Tab3"></span>Action tab

|                |                                                                                                                                                                                                                                                                                                    |
| -------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field          | Description                                                                                                                                                                                                                                                                                        |
| Build Package  | Click to build a package to download active tables from the source.                                                                                                                                                                                                                                |
| Reset          | Click to reset the running refresh. Process activates the Refresh icon and triggers the batch job schedule to calculate new run dates for the next scheduled refresh. Reset doesn’t impact processes currently running. Reset the target if the download process backs up due to network problems. |
| Refresh        | Click to manually extract a copy of data from the source and load into the target.                                                                                                                                                                                                                 |
| Truncate Table | Click to delete all data in table. Table can then be deactivated if it is no longer required.                                                                                                                                                                                                      |
| Options        | Click to configure RFC options used by RFC download process. The Options icon is only active if Package Type = BOA RFC using Options.                                                                                                                                                              |
