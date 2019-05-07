+++
title = 'Export a Project File'
solution = 'Platform'
+++

# Export a Project File

Export a project to make updates to the project in MS Project, then
import the plan to dspTrack™ to update the project data.

Refer to [Import Project Files into
dspTrack™](Import_Project_Files_into_dspTrack.htm) for more
information.

A project can be exported from dspTrack™ in the form of an Excel file
(with an .xlsx extension) or an MS Project 2012 project (with an .mpp
extension).

**NOTE**: A plan must have a Project File Type set to use export
functionality. If a plan was created in dspTrack™ and not based on a
project import, set the plan’s Project File Type to Excel 2007 or MS
Project prior to export.

**NOTE**: Once a Project File Type has been set if a project file is
imported, the Project File Type cannot be changed for the plan. For
example, a user creates a plan with a Project File Type of Excel 2007
and then imports an Excel file. The user then changes the Project File
Type to MSProject 2012 on the *Plan* page’s *Vertical* View on the
General tab. The user attempts to export the project file from
dspTrack™. An error message displays and the export does not proceed.

<span style="font-size: 11.0pt;">**NOTE**: When a project with a Project
File Type of MS Project
</span><span> </span><span style="font-size: 11.0pt;">is created in
dspTrack™ and then exported, the project’s calendar, work days and work
hours are also exported.</span><span> </span>

<span style="font-weight: bold;">NOTE</span>: If a project was created
in dspTrack and is to be exported, it must be exported before the
critical path has been calculated (i.e., before the Calculate icon is
clicked on the Plan tab of the
<span style="font-style: italic;">Plan</span> page's
<span style="font-style: italic;">Vertical</span> View).

To export a file:

1.  Click **Project** in Navigation pane.

2.  Click <span style="font-weight: bold;">Plans</span> for a project.

3.  Click **Vertical View** for a plan.

4.  Click <span style="font-weight: bold;">Plan</span>tab.

5.  Click **Export**; a confirmation message displays.

6.  Click **Ok**.
    
    <span style="font-weight: bold;">NOTE</span>: If there are no tasks
    in the plan, the Export button is disabled.

7.  Click <span style="font-weight: bold;">Plan</span> tab.

8.  Click **Download a file** next to
    <span style="font-weight: bold;">Upload</span>.

9.  Save the file.

The file exports in the selected Project File Format.

The following fields are exported.

<table>
<tbody>
<tr class="odd">
<td><p>Field</p></td>
<td><p>Description</p></td>
</tr>
<tr class="even">
<td><p>ID</p></td>
<td><p>Displays a unique identifier used for the task in underlying tables.</p></td>
</tr>
<tr class="odd">
<td><p>Active</p></td>
<td><p>Displays &quot;Yes.&quot; dspTrack™ only imports tasks that are Active in Microsoft Project. When exported, those tasks are still marked as active.</p></td>
</tr>
<tr class="even">
<td><p>Task_Mode</p></td>
<td><p>Displays “Auto Scheduled,” the only valid value.</p></td>
</tr>
<tr class="odd">
<td><p>Name</p></td>
<td><p>Displays the task name.</p></td>
</tr>
<tr class="even">
<td><p>Duration</p></td>
<td><p>Displays the number of days between planned start and planned finish dates.</p></td>
</tr>
<tr class="odd">
<td><p>Start_Date</p></td>
<td><p>Displays the start date for work on the task according to the project schedule.</p></td>
</tr>
<tr class="even">
<td><p>Finish_Date</p></td>
<td><p>Displays the finish date for work on the task according to the project schedule.</p></td>
</tr>
<tr class="odd">
<td><p>Predecessors</p></td>
<td><p>Displays the ID of task(s) that is a predecessor to the current task, along with the dependency type (Finish to Start, Start to Finish, Finish to Finish, Start to Start)</p></td>
</tr>
<tr class="even">
<td><p>Notes</p></td>
<td><p>Displays a description of the task, which displays on the <em>PlanTask</em> page’s <em>Vertical</em> View on the General tab in the Description field.</p></td>
</tr>
<tr class="odd">
<td><p>Critical</p></td>
<td><p>Indicates whether the task is on the critical path, thus controlling the calculated start and finish dates for a project.</p>
<p><strong>NOTE:</strong> This value cannot be updated in dspTrack™.</p></td>
</tr>
<tr class="even">
<td><p>Milestone</p></td>
<td><p>Indicates whether the task is attached to a milestone in the project.</p>
<p><strong>NOTE:</strong> This value cannot be updated in dspTrack™.</p></td>
</tr>
<tr class="odd">
<td><p>Actual_Start</p></td>
<td><p>Displays the actual start date originally imported into the plan or the date that a user clicked Next Action on the Work List to begin work on the task. This date may not be the same as the planned start date.</p>
<p> </p>
<p><strong>NOTE</strong>: If work on a task has not started (i.e., Actual Start Date is blank for a task), the exported value in the Actual Start column is 1/1/0001 12:00:00 AM.</p></td>
</tr>
<tr class="even">
<td><p>Actual_Finish</p></td>
<td><p>Displays the actual finish date originally imported into the plan or the date that a user clicked Next Action on the Work List to complete work on the task. This date may not be the same as the planned finish date.</p>
<p> </p>
<p><strong>NOTE</strong>: If work on a task has not finished (i.e., Actual Finish Date is blank for a task) the exported value in the Actual Finish column is 1/1/0001 12:00:00 AM.</p></td>
</tr>
<tr class="odd">
<td><p>Calendar</p></td>
<td><p>If created in dspTrack™, the default calendar for the project is also exported, along with working days and hours.</p></td>
</tr>
</tbody>
</table>
