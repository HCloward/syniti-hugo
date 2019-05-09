+++
title = 'View and Edit All Event Rules'
solution = 'Platform'
+++

# View and Edit All Event Rules

dspTrack™ displays all of the Event Rules for all Work List Items,
plans, Plan Tasks, and tags on the *Event Rules All* page.

To access this page, select **Configuration \> Event Rules**.

To edit a Work List Event Rule on this page:

1.  Select <span style="font-weight: bold;">Configuration \> Event \>
    Rules - All  </span>from the
    <span style="font-style: italic;">Navigation</span> pane.

2.  Click <span style="font-weight: bold;">Edit</span>.
    
    [View the field descriptions for the *Event Rules All*
    page](../Page_Desc/Work_List_Event_Rules_All)

3.  Enter a value in the **PRIORITY** field.
    
    **NOTE**: The rule runs in this order if multiple rules are assigned
    to the plan, Plan Task, Work List Item or tag.

4.  Select the data source that contains the rule from the **DATA SOURCE
    ID** list box.
    
    **NOTE**: These options are data sources registered in the platform.

5.  Select the rule in the **RULE** list box.

6.  Select the event that triggers the rule to run in the **WORK LIST
    EVENT ID** list box.
    
    **NOTE**: Values are:
    
      - **Finish –** The rule runs when a user completes the Work List
        Item of Plan Task. To complete the Work List Item or Plan Task,
        on the Work List, click Next Action when the item’s status is In
        Progress.
      - **Start –** The rule runs when a user starts work on the Work
        List Item or Plan Task. To start work, on the Work List, click
        Next Action when the item’s status is Ready.

7.  Click the <span style="font-weight: bold;">ACTIVE</span> check box
    to disable it, if necessary.
    
    **NOTE**: If a rule is inactive, the rule does not run.

8.  Enter a comment about the rule in **COMMENT** field.

9.  Click **Save**.

The rule will run for the Work List Item or Plan Task depending on the
option selected in the WORK LIST EVENT ID list box.
