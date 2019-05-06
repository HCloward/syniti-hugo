# Calculate the Critical Path for a Plan

dspTrack™ uses a plan’s Critical Path (and other settings) to determine
a task’s schedule status. If a task is on the Critical Path and that
task is late, all subsequent tasks on the Critical Path will also be
late, even if work on these tasks has not yet started, or the planned
start date or planned finish date has not passed.

When a Microsoft Project file or an Excel file is imported into
dspTrack™, the schedule for that project is automatically calculated.
The schedule status for each task in the plan is set and any tasks
marked as on the Critical Path in Microsoft Project or the Excel file
are also marked as critical tasks in dspTrack™.

Refer to [Import Project Files into
dspTrack™](Import_Project_Files_into_dspTrack.htm) for more
information.

**NOTE:** A task cannot be added to the Critical Path from within
dspTrack™.

View a task’s schedule status on the Work List or the *Plan Task*
page.<span> </span> View whether a task is on the Critical Path on the
*Plan Task* page’s *Vertical* View on the Additional Information tab, or
on the *Work List Detail* page (Work List on the Quick Panel \> Work
List Detail).

The Critical Path can be calculated after the initial import if a
Microsoft Project file was imported into dspTrack™ to create the
project.<span> </span> When a user calculates the critical path
following the steps below, dspTrack™ determines which tasks are marked
as Critical in Microsoft Project and updates them accordingly in
dspTrack™.

<span style="font-weight: bold;">NOTE:</span> The Critical Path cannot
be calculated after the initial import if an Excel file was imported
into dspTrack™ to create the project. If the Project File Type is Excel
2007, the Calculate icon is disabled on the
<span style="font-style: italic;">Plan</span> page's
<span style="font-style: italic;">Vertical</span> View on the Action tab
after import.

<span style="font-weight: bold;">NOTE</span><span>: If a project was
created in dspTrack and is to be exported, it must be exported before
the critical path has been calculated (i.e., before the Calculate icon
is clicked on the Plan tab of the
</span><span style="font-style: italic;">Plan</span><span> page's
</span><span style="font-style: italic;">Vertical</span><span> View).
</span>

A user should calculate the Critical Path for a plan based on an
imported Microsoft Project files when:

Task dependencies in the plan change.

**NOTE**: Refer to [Use Dependency Types](Use_Dependency_Types.htm) for
more information.

Planned Finish Dates or Planned Start Dates are updated.

Warn Thresholds for schedule status calculation are updated.

**NOTE**: Refer to Set Parameters for  Schedule Status Calculation for
more information.

To calculate the Critical Path for a plan based on an imported Microsoft
Project file:

1.  Select **Project** in the *Navigation* pane.

2.  Click **Plans** for a project.

3.  Click **Vertical View** for a plan.

4.  Click the <span style="font-weight: bold;">Plan</span>tab.

5.  Click **Calculate**; a confirmation message displays.
    
    **NOTE:**This button is disabled if:
    
      - No tasks have been added to the plan
      - The tasks in this plan were added using an Excel import.

6.  Click **Ok**.

The Schedule Status icon may update on the Work List and the *Plan Task*
page depending on the results of the calculation.
