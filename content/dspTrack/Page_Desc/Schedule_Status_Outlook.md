+++
title = 'Schedule Status Outlook'
solution = 'Platform'
+++

# Schedule Status Outlook

The Schedule Status Outlook can also affect the schedule status.

It can be set at the plan level on the *Plan* page’s *Vertical* View on
the Status Configuration tab or at the task level on the *Plan Task*
page’s *Vertical* View on the Additional Information tab.

Values are:

  - **Inherit** - A task’s schedule status settings are inherited from
    the plan level. This value is available at the plan task level only.
  - **Optimistic** - A task’s schedule status can improve. For example,
    a task passes the Post-Start Warn threshold and its Schedule Status
    icon is red. Work on the task begins. The Schedule Status icon for
    the task changes to green.
  - **Pessimistic** - A task’s schedule status cannot improve. The
    schedule status either does not change or becomes worse. For
    example, if work on a task has not started and the Pre Start Warn
    threshold has passed, the Schedule Status icon for that task is
    yellow. Depending on how work proceeds on the task, the task’s
    Schedule Status icon remains yellow or changes to red, but will
    never be green, even if the task is back on schedule.

**NOTE** The task’s schedule status can improve if the Status Outlook is
updated from pessimistic to optimistic.
