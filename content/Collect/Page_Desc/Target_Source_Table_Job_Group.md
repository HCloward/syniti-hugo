# Target Source Table Job Group

<div class="use">

Use this page to view the Target Source Table Job Group report.

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Collect \> Reports</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Target Source Table Job
    Group</span> on the *[Reports](Reports.htm)*
page.

| Field                  | Description                                                                                                                                                                                |
| ---------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| SCHEDULE GROUP         | Displays the unique name of the schedule group.                                                                                                                                            |
| TARGET                 | Displays the database target that contains the table in the schedule group.                                                                                                                |
| SCHEDULE SINGLE THREAD | If checked, table is downloaded from source in a queue with all other single-threaded tables.                                                                                              |
| SOURCE                 | Displays the database where the data is refreshed from and stored in the target.                                                                                                           |
| TABLE                  | Displays the name of the table in the source database that is in the schedule group.                                                                                                       |
| TABLE RENAME           | Displays the table name of the renamed table in the target database. The new table name must contain \[TableName\]. At run time, \[TableName\] is replaced with the processing table name. |
| ACTIVE                 | If checked, the table is active. Only active tables are downloaded from the source during refresh.                                                                                         |
