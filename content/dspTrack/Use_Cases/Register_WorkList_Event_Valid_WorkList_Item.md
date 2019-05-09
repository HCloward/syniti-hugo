+++
title = 'Register Work List Event Validations for a Work List Item'
solution = 'Platform'
+++

# Register Work List Event Validations for a Work List Item

On the *Work List Setup* page, Work List Items and Plan Tasks display. A
Work List Event Validation can be added to a Work List Item using the
Validations icon on this page.

Work List Event Validations can also be set at the [Plan
Task](Register_WorkList_Event_Validations_Plan_Task) level, the
[tag](Configure_Logic_Tags) level, and the
[plan](Register_WorkList_Event_Validations_Plan) level.

Refer to [Register Work List Event
Validations](Register_Work_List_Event_Validations) for more
information about viewing and editing all validations from one page, and
about parameters that can be used in Work List Event validations.

**NOTE**: A Work List Event Validation cannot be added to a Plan Task
using this page. if a user selects Validations for a Plan Task on the
*Work List Setup* page, the *Work List Event Validations Work List Setup
Task* page displays. This page is read only and displays information
about Work List Event Validations for Plan Tasks, which can only be
added on the *Work List Event Validation – Plan Task* page (Project \>
Plans \> Tasks\> Validations).

Validations are stored procedures or views that have been written and
saved in a data source that is registered in the DSP® prior to adding
the Work List Event Validation to a plan, Plan Task or Work List Item.

For example, if a validation registered to a Start event fails, then
work on the task cannot begin until the error is corrected and the
validation runs successfully.

**NOTE**: When a Work List Event Validation is added to a Plan Task
using a tag, then the validation cannot be edited at the Plan Task
level, on the W*ork List Event Validations All* page (Configuration \>
Work List Event Validations) or on the *Work List Event Validations All*
page (Configuration \> Work List Event Validations). Validations added
using a tag can only be edited at the tag level (Tag \> Tag Type \>
Registrations \> Validations). Refer to [Configure Logic
Tags](Configure_Logic_Tags) for more information.

To add a Work List Event Validation to a Work List Item:

1.  Select **Configuration \> Work List** in the *Navigation* pane.

2.  Click **Validations** for a Work List Item.
    
    **NOTE:** If <span style="font-weight: bold;">Validations</span> is
    clicked when a Plan Task is selected, the *Work List Event
    Validations Work List Setup Task* page displays.

3.  Enter a value in **PRIORITY** field.
    
    **NOTE:** This value determines the order the validation runs.

4.  Select whether the validation is a Stored Procedure or a View in the
    **VALIDATIONTYPE** list box.

5.  Click **Save**; the *Vertical* View displays.

6.  Select the data source that stores the view or stored procedure in
    the **Data Source ID** list box.
    
    **NOTE:** This data source must be registered in Common. Refer to
    [Register a Data Source in
    Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common)
    for more information..

7.  Select the name of the stored procedure or view from the
    **Procedure/View** list box.
    
    **NOTE:** The name that displays for this field depends on the
    selection made in the VALIDATION TYPE list box on the *Horizontal*
    View.

8.  Select whether the validation runs when the Work List Item starts or
    ends in the **Work List Event ID** list box.
    
    **NOTE:** Values are:
    
      - **Finish –** The validation runs when a user completes the Work
        List Item. To complete work, on the Work List, click Next Action
        when the task’s status is In Progress.
      - **Start –** The validation runs when a user starts work on the
        Work List Item. To start work, on the Work List, click Next
        Action when the task’s status is Ready.

9.  Click the **ACTIVE** check box to disable it, if necessary.
    
    **NOTE:** If a validation is inactive, the validation does not run.

10. Enter a brief message in the **ValidationMessage** box that will
    display to the user if the validation fails for the Work List Item.
    
    **NOTE:** The message should provide information about what may have
    caused the error and potential solutions if applicable.

11. Enter a detailed description of the validation in the
    **Description** box.
    
    **NOTE:** This description should contain notes about the validation
    that serve as a summary of the SQL code so that another user does
    not have to review the SQL code to understand the validation.

12. Click **Save**.

The validation will run for the Work List Item depending on the option
selected in the WORK LIST EVENT ID list box.
