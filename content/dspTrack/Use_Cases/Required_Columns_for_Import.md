+++
title = 'Required Columns for Import into dspTrack™'
solution = 'Platform'
+++

# Required Columns for Import into dspTrack™

To be imported into dspTrack™, the following columns are required in the
spreadsheet or project file:

  - ID

  - Active
    
    **NOTE**: dspTrack™ will only import tasks that are marked as Active
    in MicroSoft Project.

  - Task Mode
    
    **NOTE**: Auto Scheduled is the only valid value in this column.

  - Name
    
    **NOTE**: This value in this column displays in the NAME column on
    the <span style="font-style: italic;">Plan</span>*Task* page after
    the file is imported.

  - Start Date
    
    **NOTE**: This date corresponds to the Planned Start Date in
    dspTrack™.

  - Finish Date
    
    **NOTE**: This date corresponds to the Planned Finish Date in
    dspTrack™.

  - Predecessors
    
    **NOTE**: This column displays the ID of the predecessor task which
    is displayed on the
    <span style="font-style: italic;">Plan</span>*Task Dependency* page
    after the file is imported.

  - Summary
    
    <span style="font-weight: bold;">NOTE</span>: dspTrack™ does not
    import Summary tasks, so this column will always display No.

  - Critical
    
    **NOTE**: This information displays on the Task’s *Vertical* View on
    the Additional Information tab after the file is imported.

  - Milestone
    
    **NOTE**: This information displays on the Task’s *Vertical* View on
    the Additional Information tab.

  - Notes
    
    **NOTE**: The data in this column displays on the
    <span style="font-style: italic;">Plan</span>*Task* page’s
    *Vertical* View on the General tab, in the Description field after
    the file is imported.

  - Actual Start
    
    <span style="font-weight: bold;">NOTE</span>: If the Actual Start
    date for a task to be imported is after the current date, the import
    will fail. If the file being imported into dspTrack™ is an Excel
    file, the Actual Start Date must be updated to a date equal to or
    earlier than the current date in the Excel file. If the file being
    imported into dspTrack™ is a Microsoft Project file, the Actual
    Start Date must be updated to a date equal to or earlier than the
    current date in Microsoft Project. After correcting the Actual Start
    Date, import the file again.

  - Actual Finish
    
    <span style="font-weight: bold;">NOTE</span>: When importing a
    Microsoft Project file (.mpp), the Duration and Unit of Measure
    (UOM) fields are also imported for each plan task. When importing an
    Excel spreadsheet (.xlsx), if the Duration and Unit of Measure (UOM)
    fields are included, they will be imported as well. The Duration and
    UOM fields are also exported.
    
    **NOTE**: If a project is imported into dspTrack™, and the slack
    value is in the form of a percent in Microsoft Project, that value
    will be displayed as number of days in the Slack and Slack UOM
    fields on the *Plan Task Dependency* page.

  - Duration
    
    <span style="font-weight: bold;">NOTE</span>: This number, along
    with the Unit of Measure (UOM), determines how long the task should
    take to complete. This number can be a decimal and is used in
    schedule status calculations and on reports.
    
    <span style="font-weight: bold;">NOTE</span>: The import will fail
    if the Duration field is 0 for any tasks in the project.

  - UOM
    
    <span style="font-weight: bold;">NOTE</span>: This field, along with
    the Duration field, determines how long the task should take to
    complete and is used in Schedule Status calculations and on reports.
    Values are Days, Hours, Minutes, Months and Weeks.
