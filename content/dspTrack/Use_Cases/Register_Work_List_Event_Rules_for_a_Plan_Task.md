+++
title = 'Register Work List Event Rules for a Plan Task'
solution = 'Platform'
+++

# Register Work List Event Rules for a Plan Task

Rules registered at the Plan Task level execute for the selected task.

Work List Event Rules can also be registered at the
[plan](Register_Work_List_Event_Rules_for_a_Plan.htm) level, [Work List
Item](Register_WorkList_Event_Rules_WorkList_Item.htm) level, or
[tag](Configure_Logic_Tags.htm) level.

Refer to [Register Work List Event
Rules](Register_Work_List_Event_Rules.htm) for more information about
viewing and editing all rules from one page, and about parameters that
can be used in Work List Event Rules.

To add a Work List Event Rule to a plan task:

1.  Select **Project** in the *Navigation* pane.

2.  Click **Plans** for a project.

3.  Click **Tasks** for a plan.

4.  Click **Rules** for a task.
    
    **NOTE:** If no rules exist, the page displays in add mode.
    Otherwise, click Add.
    
    [View the field descriptions for the Work List Event Rule - Plan
    Task page](../Page_Desc/Work_List_Event_Rule%20Plan_Task.htm)

5.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** The rule runs in this order if multiple rules are assigned
    to the plan task.

6.  Select the data source that contains the rule from the **DATA SOURCE
    ID** list box.
    
    **NOTE:** The rule runs in this order if multiple rules are assigned
    to the plan task.These options are data sources registered in
    Common. Refer to [Register a Data Source in
    Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
    for more information.

7.  Select the rule in the **RULE** list box.

8.  Select the event that triggers the rule to run in the **WORK LIST
    EVENT ID** list box.
    
    **NOTE:** Values are:
    
      - **Finish –** The rule runs when a user completes the Plan Task.
        To complete the Plan Task, on the Work List, click Next Action
        when the task’s status is In Progress.
      - **Start –** The rule runs when a user starts work on the Plan
        Task. To start work, on the Work List, click Next Action when
        the task’s status is Ready.

9.  Click the <span style="font-weight: bold;">ACTIVE</span><span> check
    box to disable it, if necessary.</span>
    
    **NOTE:** If a rule is inactive, the rule does not run.

10. Enter a comment about the rule in **COMMENT** field.

11. Click **Save**.

The rule will run for the Plan Task depending on the option selected in
the WORK LIST EVENT ID list box.
