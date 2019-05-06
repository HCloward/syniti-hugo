# Task Status

When a project file is imported, dspTrack™ sets task status. Refer to
[Task Status on Import](Task_Status_on_Import.htm) for more information.

Work on a plan task or Work List Item can be tracked using the task
status. dspTrack™ uses the following statuses.

  - Ready
  - Waiting on Dependency
  - In Progress
  - Completed

These statuses display on the Work List,
<span style="font-style: italic;">Plan</span>*Task* and *Work List
Setup* pages.

## Ready

A task is in Ready status when:

  - It has been created and has no predecessor tasks or
  - All the predecessor tasks assigned to the task have a status of
    Completed.

When a user clicks Next Action on the Work List, a task that is in Ready
status moves to In Progress.

## Waiting on Dependency

A dependent task is in the status Waiting on Dependency on the Work List
until its predecessor task has started or finished based on the
dependency type. Once a predecessor task has started or finished, the
dependent task moves to Ready status on the Work List.

<span style="font-weight: bold;">NOTE</span>: A task in Waiting on
Dependency <span> </span>status must have at least one user assigned.

If a user clicks Next Action on the Work List for a task that is in
Waiting on Dependency status, dspTrack™ displays the task(s) and the
dependency/dependencies that prevent the selected task from moving to
the next status.

If a task has a predecessor task, the dependency type determines when
work on the dependent task can begin (i.e., when the task will move to
Ready status, so that a user can click Next Action on the Work List to
move the task to In Progress status). For example, Task A has a
predecessor that has not finished, with a dependency of Finish to
Finish. Work on Task A could start, but could not finish until its
predecessor task has finished. In this case, if a user clicks Next
Action on the Work List for a Plan task that is in Waiting on Dependency
status, an error message displays. Refer to [Use Dependency
Types](../Use_Cases/Use_Dependency_Types.htm) for more information.

**NOTE**: Work List Items, added on the Work List Setup page, do not
have predecessor tasks. They do not have dependencies so will not be
assigned a Waiting on Dependency status.

## In Progress

A task is in this status when it is being worked.

When a user clicks Next Action on the Work List for a task in this
status, a task that is in In Progress moves to Completed, and the Actual
Finish Date for the task is updated to the current date. If this is the
final task to be completed in the project, the Actual Finish Date in the
project is also updated with the current date.

A task that is in In Progress cannot be edited, except that users can be
added or removed from the task. However, all users cannot be removed
from an In Progress task, at least one user must be assigned to it.

## Completed

A Plan Task or Work List Item in this status no longer displays on the
Work List. Plan Tasks in Completed status display on the
*<span>Plan</span>Task* page and the *<span>Work List Detail</span>*
page. Work List Items in Completed status display on the *<span>Work
List Detail</span>* page only.
