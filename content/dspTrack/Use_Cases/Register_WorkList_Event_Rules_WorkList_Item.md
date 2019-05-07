+++
title = 'Register Work List Event Rules for a Work List Item'
solution = 'Platform'
+++

# Register Work List Event Rules for a Work List Item

On the *Work List Setup* page, Work List Items and Plan Tasks display. A
Work List Event Rule can be added to a Work List Item using the Rules
icon on this page.

Work List Event Rules can also be registered at the
[plan](Register_Work_List_Event_Rules_for_a_Plan.htm) level,  [Plan
Task](Register_Work_List_Event_Rules_for_a_Plan_Task.htm) level or
[tag](Configure_Logic_Tags.htm) level.

Refer to [Register Work List Event
Rules](Register_Work_List_Event_Rules.htm) for more information about
viewing and editing all rules from one page, and about parameters that
can be used in Work List Event Rules.

A Work List Event Rule cannot be added to a Plan Task using this page.
If a user selects Rules for a Plan Task on the *Work List Setup* page,
the *Work List Event Rule – Work List Setup – Plan Task* page displays.
This page is read only and displays information about Work List Event
Rules for Plan Tasks, which can only be added on the *Work List Event
Rule – Plan Task* page (Project \> Plans \> Tasks\> Rules)

To add a Work List Event Rule to a Work List Item:

1.  Select **Configuration \> Work List** in the *Navigation* pane.

2.  Click **Rules** for an item.
    
    **NOTE:** If no rules exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Work List Event Rule - Work
    List Setup
    page](../Page_Desc/Work_List_Event_Validations_Work_List_Setup_H.htm)

3.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** The rule runs in this order if multiple rules are assigned
    to the Work List Item.

4.  Select the data source that contains the rule from the **DATA SOURCE
    ID** list box.
    
    **NOTE:** These options are data sources registered in Common. Refer
    to [Register a Data Source in
    Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
    for more information.

5.  Select the rule in the **RULE** list box.

6.  Select the event that triggers the rule to run in the **WORK LIST
    EVENT ID** list box.
    
    **NOTE:** Values are:
    
      - **Finish –** The rule runs when a user completes the Work List
        Item. To complete the Work List Item, on the Work List, click
        Next Action when the item’s status is In Progress.
      - **Start –** The rule runs when a user starts work on the Work
        List Item. To start work, on the Work List, click Next Action
        when the item’s status is Ready.

7.  Click the <span style="font-weight: bold;">ACTIVE</span> check box
    to disable it, if necessary.
    
    **NOTE:** If a rule is inactive, the rule does not run.

8.  Enter a comment about the rule in **COMMENT** field.

9.  Click **Save**.

The rule will run for the Work List Item depending on the option
selected in the WORK LIST EVENT ID list box.
