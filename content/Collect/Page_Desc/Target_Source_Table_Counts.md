+++
title = 'Target Source Table Counts'
solution = 'Platform'
+++

# Target Source Table Counts

<div class="use">

Use this page to view the Target Source Table Counts report.

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Collect \> Reports</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Target Source Table
    Counts</span> on the *[Reports](Reports)*
page.

| Field           | Description                                                                                                                                                                                |
| --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| TARGET          | Displays the database target where the tables are refreshed with source data.                                                                                                              |
| SOURCE          | Displays the database where the data is refreshed from and stored in the target.                                                                                                           |
| TABLE           | Displays the name of the table in the source database.                                                                                                                                     |
| TABLE RENAME    | Displays the table name of the renamed table in the target database. The new table name must contain \[TableName\]. At run time, \[TableName\] is replaced with the processing table name. |
| DURATION        | Displays the amount of time (in seconds) the table took to download from the source.                                                                                                       |
| RECORD COUNT    | Displays the number of records in the table of the target database at the time the table was refreshed by the source data.                                                                 |
| REFRESH MESSAGE | Displays the error message from the Platform job queue.                                                                                                                                    |
