# <span id="top"></span>Job Queue (Task) H

Job Queue (Task) V

<div class="use">

Use this page to view the tasks for failed jobs.

</div>

To access this page:

1.  Select **Admin \> Resources \> Jobs (Failed)** in the *Navigation*
    pane.
2.  Click **Vertical View** for a failed job.
3.  Click the **Tasks** button.

**NOTE:** This button only displays for General Job
Types.

| Field           | Description                                                                                                                      |
| :-------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| TASK ID         | Displays a unique identifier for the task in the queue.                                                                          |
| STATUS          | Displays the status of the task. Values are Ready, Failed or Completed.                                                          |
| TASK TYPE       | Displays whether the task is a stored procedure (SP), event or error.                                                            |
| TASK OBJECT     | Displays the name of the stored procedure, event or error (for example, webService\_UpdateStatusDeleteData).                     |
| TIMEOUT         | Displays the time (calculated from the START TIME to the END TIME) that a process can take to execute before it times out.       |
| MAXIMUM REPEATS | Displays the maximum number of times the task will run after timing out. The default is 0, meaning that the task only runs once. |
| RECORD COUNT    | Displays the number of records affected by the task’s processing.                                                                |
| START TIME      | Displays the time the task began processing.                                                                                     |
| END TIME        | Displays the time the task finished processing.                                                                                  |

## <span id="Job"></span>Job Queue (Task) V

Job Queue (Task) H

Field

Description

Task ID

Displays a unique identifier for the task in the queue.

Task Information

Task Type

Displays whether the task is a stored procedure (SP), event or error.

Task Object

Displays the name of the stored procedure, event or error (for example,
webService\_UpdateStatusDeleteData).

Timeout

Displays the time (from the START TIME to the END TIME) that a process
can take to execute before it times out.

Maximum Repeats

Displays the maximum number of times the task will run after timing out.
The default is 0, meaning that the task only runs once.

Execution Results

Status

Displays the status of the task. Values are Ready, Failed or Completed.

Start Time

Displays the time the task began processing.

End Time

Displays the time the task finished processing.

Record Count

Displays the number of records affected by the task’s processing.

Message

Displays the error message associated with the failure if the task
failed to process.

Search ID

Displays the Search ID for the failed event job. The search ID is the ID
of a predefined Search set. Search sets are defined in the Search menu
in the System Administration WebApp.

**NOTE:** This field only displays for Event Job Queue Tasks.

Page ID

Displays the Page ID, which allows auto-indexing the Primary key for
pages.

**NOTE:** This field only displays for Event Job Queue Tasks.

Queued Token

Displays a unique identifier created by a Stored Procedure in the
CranSoft database that assigns a random GUID.

**NOTE:** This field only displays for Event Job Queue Tasks.

DTS Server

This field is not used.

**NOTE:** This field only displays for Event Job Queue Tasks.

DTS Userid

This field is not used.

**NOTE:** This field only displays for Event Job Queue Tasks.

Package Password

This field is not used.

**NOTE:** This field only displays for Event Job Queue Tasks.

Delete DTS After Run

This field is not used.

**NOTE:** This field only displays for Event Job Queue Tasks.

Data Source ID

Displays the Primary key for the selected data source.

**NOTE:** This field only displays for Event Job Queue Tasks.
