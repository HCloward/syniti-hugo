# Use Dependency Types

When a project file is imported into dspTrack™, the predecessor tasks
and dependency types are also imported.

Refer to [Import Project Files into
dspTrack™](Import_Project_Files_into_dspTrack.htm) for more
information.

Use a dependency type (Start to Finish, Finish to Start, Finish to
Finish, or Start to Start) to set when work on a dependent Plan task can
start or finish based on when work on the predecessor task starts or
finishes.

**NOTE**: If a project is imported into dspTrack™, the dependency types
are automatically added in dspTrack™ and do not need to be set.

<span style="font-weight: bold;">NOTE</span>: If a project is imported
into dspTrack™, and the slack value is in the form of a percent in
Microsoft Project, that value will be displayed as number of days in the
Slack and Slack UOM fields on the <span style="font-style: italic;">Plan
Task Dependency</span> page.

Refer to [Add a Predecessor Task](Add_a_Predecessor_Task.htm) and
[Import Project Files into
dspTrack™](Import_Project_Files_into_dspTrack.htm) for more
information.

**NOTE**: Work List Items, added on the *Work List Setup* page, do not
have predecessor tasks and do not use dependency types.

A dependent task is in the status Waiting on Dependency on the Work List
until its predecessor task has started or finished based on the
dependency type. Once a predecessor task has started or finished, the
dependent task moves to Ready status on the Work List.

If a task on the Work List is in a status of Waiting on Dependency, when
the user clicks the Next Action button, the task(s) and the
dependency/dependencies that prevent the selected task from moving to
the next status display.

A Plan task has started when a user clicks the Next Action button on the
Work List to move the task status from Ready to In Process.

A Plan task has finished when a user clicks Next Action on the Work List
to move the task status from In Progress to Completed.<span> </span>

Until the predecessor task is in the appropriate status based on the
dependency type, the dependent task will remain in Waiting on Dependency
status and work cannot start or finish for the dependent task. For
example, Task A has a predecessor that has not finished, with a
dependency of Finish to Finish. Work on Task A could start, but could
not finish until its predecessor task has finished. In this case, if a
user clicks Next Action on the Work List for a Plan task that is in
Waiting on Dependency status, an error message displays.

Based on the dependency type, if<span> </span>work on a dependent task
begins late, the dependent task will show as late on the Work List. If
the dependent task is part of the critical path used by the Schedule
Status feature, the critical path will show as late.

Refer to [Calculate the Critical Path for a
Plan](Calculate_the_Critical_Path_for_a_Plan.htm) for more information.

There are four dependency types.

  - [Finish to Start](Finish_to_Start.htm)

  - [Start to Finish](Start_to_Finish.htm)

  - [Start to Start](Start_to_Start.htm)

  - [Finish to Finish](Finish_to_Finish.htm)
