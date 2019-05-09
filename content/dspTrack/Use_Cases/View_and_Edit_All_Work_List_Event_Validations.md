+++
title = 'View and Edit All Event Validations'
solution = 'Platform'
+++

# View and Edit All Event Validations

dspTrack™ displays all of the Event Validations for all Work List Items,
plans, Plan Tasks, and tags on the *Event Validations All* page.

To access this page, select **Configuration \> Event Validations**.

To edit an Event Validation on this page:

1.  Select <span style="font-weight: bold;">Configuration \> Events \>
    Validations</span><span style="font-weight: bold;">All</span> from
    the <span style="font-style: italic;">Navigation</span> pane.

2.  Click **Edit**; *Vertical* View displays.
    
    [View the field descriptions for the Event Validations All
    page](../Page_Desc/Event_Validations_All)

3.  Enter a value in **PRIORITY** field.
    
    **NOTE**: This value determines the order the validation runs.

4.  Select the data source that stores the view or stored procedure in
    the **Data Source ID** list box.
    
    **NOTE**: This data source must be registered in Common. Refer to
    [Register a Data Source in
    Common](../../Common/Use_Cases/Register_a_Data_Source_in_Common)
    for more information.

5.  Select the name of the stored procedure or view from the
    **Procedure/View** list box.
    
    **NOTE:** The name that displays for this field depends on the
    selection made in the VALIDATION TYPE list box on the *Horizontal*
    View.

6.  Select whether the validation runs when the Work List Item starts or
    ends in the **Work List Event ID** list box.
    
    **NOTE**: Values are:
    
      - **Finish –** The validation runs when a user completes the Work
        List Item. To complete work, on the Work List, click Next Action
        when the task’s status is In Progress.
      - **Start –** The validation runs when a user starts work on the
        Work List Item. To start work, on the Work List, click Next
        Action when the task’s status is Ready.

7.  Click the <span style="font-weight: bold;">ACTIVE</span> check box
    to disable it, if necessary.
    
    **NOTE**: If a validation is inactive, the validation does not run.

8.  Enter a brief message in the **ValidationMessage** box that will
    display to the user if the validation fails for the Work List Item.
    
    **NOTE**: The message should provide information about what may have
    caused the error and potential solutions if applicable.

9.  Enter a detailed description of the validation in the
    **Description** box.
    
    **NOTE**: This description should contain notes about the validation
    that serve as a summary of the SQL code so that another user does
    not have to review the SQL code to understand the validation.

10. Click **Save**.

The validation will run for the Work List Item depending on the option
selected in the WORK LIST EVENT ID list box.
