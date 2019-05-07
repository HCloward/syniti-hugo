+++
title = 'Duration Warning List'
solution = 'Platform'
+++

# Duration Warning List

<div class="use">

Use this page to view the Duration Warning List report.

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Collect \> Reports</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Duration Warning List</span>
    on the *[Reports](Reports.htm)*
page.

| Field                  | Description                                                                                                                                                                                |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| DURATION TIME          | Displays the amount of time (in seconds) the table took to download from the source.                                                                                                       |
| TARGET                 | Displays the database target where the tables are refreshed with source data.                                                                                                              |
| SOURCE                 | Displays the database where the data is refreshed from and stored in the target.                                                                                                           |
| TABLE                  | Displays the table name in the source database.                                                                                                                                            |
| TABLE RENAME           | Displays the table name of the renamed table in the target database. The new table name must contain \[TableName\]. At run time, \[TableName\] is replaced with the processing table name. |
| JOB ID                 | Displays the number associated with the Platform job that ran the package that downloaded the table from the source.                                                                       |
| RECORD COUNT           | Displays the number of records in the table being reported.                                                                                                                                |
| STARTED ON             | Displays the date and time the refresh started.                                                                                                                                            |
| COMPLETED ON           | Displays the date and time the refresh completed.                                                                                                                                          |
| PACKAGE TYPE           | Displays the package type (to refresh target table with source data) for the erroneous table.                                                                                              |
| PACKAGE NAME           | Displays the name of the package that refreshes the target table with the source data.                                                                                                     |
| POOLED TABLE NAME      | Displays the name of the SAP pooled table. Collect automatically changes the download RFC for pooled tables. Refer to SAP documentation for more information about pooled tables.          |
| DURATION WARNING LIMIT | Displays the limit (in seconds) for long-running tables.                                                                                                                                   |
| DURATION               | Displays the amount of time (in seconds) the table took to download from the source.                                                                                                       |
