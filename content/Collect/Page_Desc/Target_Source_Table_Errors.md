+++
title = 'Target Source Table Errors'
solution = 'Platform'
+++

# Target Source Table Errors

<div class="use">

Use this page to [View Collect
Reports](../Use_Cases/View_Collect_Reports.htm).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Collect \> Reports</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Target Source Table
    Errors</span> on the *[Reports](Reports.htm)*
page.

| Field                 | Description                                                                                                                                                                                |
| --------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| TARGET                | Displays the database target where the tables are refreshed with source data.                                                                                                              |
| SOURCE                | Displays the database where the data is refreshed from and stored in the target.                                                                                                           |
| TABLE                 | Displays the name of the table in the source database that caused the error.                                                                                                               |
| TABLE RENAME          | Displays the table name of the renamed table in the target database. The new table name must contain \[TableName\]. At run time, \[TableName\] is replaced with the processing table name. |
| REFRESH MESSAGE       | Displays the error message from the Platform job queue.                                                                                                                                    |
| DESCRIPTION           | Displays information about table, for example, the data contained within the table.                                                                                                        |
| ACTIVE                | If checked, the table is active. Only active tables are downloaded from the source during refresh. The default value is Active.                                                            |
| PACKAGE TYPE          | Displays the package type (to refresh target table with source data) for the erroneous table.                                                                                              |
| PACKAGE NAME          | Displays the name of the package that refreshes the target table with source data.                                                                                                         |
| POOLED TABLE NAME     | Displays the name of the SAP pooled table. Collect automatically changes the download RFC for pooled tables. Refer to SAP documentation for more information about pooled tables.          |
| WHERE CLAUSE OVERRIDE | Displays a Where Clause that is used to filter the data during a download.                                                                                                                 |
| JOB ID                | Displays the number associated with the Platform job that ran the package that downloaded the table from the source.                                                                       |
| RECORD COUNT          | Displays the number of records in the table of the target database at the time the table was refreshed by the source data.                                                                 |
| REFRESH STARTED ON    | Displays the date and time when the manual refresh started.                                                                                                                                |
| REFRESH COMPLETED ON  | Displays the date and time when the manual refresh completed.                                                                                                                              |
