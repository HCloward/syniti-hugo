+++
title = 'Monitor (Downloads) H'
solution = 'Platform'
+++

# Monitor (Downloads) H

[Monitor (Downloads) V](#Monitor_Downloads_V)

<div class="use">

Use this page to:

  - [Monitor table refresh activity](../Use_Cases/View_Summary.htm)
  - [View Summary](../Use_Cases/View_Summary.htm)

</div>

To access this page:

1.  Select<span style="font-weight: bold;"> Collect \> Summary \> Target
    Summary</span> in the Navigation pane.
2.  Click the <span style="font-weight: bold;">Refreshing Tables</span>
    link for the table that is currently being
refreshed.

|                    |                                                                                                                                                                                                |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Field              | Description                                                                                                                                                                                    |
| JOB ID             | Displays the identifier associated with the job that refreshed the tables.                                                                                                                     |
| STATUS             | Displays current status of the refresh job.                                                                                                                                                    |
| TARGET             | Displays the target database where tables are refreshed with source data impacted by the job. Click link open the <span style="font-style: italic;">Targets</span>page to view target details. |
| SOURCE             | Displays source database where data is refreshed from and stored in the target. Click link to open the <span style="font-style: italic;">Target Sources</span>page to view source details.     |
| TABLE              | Displays target table being refreshed with source data. Click link to open the <span style="font-style: italic;">Tables</span>page to view table details.                                      |
| REFRESH STARTED ON | Displays date and time when manual refresh started.                                                                                                                                            |
| PROCESSING COUNT   | Displays how many tables are either downloading or are queued to be downloaded.                                                                                                                |
| SCHEDULE GROUP     | Displays schedule to build packages, refresh or filter on tables in a group. Schedule Groups are managed in Configuration \> Schedule Groups.                                                  |
| Tasks              | Click to open the <span style="font-style: italic;">Table Download Task List</span>page to view list of tasks within the job.                                                                  |
| Reset              | Click to stop job; this process resets the table.                                                                                                                                              |
| Hold               | Click to pause the download process for this table.                                                                                                                                            |
| Release            | Click to release the pause on the table being downloaded, resuming the table download process.                                                                                                 |

## <span id="Monitor_Downloads_V"></span>Monitor (Downloads) V

[Monitor (Downloads) H](Monitor_Downloads_H.htm)

<div class="use">

Use this page to:

  - [Monitor table refresh activity](../Use_Cases/View_Summary.htm)
  - [View
Summary](../Use_Cases/View_Summary.htm)

</div>

|                        |                                                                                                                                                                                                        |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Field                  | Description                                                                                                                                                                                            |
| Job ID                 | Displays identifier associated with the job that refreshed the tables                                                                                                                                  |
| Target                 | Displays target database where tables are refreshed with source data impacted by the job. Click link to view target details.                                                                           |
| Source                 | Displays source database where data is refreshed from and stored in the target. Click link to view source details.                                                                                     |
| Table                  | Displays target table being refreshed with source data. Click link to view table details.                                                                                                              |
| Table Rename           | Displays table name of renamed table in target database. New table name must contain \[TableName\]. At run time, \[TableName\] is replaced with processing table name.                                 |
| Refresh Started On     | Displays date and time when manual refresh started.                                                                                                                                                    |
| Processing Count       | Displays how many tables are either downloading or are queued to be downloaded.                                                                                                                        |
| Scheduled By           | Displays user ID of individual who started the table refresh process.                                                                                                                                  |
| Description            | Displays a brief description of the table being refreshed.                                                                                                                                             |
| Schedule Group         | Displays schedule to build packages, refresh or filter on tables in a group. Schedule Groups are managed in Configuration \> Schedule Groups.                                                          |
| Schedule Single Thread | If enabled, table is downloaded from source in a queue with all other single-threaded tables.                                                                                                          |
| Package Type           | Displays package type (to refresh target table with source data) for erroneous table.                                                                                                                  |
| Package Name           | Displays package type to refresh target table with source data.                                                                                                                                        |
| Tasks                  | Click to open the <span style="font-style: italic;">Table Download Task List</span><span>page to</span> view list of tasks within the job.                                                             |
| Hold All               | Click to stop the download process for all running tables in Collect. This icon is disabled until the target download process begins.                                                                  |
| Hold Target            | Click to pause the download process for all running tables in the target. This icon is disabled until the target download process begins.                                                              |
| Hold Group             | Click to pause the download process for all running tables in the group. This icon is disabled until the target download process begins.                                                               |
| Release All            | Click to release the pause on all tables being downloaded, resuming the table download process. This icon is enabled if the Hold All icon has been clicked, initiating the pause.                      |
| Release Target         | Click to release the pause on all tables within the target being downloaded, resuming the table download process. This icon is enabled if the Hold Target icon has been clicked, initiating the pause. |
| Release Group          | Click to release the pause on all tables within the group being downloaded, resuming the table download process. This icon is enabled if the Hold Group icon has been clicked, initiating the pause.   |
| Reset                  | Click to reset the table so it can be downloaded again. This process is helpful if the system crashed during the table download process.                                                               |
