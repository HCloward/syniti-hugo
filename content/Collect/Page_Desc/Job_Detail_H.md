+++
title = 'Job Detail H'
solution = 'Platform'
+++

# Job Detail H

[Job Detail V](#Job_Detail_V)

<div class="use">

Use this page to [View Summary](../Use_Cases/View_Summary).

</div>

To access this page:

1.  Select <span style="font-weight: bold;">Collect \> Summary</span> on
    <span style="font-style: italic;">Navigation</span> pane.
2.  Click
<span style="font-weight: bold;">Records</span>.

|            |                                                                                                       |
| ---------- | ----------------------------------------------------------------------------------------------------- |
| Field      | Description                                                                                           |
| MONITOR ID | Displays the unique identifier for monitoring record.                                                 |
| STATUS     | Displays current status of the monitored job.                                                         |
| MESSAGE    | Displays message returned when the job completed.                                                     |
| TARGET     | Displays target database (where tables are refreshed with source data) impacted by the job.           |
| SOURCE     | Displays source database (where data is refreshed from and stored in the target) impacted by the job. |
| TABLE      | Displays table impacted by the job.                                                                   |
| JOB TYPE   | Displays type of job performed on table.                                                              |

## <span id="Job_Detail_V"></span>Job Detail V

[Job Detail H](Job_Detail_H)

<div class="use">

Use this page to [View Summary](../Use_Cases/View_Summary).

</div>

Field

Description

General

Monitor ID

Displays unique identifier of the monitoring record.

Status

Displays current status of the job.

Message

Displays message returned when job completed.

Target

Displays target database (where tables are refreshed with source data)
impacted by the job.

Source

Displays source database (where data is refreshed from and stored in the
target) impacted by the job.

Table

Displays table impacted by the job.

Job Information

Job Type

Displays type of job performed on table.

Job ID

Displays unique identifier associated with the job.

Additional Information

Function Name

Displays procedure that created the monitoring record.

Index

Displays table index impacted by the job. Field is blank if there is no
index. Indices are defined at Target \> Source \> Table \> Indices.

Added By

Displays user ID who started the job that added the monitoring record
(i.e., whoever ran the event).

Added On

Displays date and time when job that added the monitoring record was
started (i.e., when the event was run).
