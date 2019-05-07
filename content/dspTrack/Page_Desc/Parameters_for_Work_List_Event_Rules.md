+++
title = 'Parameters for Work List Event Rules'
solution = 'Platform'
+++

# Parameters for Work List Event Rules

The Work List Event Rule Execution engine supports the following
parameters for use in the
rules:

|                   |                                                                                                            |
| ----------------- | ---------------------------------------------------------------------------------------------------------- |
| Parameter         | Description                                                                                                |
| WorkListItemID    | The primary key in ttWorkList table.                                                                       |
| ItemReferenceID   | The primary key in ttProjectTask table.                                                                    |
| Name              | Task name entered on *PlanTask* page or *Work List Setup* page.                                            |
| Item Description  | Description entered on *PlanTask* page or *Work List Setup* page.                                          |
| PlannedStartDate  | Task's planned start date entered on the *Vertical* View of the *Work List Setup* or the *PlanTask* page.  |
| PlannedFinishDate | Task's planned finish date entered on the *Vertical* View of the *Work List Setup* or the *PlanTask* page. |
| WebAppID          | ID for the task's WebApp (dspTrack™).                                                                      |
| ItemStatus        | Numeric representation of task status from ztTaskStatus table.                                             |
| boaUserID         | User ID who performed the action.                                                                          |
| Comment           | Comment entered on the *Vertical* View of the *Work List* or the *PlanTask* page.                          |
