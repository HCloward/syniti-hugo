+++
title = 'Register Work List Event Validations for a Plan Task'
solution = 'Platform'
+++

# Register Work List Event Validations for a Plan Task

Validations registered at the Plan Task level execute for the selected
task.

Work List Event Validations can also be set at the [Plan
Task](Register_WorkList_Event_Validations_Plan_Task.htm) level, [Work
List Item](Register_WorkList_Event_Valid_WorkList_Item.htm) level, at
the [tag](Configure_Logic_Tags.htm) level, and at the
[plan](Register_WorkList_Event_Validations_Plan.htm) level.

Refer to [Register Work List Event
Validations](Register_Work_List_Event_Validations.htm) for more
information about registering validations at the plan level, viewing and
editing all validations, and parameters that can be used for Work List
Event Validations.

To add a Work List Event Validation to a plan task:

1.  Select **Project** in the *Navigation* pane.

2.  Click **Plans** for a project.

3.  Click **Tasks** for a plan.

4.  Click **Validations** for a task.
    
    **NOTE:** If no validations exist, the page displays in add mode.
    Otherwise, click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Work List Event Validation -
    Plan Task
    page](../Page_Desc/Work_List_Event_Validations_Plan_Task.htm)

5.  Enter a value in **PRIORITY** field.
    
    **NOTE:** This value determines the order the validation runs.

6.  Select whether the validation is a Stored Procedure or a View in the
    **VALIDATIONTYPE** list box.

7.  Click **Save**; the *Vertical* View displays.

8.  Select the data source that stores the view or stored procedure in
    the **Data Source ID** list box.
    
    **NOTE:** This data source must be registered in Common. Refer to
    [Register a Data Source in
    Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common.htm)
    for more information.

9.  Select the name of the stored procedure or view from the
    **Procedure/View** list box.
    
    **NOTE:** The name that displays for this field depends on the
    selection made in the VALIDATION TYPE list box on the *Horizontal*
    View.

10. Select whether the validation runs when the task starts or ends in
    the **Work List Event ID** list box.
    
    **NOTE:** Values are:
    
      - **Finish –** The validation runs when a user completes the Plan
        Task. To complete the Plan Task, on the Work List, click Next
        Action when the task’s status is In Progress.
      - **Start –** The validation runs when a user starts work on the
        Plan Task. To start work, on the Work List, click Next Action
        when the task’s status is Ready.

11. Click the <span style="font-weight: bold;">ACTIVE</span> check box
    to disable it, if necessary.
    
    **NOTE:** If a validation is inactive, the validation does not run.

12. Enter a brief message in the **ValidationMessage** box that will
    display to the user if the validation fails for the Plan Task.
    
    **NOTE:** The message should provide information about what may have
    caused the error and potential solutions if applicable.

13. Enter a detailed description of the validation in the
    **Description** box.
    
    **NOTE:** This description should contain notes about the validation
    that serve as a summary of the SQL code so that another user does
    not have to review the SQL code to understand the validation.

14. Click **Save**.

The validation will run for the Plan Task depending on the option
selected in the WORK LIST EVENT ID list box.
