+++
title = 'Set Parameters for Schedule Status Calculation'
solution = 'Platform'
+++

# Set Parameters for Schedule Status Calculation

To set parameters for schedule status calculation at the plan level:

1.  Select **Project** in the *Navigation* pane.

2.  Click **Plans** for a project.

3.  Click **Vertical View** for a plan.

4.  Click the **Status Configuration** tab.

5.  Click **Edit**.
    
    [View the field descriptions for the Plan page’s Vertical View
    Status Configuration
    tab](../Page_Desc/Plan_H#tatus_Configuration_Tab)

6.  Enter a value in the **Pre Start Warn Threshold** field.
    
    **NOTE**: This threshold is the percent of the task duration prior
    to the <span> </span>planned start date as compared to the total
    duration of a task.
    
    For example, there are five days between a task’s planned start date
    and planned finish date. A user sets the Pre Start Warn threshold to
    20 (i.e., 20%). The task is behind and the task’s Schedule Status
    icon is yellow one day prior to the planned start date for the task.

7.  Enter a value in the **Post Start Warn Threshold** field.
    
    **NOTE**: This threshold is the percent of the task duration after
    the <span> </span>planned start date as compared to the total
    duration of the task. For example, there are five days between a
    task’s <span> </span>planned start date and planned finish date. A
    user sets the Post Start Warn threshold to 20 (i.e., 20%). The task
    is late, the task’s Schedule Status icon is red one day after the
    <span> </span>planned start date for the task.
    
    **NOTE**: If neither a Pre Start Warn or Post Start Warn threshold
    is supplied, a task’s <span> </span>planned start date is used to
    determine whether a task is on time or late. In this case, the
    task’s Schedule Status icon is either green or red, but will not
    display yellow.

8.  Enter a value in the **Pre End Warn Threshold** field.
    
    **NOTE**: This threshold is the percent of the task
    duration<span> </span> prior to the <span> </span>planned finish
    date as compared to the total task duration.<span> </span> For
    example, there are five days between a task’s planned start date and
    planned finish date. A user sets the Pre End Warn threshold to 20
    (i.e., 20%). The task is behind and the task’s Schedule Status icon
    is yellow one day prior to the <span> </span>planned finish date for
    the task.

9.  Enter a value in the **Post End Warn Threshold** field.
    
    **NOTE**: This threshold is the percent of the task duration after
    the <span> </span>planned finish date as compared to the total task
    duration. For example, there are five days between a task’s
    <span> </span>planned start date and planned finish date. A user
    sets the Post End Warn threshold to 20 (i.e., 20%). The task is late
    and the task’s Schedule Status icon is red one day after the
    <span> </span>planned finish date for the task.
    
    **NOTE**: If neither a Pre End Warn or Post End Warn threshold is
    supplied, a task’s planned finish date is used to determine whether
    a task is on time or late. In this case, the task’s Schedule Status
    icon is either green or red, but will not display yellow.

10. Select an option in the **Schedule Status Outlook ID** list box.
    
    **NOTE**: Values are:
    
      - **Optimistic** - A task’s schedule status can improve. For
        example, a task passes the Post-Start Warn threshold and its
        Schedule Status icon is red. Work on the task begins. The
        Schedule Status icon for the task changes to green.
      - **Pessimistic** - A task’s schedule status cannot improve. The
        schedule status either does not change or becomes worse. For
        example, if work on a task had not started after the Pre Start
        Warn threshold has passed the Schedule Status icon for that task
        is yellow. Depending on how work proceeds on the task, the
        task’s Schedule Status icon remains yellow or changes to red,
        but will never be green, even if the task is back on schedule.
    
    **NOTE**: The Schedule Status Outlook ID setting is required at the
    plan level and can be overridden at the task level.

11. Click **Save**.

To override the Schedule Status Outlook ID setting at the plan task
level:

1.  Select **Project** in the *Navigation* pane.

2.  Click **Plans** for a project.

3.  Click **Tasks** for plan.

4.  Click **Vertical View** for a task.

5.  Click the <span style="font-weight: bold;">Status
    Configuration</span> tab.

6.  Click **Edit**.
    
    [View the field descriptions for the Plan page’s Vertical View
    Status Configuration
    tab](../Page_Desc/Plan_H#tatus_Configuration_Tab)

7.  Select an option in the **Schedule Status Outlook ID** list box.
    
    **NOTE**: Values are:
    
      - **Inherit** - A task’s schedule status settings are inherited
        from the plan level.
      - **Optimistic** - A task’s schedule status can improve. For
        example, a task passes the Post-Start Warn threshold and its
        Schedule Status icon is red. Work on the task begins. The
        Schedule Status icon for the task changes to green.
      - **Pessimistic** - A task’s schedule status cannot improve. The
        schedule status either does not change or becomes worse. For
        example, if work on a task has not started and the Pre Start
        Warn threshold has passed, the Schedule Status icon for that
        task is yellow. Depending on how work proceeds on the task, the
        task’s Schedule Status icon remains yellow or changes to red,
        but will never be green, even if the task is back on schedule.
    
    **NOTE**: If no selection is made, Inherit is used.

8.  Click **Save**.
