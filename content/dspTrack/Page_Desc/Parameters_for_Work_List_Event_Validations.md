# Parameters for Work List Event Validations

The validation can only use parameters that can be passed in from the
Work List.

The following parameters can be used in
validations.

|                   |                                                                                                            |
| ----------------- | ---------------------------------------------------------------------------------------------------------- |
| Parameters        | Descriptions                                                                                               |
| WorkListItemID    | The primary key in ttWorkList table.                                                                       |
| ItemReferenceID   | The primary key in ttProjectTask table.                                                                    |
| Name              | Task name entered on *PlanTask* page or *Work List Setup* page.                                            |
| Item Description  | Description entered on *PlanTask* page or *Work List Setup* page.                                          |
| PlannedStartDate  | Task's planned start date entered on the *Vertical* View of the *Work List Setup* or the *Plan Task* page. |
| PlannedFinishDate | Task's planned finish date entered on the *Vertical* View of the *Work List Setup* or the *PlanTask* page. |
| WebAppID          | ID for the task's WebApp (dspTrack™).                                                                      |
| ItemStatus        | Numeric representation of task status from ztTaskStatus table.                                             |
| boaUserID         | User ID who performed the action.                                                                          |
| Comment           | Comment entered on the *Vertical* View of the Work List or the *PlanTask* page.                            |
