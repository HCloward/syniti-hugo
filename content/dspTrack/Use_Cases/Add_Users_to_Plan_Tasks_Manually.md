+++
title = 'Add Users to Plan Tasks Manually'
solution = 'Platform'
+++

# Add Users to Plan Tasks Manually

When a project file is imported into dspTrack™, the component matches
the resources assigned to tasks to users registered in the platform.

Refer to [Import Project Files into
dspTrack™](Import_Project_Files_into_dspTrack) for more
information.

Users can also be assigned to tasks manually.

To add multiple users to a task, use a Security tag. Refer to [Configure
Security Tags](Configure_Security_Tags) for more information.

To add a few users to a task, use the *Plan Task User* page.

To add a user to a task:

1.  Select **Project** in the Navigation pane.

2.  Click **Plans** for a project.

3.  Click **Tasks** for a plan.

4.  Click **Users** for a task.
    
    **NOTE**: If no users are assigned to the task, the page displays in
    add mode. Otherwise, click
    <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Plan Task User
    page](../Page_Desc/Plan_Task_User)

5.  Select a user from the **USER ID** list box.

6.  Click the **PRIMARY CONTACT** check box to enable it, if necessary.
    
    **NOTE**: Only one user can be assigned as a primary contact per
    task. Use this setting for reporting purposes or to indicate the
    single source of contact for the task.

7.  Click the **PINNED** check box to change the setting, if necessary.
    
    **NOTE**: If the **PINNED** check box is enabled for a user, and the
    user is added to a task using a Security tag, that user will not be
    removed from the task if the Security tag is removed from the
    task.  
      
    Users can be assigned to tasks in two ways. Multiple users can be
    assigned to a task using a Security tag (Configuration \> Tag Type
    \> Security \> Registrations \> Users), or individual users can be
    added using the *Plan Task User* page (Project \> Plans \> Tasks \>
    Users).  
    Users assigned to a task using a Security tag can only be added or
    removed from the task via the *SecurityTagUser* page, but if the
    PINNED setting is enabled for a user, that user will not be removed
    from a task, even if the Security tag is removed from a task.
    
    <span style="font-weight: bold;">NOTE</span>: The PINNED setting is
    enabled by default for users added to a task directly on the *Plan
    Task User*<span> </span>page. However, if a user is added to a task
    using a Security tag, the PINNED check box is not enabled by default
    for the user and must be manually enabled on the *Plan Task User*
    page. Refer to [Use Tags](Use_Tags) and [Configure Security
    Tags](Configure_Security_Tags) for more information.

8.  Click **Save**.
