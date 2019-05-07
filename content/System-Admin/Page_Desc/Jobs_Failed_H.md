+++
title = ''
solution = 'Platform'
+++

# <span id="Jobs__Failed__H"></span>Jobs (Failed) H

[Jobs (Failed) V](#Jobs__Failed__V)

<div class="use">

Use this page to:

  - [View Failed Jobs](../Use_Cases/View_Failed_Jobs.htm)
  - [Acknowledge Failed Jobs](../Use_Cases/Acknowledge_Failed_Jobs.htm)

</div>

To access this page:

Click the yellow Services icon on the Site toolbar.

OR

Click **Admin \> Resources \> Jobs (Failed)** in *Navigation*
pane.

|              |                                                                                                            |
| ------------ | ---------------------------------------------------------------------------------------------------------- |
| Field        | Description                                                                                                |
| JOB ID       | Displays the unique identifier for the failed job.                                                         |
| WEB APP NAME | Displays the name of the WebApp in which the job is executed.                                              |
| ADDED ON     | Displays the date and time the job was added to the job list.                                              |
| TYPE         | Displays the type of job. Options are: Background Event, General, Index and Service Page.                  |
| TITLE        | Displays the name of the queued job, e.g., the Event name from the page that queues the job.               |
| QUEUE NAME   | Displays the job queue a job has run on.                                                                   |
| START TIME   | Displays the time the job started to run.                                                                  |
| END TIME     | Displays the time the job stopped running.                                                                 |
| ACKNOWLEDGE  | Click to acknowledge that the failed job has been debugged and fixed; the record is removed from the page. |

## <span id="Jobs__Failed__V"></span>Jobs (Failed) V

[Jobs (Failed) H](#Jobs__Failed__H)

Field

Description

Job ID

Displays the unique identifier for the failed job.

Job Information

Job Type

Displays the type of job. Options are: Background Event, General, Index
and Service Page. This field is the same as the TYPE field on the
Horizontal View.

Web App

Displays the name of the WebApp where the job failed.

Page

Displays the name of the page within the WebApp where the job failed.

Parameters

Click to open the *[Job Queue Task Params](Job_Queue_Task_Params_H.htm)*
page to view the parameters that pass into the event. The parameters are
helpful when determining what record the event was running for, such as
a target table name or an assemble package name.

Event

Displays the name of the event that ran when the job failed.

QUEUE

Displays the name of the queue that processes the failed job. Options
are: Background Events, Indexing, Service Pages and General.

Execution Results

Status

Displays the status of the job. Since all records on the page are for
failed jobs, this field always says “Failed.”

Service Provider

Displays the name of the service that ran the job. Typically, there is
just one Service Provider for a site, but it is becoming common to have
two Service Providers set up.

Start Time

Displays the time the job started to run.

End Time

Displays the time the job stopped running.

Message

Displays a message returned from the logger.

Actions

Acknowledge

Click to acknowledge that the failed job has been debugged and fixed;
the record is removed from the page.

Tasks

Click to open the *[Job Queue (Task)](Job_Queue_Task.htm)* page to view
details about all tasks in the queue to troubleshoot a failed job.

**NOTE:** This button only displays for a job with a Type of General.
