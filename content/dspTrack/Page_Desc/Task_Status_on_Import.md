# Task Status on Import

When a project file is imported, dspTrack™ analyzes data for each task
and sets the Task Status. Every task must be assigned a Task Status.

dspTrack™ assigns a task a Waiting on Dependency status if any of the
task’s predecessor tasks are not complete and the dependency type is
Finish to Start.

dspTrack™ assigns a task a Completed status if the task has valid values
for its Actual Start Date and Actual Finish Date.

dspTrack™ assigns a task an In Progress status if the task has a valid
Actual Start Date and the Actual Finish Date is NULL.

All other tasks are assigned a status of Ready.
