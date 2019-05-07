+++
title = 'Register Work List Event Validations for a Plan'
solution = 'Platform'
+++

# Register Work List Event Validations for a Plan

Validations registered at the plan level execute for all tasks in the
plan.

**NOTE:** Work List Items do not belong to plans, so validation
registered to a plan have no effect on Work List Items.

Work List Event Validations can also be set at the [Plan
Task](Register_WorkList_Event_Validations_Plan_Task.htm) level, [Work
List Item](Register_WorkList_Event_Valid_WorkList_Item.htm) level, and
the [tag](Configure_Logic_Tags.htm) level.

Refer to [Register Work List Event
Validations](Register_Work_List_Event_Validations.htm) for more
information about viewing and editing all validations from one page, and
about parameters that can be used in Work List Event validations.

To add a Work List Event Validation to a plan:

1.  Select **Project** in the *Navigation* pane.

2.  Click **Plans** for a project.

3.  Click **Validations** for a plan.
    
    [View the field descriptions for the Work List Event Validations
    page](../Page_Desc/Work_List_Event_Validations_H.htm)
    
    **NOTE:** If no validations exist, the page displays in Add mode.
    Otherwise, click **Add**.

4.  Enter a value in **PRIORITY** field.
    
    **NOTE:** This value determines the order the validation runs.

5.  Select whether the validation is a Stored Procedure or a View in the
    **VALIDATIONTYPE** list box.

6.  Click **Save**; the *Vertical* View displays.

7.  Select the data source that stores the view or stored procedure in
    the **Data Source ID** list box.
    
    **NOTE:** This data source must be registered in Common. Refer to
    [Register a Data Source in
    Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
    for more information.

8.  Select the name of the stored procedure or view from the
    **Procedure/View** list box.
    
    **NOTE:** The name that displays for this field depends on the
    selection made in the VALIDATION TYPE list box on the *Horizontal*
    View.

9.  Select whether the validation runs when a task in the plan starts or
    ends in the **Work List Event ID** list box.
    
    **NOTE:** Values are:
    
      - **Finish –** The validation runs when a user completes a Plan
        Task in the plan. To complete the Plan Task, on the Work List,
        click Next Action when the task’s status is In Progress.
      - **Start –** The validation runs when a user starts work on a
        Plan Task in the plan. To start work, on the Work List, click
        Next Action when the task’s status is Ready.

10. Click the <span style="font-weight: bold;">ACTIVE</span><span> check
    box to disable it, if necessary.</span>
    
    **NOTE:** If a validation is inactive, the validation does not run.

11. Enter a brief message in the **ValidationMessage** box that will
    display to the user if the validation fails for a task in the plan.
    
    **NOTE:** The message should provide information about what may have
    caused the error and potential solutions if applicable.

12. Enter a detailed description of the validation in the
    **Description** box.
    
    **NOTE:** This description should contain notes about the validation
    that serve as a summary of the SQL code so that another user does
    not have to review the SQL code to understand the validation.

13. Click **Save**.

The validation will run for Plan Tasks in the plan depending on the
option selected in the WORK LIST EVENT ID list box.
