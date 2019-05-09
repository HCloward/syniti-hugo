+++
title = 'Error List in Metrics'
solution = 'Platform'
+++

# Error List in Metrics

<div class="use">

Use this page to view the Error List in Metrics report.

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Collect \> Reports</span> in
    the <span style="font-style: italic;">Navigation</span> pane.
2.  Click <span style="font-weight: bold;">Error List in Metrics</span>
    on the *[Reports](Reports)*
page.

| Field               | Description                                                                                                          |
| ------------------- | -------------------------------------------------------------------------------------------------------------------- |
| TARGET              | Displays the database target where tables are refreshed with source data.                                            |
| SOURCE              | Displays the database where the data is refreshed from and stored in the target.                                     |
| TABLE               | Displays the table name in the source database.                                                                      |
| PROCESS MESSAGE     | Displays the job processing message.                                                                                 |
| JOB ID              | Displays the number associated with the Platform job that ran the package that downloaded the table from the source. |
| EVENT               | Displays job failed events.                                                                                          |
| RECORD COUNT        | Displays the total number of records downloaded before the failure.                                                  |
| PROCESS STARTEDON   | Displays the date and time when the refresh started.                                                                 |
| PROCESS COMPLETEDON | Displays the date and time when the refresh completed.                                                               |
| DURATION            | Displays the amount of time (in seconds) the table took to download from the source.                                 |
| COUNTER             | Displays the log tracking sequence (primary key).                                                                    |
