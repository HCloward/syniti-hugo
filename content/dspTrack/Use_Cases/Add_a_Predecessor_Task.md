+++
title = 'Add a Predecessor Task'
solution = 'Platform'
+++

# Add a Predecessor Task

When a project file is imported into dspTrack™, the predecessor tasks
and dependency types are also imported.

Refer to [Import Project Files into
dspTrack™](Import_Project_Files_into_dspTrack) for more
information.

A predecessor task can also be added manually.

If a task has a predecessor task, the dependency type determines when
work on the dependent task can begin (i.e., when the task will move from
Waiting on Dependency status to Ready status, so that a user can click
Next Action on the Work List to move the task to In Progress status).

Until the predecessor task is in the appropriate status based on the
dependency type, the dependent task will remain in Waiting on Dependency
status and work cannot start or finish for the dependent task. For
example, Task A has a predecessor that has not finished, with a
dependency of Finish to Finish. Work on Task A could start, but could
not finish until its predecessor task has finished. In this case, if a
user clicks Next Action on the Work List for a Plan task that is in
Waiting on Dependency status, an error message displays.

Refer to [Use Dependency Types](Use_Dependency_Types) for more
information.

To add a predecessor task to a Plan Task:

1.  Select **Project** from the Navigation pane.

2.  Click **Plans** for a project.

3.  Click **Tasks** for a plan.

4.  Click **Predecessor Tasks** for a task.
    
    **NOTE:** If no predecessor tasks exist for the task, the *Plan Task
    Dependency* page displays in add mode. Otherwise, click **Add**.
    
    [View the field descriptions for the Plan Task Dependency
    page](../Page_Desc/Plan_Task_Dependency)
    
    **NOTE:** By default DEPENDENCY TYPE ID list box defaults to
    FinishtoStart.

5.  Select a plan ID from the **PREDECESSOR PLAN ID** list box.
    
    **NOTE:** The plan’s that display are based on the logged in user’s
    security settings. Only plans that the logged in user can access
    display.

6.  Select a task ID from the **PREDECESSOR PLAN TASK ID** list box.

7.  Select a dependency type from the **DEPENDENCY TYPE ID** list box,
    if the default value is not correct. Options are StartToFinish,
    StartToStart, FinishToStart, and FinishToFinish.

8.  Enter a value in the **SLACK** field.
    
    **NOTE:** This number is used with the SLACK UOM to determine the
    amount of time that has to pass before a successor task can start or
    finish after its predecessor starts or finishes.

9.  Select an option in the **SLACK UOM** list box.
    
    **NOTE:** This Unit of Measure option is used with SLACK to
    determine the amount of time that has to pass before a successor
    task can start or finish after its predecessor starts or finishes.

10. Click **Save**.
