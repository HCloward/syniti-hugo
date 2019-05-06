# Table List in Source and Target

<div class="use">

Use this page to view the Table List in Source and Target report.

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Collect \> Reports</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;"> List in Source and
    Target</span> on the *[Reports](Reports.htm)*
page.

| Field                | Description                                                                                                                                                                                |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| TABLE                | Displays the database target where the tables are refreshed with source data.                                                                                                              |
| SOURCE               | Displays the database where the data is refreshed from and stored in the target.                                                                                                           |
| TARGET               | Displays the database target where tables are refreshed with source data.                                                                                                                  |
| DESCRIPTION          | Displays information about the table, for example, the data contained within table.                                                                                                        |
| TABLE RENAME         | Displays the table name of the renamed table in the target database. The new table name must contain \[TableName\]. At run time, \[TableName\] is replaced with the processing table name. |
| ACTIVE               | If checked, the table is active in the source and the data can be downloaded. If unchecked, no data will be downloaded for this table.                                                     |
| PACKAGE TYPE         | Displays the package type (to refresh the target table with source data) for the table.                                                                                                    |
| POOLED TABLE NAME    | Displays the name of the SAP pooled table. Collect automatically changes the download RFC for pooled tables. Refer to SAP documentation for more information about pooled tables.          |
| DURATION             | Displays the amount of time (in seconds) the table took to download from the source.                                                                                                       |
| RECORD COUNT         | Displays the number of records in the table of the target database at the time the table was refreshed by source data.                                                                     |
| REFRESH MESSAGE      | Displays the error message from the Platform job queue.                                                                                                                                    |
| REFRESH COMPLETED ON | Displays the date and time when the manual refresh completed.                                                                                                                              |
