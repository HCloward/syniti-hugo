+++
title = 'Register Work List Event Rules for a Plan'
solution = 'Platform'
+++

# Register Work List Event Rules for a Plan

Rules registered at the plan level execute for all tasks in the plan.

**NOTE:** Work List Items do not belong to plans, so rules registered to
a plan have no effect on Work List Items.

Work List Event Rules can also be registered at the [Work List
Item](Register_WorkList_Event_Rules_WorkList_Item) level, [Plan
Task](Register_Work_List_Event_Rules_for_a_Plan_Task) level or
[tag](Configure_Logic_Tags) level.

Refer to [Register Work List Event
Rules](Register_Work_List_Event_Rules) for more information about
viewing and editing all rules from one page, and about parameters that
can be used in Work List Event Rules.

To add a Work List Event Rule to a plan:

1.  Select **Project** in the *Navigation* pane.

2.  Click **Plans** for a project.

3.  Click **Rules** for a plan.
    
    **NOTE**: If no rules exist, the page displays in add mode.
    Otherwise, click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Work List Event Rules
    page](../Page_Desc/Work_List_Event_Rules)

4.  Enter a value in the **PRIORITY** field.
    
    **NOTE**: The rule runs in this order if multiple rules are assigned
    to the plan.

5.  Select the data source that contains the rule from the **DATA SOURCE
    ID** list box.
    
    **NOTE**: These options are data sources registered in Common. Refer
    to [Register a Data Source in
    Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common)
    for more information.

6.  Select the rule in the **RULE** list box.

7.  Select the event that triggers the rule to run in the **WORK LIST
    EVENT ID** list box.
    
    **NOTE:** Values are:
    
      - **Finish –** The rule runs when a user completes a Plan Task in
        the plan. To complete the Plan Task, on the Work List, click
        Next Action when the task’s status is In Progress.
      - **Start –** The rule runs when a user starts work on the Plan
        Task in the plan. To start work, on the Work List, click Next
        Action when the task’s status is Ready.

8.  Click the <span style="font-weight: bold;">ACTIVE</span> check box
    to disable it, if necessary.
    
    **NOTE:** If a rule is inactive, the rule does not run.

9.  Enter a comment about the rule in **COMMENT** field.

10. Click **Save**.

The rule will run for all tasks in the plan depending on the option
selected in the WORK LIST EVENT ID list box.
