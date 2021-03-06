+++
title = 'Register View Validations'
solution = 'Platform'
+++

# Register View Validations

To register view interface validations in Automate:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click the **Interfaces** icon for the desired interface to add a
    view validation at the interface level.
    
    OR
    
    Click the **Events** icon for the desired interface.

3.  Click the **Validations** icon for the desired event to add a view
    validation at the event level.

4.  Click **Add**.
    
    [View the field description for the Interface Validations
    page](../Page_Desc/Interface_Validations)

5.  Enter a value in the **PRIORITY** field to indicate the order in
    which the interface’s validations run.

6.  Select **View** from the **VALIDATION TYPE** list box.

7.  Select a purpose from the **VALIDATION PURPOSE** list box to
    determine why the validation is needed. Options are:
    
      - **Requirement–** Interface is not run if the view returns
        records.
    
      - **Validation –** Interface is not run if the view fails to
        return a record.

8.  Select a value from the **VALIDATION WHEN** list box to define when
    the validation is processed in relation to the event. Options are:
    
      - **Pre –** Runs the validation before running the event.
    
      - **Post –** Runs the validation after running the event. This
        option is typically used to determine if an event has run to
        completion.

9.  Select a disposition from the **DISPOSITION** list box. If the event
    fails the event validation rule, the disposition defines what
    happens next. Options are:
    
      - **Abort –** Unexpected condition. If the validation fails, the
        interface is turned off, and workflow emails are sent to the
        business and technical roles.
    
      - **Consider Complete –** Expected condition. The interface does
        not retry, the event is considered complete and the next event
        runs.
    
      - **Retry –** Expected condition. The interface retries this
        event/validation until there are no more event validation
        failures.

10. Click **Save**; the *Vertical* View displays.
    
    **NOTE:** The VALIDATION TYPE selected on the *Horizontal* View
    determines the configuration of the *Vertical* View.
    
    [View the field description for the Interface Validations page’s
    Vertical
    View](../Page_Desc/Interface_Validations#InterfaceValidationsV)

11. Click the **Validation View** list box to select a registered
    validation view. Only views ending in “Val” display, as defined by
    the Validation Filter field on the
    *[Parameters](../Page_Desc/Parameters)* page.

12. Enter a descriptive comment in the **Comment** field.

13. Click **Save**.
