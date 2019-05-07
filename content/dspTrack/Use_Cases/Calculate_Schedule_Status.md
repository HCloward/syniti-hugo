+++
title = 'Calculate Schedule Status'
solution = 'Platform'
+++

# Calculate Schedule Status

The Schedule Status for a task indicates whether a task is on time,
behind or late.<span> </span>

Using Warn Thresholds, dspTrack™ can give users a nuanced understanding
of a task’s schedule status so that resources can be allocated or a
project plan can be updated before the plan becomes late.

These thresholds are set at the plan level and expressed as percentages
of the entire duration of a task.

Schedule status displays for tasks on the Work List and the *Plan Task*
page. Schedule status is calculated for tasks in both active and
inactive plans.

The Schedule Status icon is a circle that displays in a color that
indicates the task’s schedule status. A green icon means the task is on
time according to the project plan. A yellow icon indicates the task is
behind. A red icon indicates the task is late.

**NOTE**: Work List items added on the *Work List Setup* page are not
associated with projects or plans, and the schedule status is calculated
based on the planned finish date. A Work List item’s schedule status is
green until the current date is later than the planned finish date, at
which point the schedule status is red. It does not turn yellow.

The schedule status is calculated using:

  - [Warn Thresholds](../Page_Desc/Warn_Thresholds.htm)
  - [Schedule Status Outlook](../Page_Desc/Schedule_Status_Outlook.htm)
  - [The Critical Path](Tasks_on_the_Critical_Path.htm)
  - The Current Date/Time

Refer to [Set Parameters for Schedule Status
Calculation](Set_Parameters_for_Schedule_Status_Calculation.htm).
