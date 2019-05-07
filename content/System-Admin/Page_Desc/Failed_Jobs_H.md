+++
title = ''
solution = 'Platform'
+++

# <span id="Failed_Jobs_H"></span>Failed Jobs H

[Failed Jobs V](#Failed_Jobs_V)

<div class="use">

Use this page to [View Failed Jobs](../Use_Cases/View_Failed_Jobs.htm).

</div>

To access this page:

1.  Click **Admin \> Resources \> Monitor** in the *Navigation* pane.
2.  Click the <span style="font-weight: bold;">Failed</span> icon for a
    resource type.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>JOB ID</p></td>
<td><p>Displays the services job number.</p></td>
</tr>
<tr class="odd">
<td><p>TASK ID</p></td>
<td><p>Displays the task ID.</p></td>
</tr>
<tr class="even">
<td><p>TYPE</p></td>
<td><p>Displays the type of job. The types are:</p>
<ul>
<li><p>Background Event – The job is in the background service controls job queue.</p></li>
<li><p>General – The job is in the General queue.</p></li>
<li><p>Index – The job is in the Index queue.</p></li>
<li><p>Service Page – The job is in the associated service page controls job queue.</p></li>
</ul></td>
</tr>
<tr class="odd">
<td><p>TITLE</p></td>
<td><p>Displays the title (or name) of the job.</p></td>
</tr>
<tr class="even">
<td><p>START TIME</p></td>
<td><p>Displays the date and time the job started.</p></td>
</tr>
<tr class="odd">
<td><p>END TIME</p></td>
<td><p>Displays the date and time the job ended.</p></td>
</tr>
<tr class="even">
<td><p>ACKNOWLEDGE</p></td>
<td><p>Click to acknowledge job failure.</p></td>
</tr>
</tbody>
</table>

## <span id="Failed_Jobs_V"></span>Failed Jobs V

[Failed Jobs H](#Failed_Jobs_H)

Field

Description

Job ID

Displays the services job number.

Job Information

Title

Displays the title (or name) of the job.

Job Type

Displays the type of job. The types are:

  - Background Event – The job is in the background service controls job
    queue.

  - General – The job is in the General queue.

  - Index – The job is in the Index queue.

  - Service Page – The job is in the associated service page controls
    job queue.

Parameters

Displays the parameter name and value of the job.

QUEUE

Displays the name of the Queue the job is in.

Tasks

Displays the tasks associated with the job.

Execution Results

Status

Displays the status of the job. Options are:

  - Ready – The job is awaiting processing.

  - Processing – The job is currently running.

  - Failed –The job has failed.

  - Executed – The job was successfully run.

Service Provider

Displays the name of the associated Windows Service.

Start Time

Displays the date and time the job started.

End Time

Displays the date and time the job ended.

MESSAGE

Displays error message received during job failure. May be used to
determine reason for failure.

Actions

Acknowledge

Click to acknowledge job failure.
