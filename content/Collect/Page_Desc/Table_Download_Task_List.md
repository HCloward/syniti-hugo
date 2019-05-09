+++
title = 'Table Download Task List'
solution = 'Platform'
+++

# Table Download Task List

<div class="use">

Use this page to [Monitor Table Download
Process](../Use_Cases/Monitor_Table_Download_Process).

</div>

To access this page:

1.  Click <span style="font-weight: bold;">Collect \> Tables</span> in
    the Navigation pane.
2.  Build the download package for the table by either clicking
    <span style="font-weight: bold;">Build and Refresh</span> or
    <span style="font-weight: bold;">Build Package</span> on the Page
    toolbar.
3.  Click <span style="font-weight: bold;">Vertical View</span> for the
    table.
4.  Click <span style="font-weight: bold;">General Information</span>
    tab.
5.  Click <span style="font-weight: bold;">View Job
Tasks</span>.

|              |                                                                                                                    |
| ------------ | ------------------------------------------------------------------------------------------------------------------ |
| Field        | Description                                                                                                        |
| JOB ID       | Displays the unique identifier associated with the job that ran the package.                                       |
| TASK ID      | Displays the ID of a task within the job.                                                                          |
| STATUS       | Displays current status of the task.                                                                               |
| TASK TYPE    | Displays type of task within the job.                                                                              |
| TASK OBJECT  | Displays task in the job (usually a stored procedure or a Platform event).                                         |
| MESSAGE      | Displays message returned by task. This field is usually only populated with error message.                        |
| RECORD COUNT | Displays number of records in the table of the target database at the time the table was refreshed by source data. |
| START TIME   | Displays time task started.                                                                                        |
| END TIME     | Displays time task ended.                                                                                          |
