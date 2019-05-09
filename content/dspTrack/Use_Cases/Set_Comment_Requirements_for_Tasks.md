+++
title = 'Set Comment Requirements for Tasks'
solution = 'Platform'
+++

# Set Comment Requirements for Tasks

By default, comments are not required when finishing a task, even if the
task is finished after the planned finish date. A user finishes a task
by clicking the Next Action button on the Work List for a task with a
status of In Progress.

Refer to [Task Status](../Page_Desc/Task_Status1) for more
information.

dspTrack™ can be configured to require a user to enter a comment when
finishing a task on, before, or after the planned finish date.

Comment requirements can be set at the following levels:

  - [Parameters](#Parameters)
  - [Plan](#Project)
  - [Tag](#Tag)
  - [Task](#Task)

## <span id="Parameters"></span>Parameters

Configurations set at the parameter level can be inherited by all plans
(and their assigned tags and tasks), but can be overwritten at the plan,
tag or task level.

To set the comment requirement at the parameter level:

1.  Select **Configuration \> Parameters** from *Navigation* pane.

2.  Click the **Validations** tab.

3.  Click **Edit**.
    
    [View the field descriptions for the Validations tab on the
    Parameters
    page](../Page_Desc/Parameters_dspTrack#Validations_Tab)

4.  Select an option in **Require Late Comment** list box, if
    applicable.
    
    **NOTE:** Values include:
    
      - **Yes –** All of the tasks in dspTrack™ will require a comment
        when the user clicks Next Action for a task with a status of In
        Progress on the <span>Work List</span> after the planned finish
        date.
      - **No –** None of the tasks in dspTrack™ will require a comment
        when the user clicks Next Action for a task with a status of In
        Progress after the planned finish date.

5.  Select an option in **Require Comment** list box, if applicable.
    
    **NOTE:** Values include:
    
      - **Yes –** All of the tasks in dspTrack™ will require a comment
        when the user clicks Next Action for a task in In Progress
        status on or before the planned finish date.
      - **No –** None of the tasks in dspTrack™ will require a comment
        when the user clicks Next Action for a task in In Progress
        status on or before the planned finish date.

## <span id="Project"></span>Plan

Configurations set at the plan level can be inherited by all tags and
tasks, but can be overwritten at the tag or task level.

To set the comment requirement at the plan level:

1.  Select **Project** from *Navigation* pane.

2.  Click Plans for a project.

3.  Click **Vertical View** for a plan.

4.  Click **Edit**.
    
    [View the field descriptions for the General tab of the Plan Task
    page’s Vertical View](../Page_Desc/Plan_Task_H#Plan_Task_V)

5.  Select an option in **Require Late Comment** list box, if
    applicable.

6.  Select an option in **Require Comment** list box, if applicable.
    
    **NOTE:** Values include:
    
      - **Inherit** - The Require Comment setting is inherited from the
        most granular level in the hierarchy. If the Require Comment
        setting is set to\[None\], Inherit is used by default. The
        requirement hierarchy’s most granular level is task, followed by
        tag, plan and parameter.  
        Require Comment settings set at the task level override those
        set at any other level. If a task's Require Comment setting is
        set to\[None\]or Inherit, the task's Require Comment setting is
        inherited from the tag level (provided the tag level does not
        also have a Require Comment setting of\[None\]or Inherit). If
        the tag level has a Require Comment setting of Inherit
        or\[None\], Require Comment settings are then inherited at the
        plan level (provided the plan level does not also have a Require
        Comment setting of\[None\]or Inherit), and so on.  
        For example, the Require Comment list box has been set
        to\[None\]at the parameter level. At the plan level, it has been
        set to Inherit. At the tag level, the Require Comment list box
        is set to Yes. At the task level, Task A in the Plan has a
        Require Comment setting of Inherit. Task B in the plan has a
        Require Comment setting of No. In this scenario, Task A would
        have a Require Comment setting of Yes. Task B would have a
        Require Comment setting of No.
      - **Yes –** All of the tasks in the plan will require a comment
        when the user clicks Next Action for a task in In Progress
        status on or before the planned finish date.
      - **No –** None of the tasks in the plan will require a comment
        when the user clicks Next Action for a task in In Progress
        status on or before the planned finish date.

## <span id="Tag"></span>Tag

Configurations set at the tag level can be inherited by all tasks that
are assigned to that tag, but can be overwritten at the task level.

**NOTE**: In a case where different tags assigned to the same task have
different requirements settings, if a configuration setting exists at
the plan level, this will be the setting selected for the task. If no
requirement setting exists at the plan level, the setting at the
parameters level will be applied to the task.  
For example, a plan requires comments for all tasks. The plan has two
tags. The Comment tag requires comments must be entered when finishing a
task. The tag No Comment does not require comments for a task. The
Generate Audit Report task has both the Comment and No Comment tags
assigned. Because these tags are in conflict, the task will use the
comment requirement setting from the plan level, and will require
comments when a user finishes the task.

To set the comment requirement at the tag level:

1.  Select **Configuration \> Tag Type** from *Navigation* pane.

2.  Select a Tag Type.

3.  Click **Vertical View** for a tag.

4.  Click **Edit**.
    
    [View the field descriptions for the Tag page’s Vertical
    View](../Page_Desc/Tag#Tag_V)

5.  Select an option in **Require Late Comment** list box, if
    applicable.
    
    **NOTE**: Values include:
    
      - **Inherit** - The Require Late Comment setting is inherited from
        the most granular level in the hierarchy. If the Require Late
        Comment setting is set to\[None\], Inherit is used by default.
        The requirement hierarchy’s most granular level is task,
        followed by tag, plan and parameter.  
        Require Late Comment settings set at the task level override
        those set at any other level. If a task's Require Late Comment
        setting is set to\[None\]or Inherit, the task's Require Late
        Comment setting is inherited from the tag level (provided the
        tag level does not also have a Require Late Comment setting
        of\[None\]or Inherit). If the tag level has a Require Late
        Comment setting of Inherit or\[None\], Require Late Comment
        settings are then inherited at the plan level (provided the plan
        level does not also have a Require Late Comment setting
        of\[None\]or Inherit), and so on.  
        For example, the Require Late Comment list box has been set
        to\[None\]at the parameter level. At the plan level, it has been
        set to Inherit. At the tag level, the Require Late Comment list
        box is set to Yes. At the task level, Task A in the Plan has a
        Require Late Comment setting of Inherit. Task B in the plan has
        a Require Late Comment setting of No. In this scenario, Task A
        would have a Require Late Comment setting of Yes. Task B would
        have a Require Late Comment setting of No.
      - **Yes –** All of the tasks with the tag will require a comment
        when the user clicks Next Action for a task with a status of In
        Progress status after the planned finish date.
      - **No –** None of the tasks with the tag will require a comment
        when the user clicks Next Action for a task with a status of In
        Progress after the planned finish date.

6.  Select an option in **Require Comment** list box, if applicable.
    
    **NOTE**: Values include:
    
      - **Inherit** - The Require Comment setting is inherited from the
        most granular level in the hierarchy. If the Require Comment
        setting is set to\[None\], Inherit is used by default. The
        requirement hierarchy’s most granular level is task, followed by
        tag, plan and parameter.  
        Require Comment settings set at the task level override those
        set at any other level. If a task's Require Comment setting is
        set to\[None\]or Inherit, the task's Require Comment setting is
        inherited from the tag level (provided the tag level does not
        also have a Require Comment setting of\[None\]or Inherit). If
        the tag level has a Require Comment setting of Inherit
        or\[None\], Require Comment settings are then inherited at the
        plan level (provided the plan level does not also have a Require
        Comment setting of\[None\]or Inherit), and so on.  
        For example, the Require Comment list box has been set
        to\[None\]at the parameter level. At the plan level, it has been
        set to Inherit. At the tag level, the Require Comment list box
        is set to Yes. At the task level, Task A in the Plan has a
        Require Comment setting of Inherit. Task B in the plan has a
        Require Comment setting of No. In this scenario, Task A would
        have a Require Comment setting of Yes. Task B would have a
        Require Comment setting of No. 
      - **Yes –** All of the tasks with the label will require a comment
        when the user clicks Next Action for a task in In Progress
        status on or before the planned finish date.
      - **No –** None of the tasks with the label will require a comment
        when the user clicks Next Action for a task in In Progress
        status on or before the planned finish date.

## <span id="Task"></span>Task

To set the comment requirement at the task level:

1.  Select **Project** from *Navigation* pane.

2.  Click Plans for a project.

3.  Click **Tasks** for a plan.

4.  Click **Vertical View** for a task.

5.  Click **Edit**.
    
    [View the field descriptions for the General tab of the Plan Task
    page’s Vertical View](../Page_Desc/Plan_Task_H#General_Tab)

6.  Select an option in **Require Late Comment** list box, if
    applicable.
    
    **NOTE:** Values include:
    
      - **Inherit** - The Require Late Comment setting is inherited from
        the most granular level in the hierarchy. If the Require Late
        Comment setting is set to\[None\], Inherit is used by default.
        The requirement hierarchy’s most granular level is task,
        followed by tag, plan and parameter.  
        Require Late Comment settings set at the task level override
        those set at any other level. If a task's Require Late Comment
        setting is set to\[None\]or Inherit, the task's Require Late
        Comment setting is inherited from the tag level (provided the
        tag level does not also have a Require Late Comment setting
        of\[None\]or Inherit). If the tag level has a Require Late
        Comment setting of Inherit or\[None\], Require Late Comment
        settings are then inherited at the plan level (provided the plan
        level does not also have a Require Late Comment setting
        of\[None\]or Inherit), and so on.  
        For example, the Require Late Comment list box has been set
        to\[None\]at the parameter level. At the plan level, it has been
        set to Inherit. At the tag level, the Require Late Comment list
        box is set to Yes. At the task level, Task A in the Plan has a
        Require Late Comment setting of Inherit. Task B in the plan has
        a Require Late Comment setting of No. In this scenario, Task A
        would have a Require Late Comment setting of Yes. Task B would
        have a Require Late Comment setting of No.
      - **Yes –** This task will require a comment when the user clicks
        Next Action for a task with a status of In Progress after the
        planned finish date.
      - **No –** This task will not require a comment when the user
        clicks Next Action for a task with a status of In Progress after
        the planned finish date.

7.  Select an option in **Require Comment** list box, if applicable.
    
    **NOTE:** Values include:
    
      - **Inherit** - The Require Comment setting is inherited from the
        most granular level in the hierarchy. If the Require Comment
        setting is set to\[None\], Inherit is used by default. The
        requirement hierarchy’s most granular level is task, followed by
        tag, plan and parameter.  
        Require Comment settings set at the task level override those
        set at any other level. If a task's Require Comment setting is
        set to\[None\]or Inherit, the task's Require Comment setting is
        inherited from the tag level (provided the tag level does not
        also have a Require Comment setting of\[None\]or Inherit). If
        the tag level has a Require Comment setting of Inherit
        or\[None\], Require Comment settings are then inherited at the
        plan level (provided the plan level does not also have a Require
        Comment setting of\[None\]or Inherit), and so on.  
        For example, the Require Comment list box has been set
        to\[None\]at the parameter level. At the plan level, it has been
        set to Inherit. At the tag level, the Require Comment list box
        is set to Yes. At the task level, Task A in the Plan has a
        Require Comment setting of Inherit. Task B in the plan has a
        Require Comment setting of No. In this scenario, Task A would
        have a Require Comment setting of Yes. Task B would have a
        Require Comment setting of No.
      - **Yes –** This task will require a comment when the user clicks
        Next Action for a task in In Progress status on or before the
        planned finish date.
      - **No –** This task will not require a comment when the user
        clicks Next Action for a task in In Progress status on or before
        the planned finish date.
