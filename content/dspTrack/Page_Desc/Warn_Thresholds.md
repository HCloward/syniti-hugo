+++
title = 'Warn Thresholds'
solution = 'Platform'
+++

# Warn Thresholds

Thresholds can be set around the start or end of work on a task.

### Pre Start Warn and Post Start Warn Thresholds

If work has not started on a task (the task is in Ready or Waiting on
Dependency status), the Pre Start Warn Threshold marks the point in time
prior to the planned start date that the task’s schedule status is
behind and its Schedule Status icon becomes yellow.

If work on the task has not started, the Post Start Warn Threshold marks
the point in time after the planned start date that the task’s schedule
status is late and its Schedule Status icon becomes red.

  - **If the Pre Start Warn threshold is set to 0, and the Post Start
    Warn threshold is greater than 0,** dspTrack™ treats the planned
    start date as the Pre Start Warn threshold. Once the planned start
    date has passed, if work on a task has not started, the task’s
    schedule status is behind and its Schedule Status icon becomes
    yellow.

  - **If the Pre Start Warn threshold is greater than 0 and the Post
    Start Warn threshold is set to 0**, dspTrack™ treats the planned
    start date as the Post Start Warn threshold. When the Pre Start Warn
    date has passed, if work on a task has not started, the task will be
    behind and the Schedule Status icon displays as yellow. When the
    planned start date has passed, if work on the task has not started,
    the task will be late and the Schedule Status icon displays as red.

  - **If both Pre Start Warn and Post Start Warn thresholds are 0**,
    dspTrack™ will treat the planned start date as the Post Start Warn
    threshold.  If the planned start date passes and work on a task has
    not started, the task will move from an on-time status to a late
    status, and the Schedule Status icon will change from green to red.
    It will not display yellow.

### Pre End Warn and Post End Warn Thresholds

If work has started on a task (the task is in a status of In Progress),
the Pre End Warn Threshold sets the point in time prior to the planned
finish date that the task’s schedule status is behind and its Schedule
Status icon becomes yellow.

If work on the task has started (the task is in a status of In
Progress), the Post Start Warn Threshold sets the point in time after
the planned finish date that the task’s schedule status is late and its
Schedule Status icon becomes red.

  - **If the Pre End Warn threshold is set to 0, and the Post End Warn
    threshold is greater than 0,** dspTrack™ treats the planned finish
    date as the Pre End Warn threshold. Once the planned finish date has
    passed, if work on a task has not completed, the task’s schedule
    status is behind and its Schedule Status icon becomes yellow.

  - **If the Pre End Warn threshold is greater than 0 and the Post End
    Warn threshold is set to 0**, dspTrack™ will treat the planned
    finish date as the Post End Warn threshold. When the Pre End Warn
    date has passed, if work on a task has not started, the task will be
    behind and the Schedule Status icon displays as yellow. When the
    planned finish date has passed, if work on a task has not completed,
    the task will be late and the Schedule Status icon displays as red.

  - **If both Pre End Warn and Post End Warn thresholds are 0**,
    dspTrack™ will treat the planned finish date as the Post End Warn
    threshold.  If the planned finish date passes and work on a task has
    not finished, the task will move from an on-time status to a late
    status, and the Schedule Status icon will change from green to red.
    It will not display yellow.
