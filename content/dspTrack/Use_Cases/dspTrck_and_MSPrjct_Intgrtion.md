+++
title = 'dspTrack™ and MSProject Integration'
solution = 'Platform'
+++

# dspTrack™ and MSProject Integration

dspTrack™ is a task execution tool and should be used to monitor tasks
as they move through a workflow. It should not be used as a project
management tool. Updates to project data should be maintained in
MSProject or Microsoft Excel.

To update project data for a dspTrack™ plan:

1.  Export the data from dspTrack™

2.  Import the data into MSProject.

3.  Update the data in MSProject

4.  Import the updated data into dspTrack™ to update the existing plan.

**NOTE**: The critical path in dspTrack™ can be updated from MSProject
without requiring an export and import of data. Refer to [Calculate the
Critical Path for a Plan](Calculate_the_Critical_Path_for_a_Plan)
for more information.

Data can pass between dspTack™ and MSProject when:

  - [A project file created in MSProject is imported into dspTrack™ to
    create a new
    plan.](#MSProject_File_is_Imported_into_dspTrack__to_Create_a_Plan)
  - [A project file from MSProject with updated project data is imported
    into dspTrack™ to update  an existing plan in
    dspTrack™](#MSProject_File_is_Imported_into_dspTrack__to_Update_an_Existing_Plan)
  - [A project file is exported from dspTrack™ and imported into
    MSProject to update MSProject
    data](#A_project_file_is_Exported_from_dspTrack__and_Imported_into_MSProject_to_Create_project__in__MSProject)
  - [A project file is exported from dspTrack™ and imported into
    dspTrack™ to create a new
    project](#A_project_file_is_Exported_from_dspTrack__and_Imported_into_MSProject_to_Update_MSProject_Data_)

Refer to [Required Column for
Import](Required_Columns_for_Import)<span> </span>and [Export a
Project File](Export_a_Project_File) for more information about
which columns are imported into and exported from
dspTrack™.

### <span id="MSProject_File_is_Imported_into_dspTrack__to_Create_a_Plan"></span><span style="font-size: 14.0pt;">MSProject File is Imported into dspTrack™ to Create a</span><span> </span><span class="Heading2Char" style="font-size: 14.0pt;">Plan</span>

<span>When a project file created in MSProject is imported into</span>
dspTrack™ to create a new plan, all data comes from MSProject.

dspTrack™ sets the task status for each task. Refer to [Task Status on
Import](../Page_Desc/Task_Status_on_Import) for more information.

Refer to [Import Project Files into
dspTrack™](Import_Project_Files_into_dspTrack) for more
information.

### <span id="MSProject_File_is_Imported_into_dspTrack__to_Update_an_Existing_Plan"></span><span style="font-size: 14.0pt;">MSProject File is Imported into dspTrack™ to Update an Existing</span><span> </span><span class="Heading2Char" style="font-size: 14.0pt;">Plan</span>

Every time an MSProject file is imported in this case, the following
update occur in dspTrack™:

  - Any task created in MSProject that does not exist in dspTrack™ is
    created in dspTrack™
  - If a resource assignment in MSProject is updated for a task and that
    resource is registered in the platform, the resource assignment for
    the task is updated in dspTrack™
  - If a resource assignment in MSProject is updated for a task that
    exists in dspTrack™ and that resource is not registered in the
    platform, the resource must be registered on the
    <span style="font-style: italic;">Register Unregistered Users</span>
    page. After the user is registered, dspTrack™ assigns this user to a
    task.
  - If a MS Project plan has resource names assigned to tasks that do
    not exactly match the corresponding user IDs in the platform, the
    <span style="font-style: italic;">Resource Synonym</span> page can
    be used to map the resource names to the platform user IDs.
  - If a task was deleted in MSProject, dspTrack™ does not delete the
    task.
  - If a task is in a status of Complete in dspTrack™ and is not
    complete in MSProject (i.e., there is no date in the Actual Finish
    Date field when imported) there is no change to the task in
    dspTrack™. The task status will remain Completed.
  - dspTrack™ will notify the resource(s) assigned to a task using a
    workflow message and/or a notification if:
      - The task is not complete, and
      - The planned start date, planned finish date, actual start date
        or actual finish date are updated in the MSProject file.

Refer to [Receive Workflow Messages](Receive_Workflow_Messages) for
more information.

If data for any other imported field has been updated in the MSProject
file, that data will be updated in dspTrack™.

Refer to [Import Project Files into
dspTrack™](Import_Project_Files_into_dspTrack) for more
information.

### <span id="A_project_file_is_Exported_from_dspTrack__and_Imported_into_MSProject_to_Update_MSProject_Data_"></span>A project file is Exported from dspTrack™ and Imported into MSProject to Update MSProject Data<span> </span>

All data exported from dspTrack™ updates MSProject data when it is
imported into MSProject.

Refer to [Export a Project File](Export_a_Project_File) for
information about which columns are exported from
dspTrack™.

### <span id="A_project_file_is_Exported_from_dspTrack__and_Imported_into_MSProject_to_Create_project__in__MSProject"></span>A project file is Exported from dspTrack™ and Imported into MSProject to Create project<span> </span> in <span> </span>MSProject

If a dspTrack™ project is exported and the name of the project does not
exist in MSProject, a new project is created in MSProject when the
project is imported.
