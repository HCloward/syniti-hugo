+++
title = 'Create an OnValidate Page Event for Bulk Execution'
solution = 'Platform'
+++

# Create an OnValidate Page Event for Bulk Execution

Bulk Execution is only supported on the OnValidate event. This event
executes when a record is inserted, updated, or manually validated.
Validations can be of type Warning, Message, or Error. Refer to
[Validation Rules](../../WebApp_Dev/ValidationRules) for more
information.

Validations can also be configured to conditionally execute business
rules based on validation results. Refer to [Business
Rules](../../WebApp_Dev/Business_Rules) for more information.

To create an OnValidate page event for Bulk Execution:

1.  Select **WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a **WEB APP NAME**.

3.  Click the **Events** icon for a **DESCRIPTION**.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Page Events
    page](../Page_Desc/Page_Events_H)

4.  Select **OnValidate** from the **EVENT** list box.

5.  Select Foreground from the **EVENT PROCESS TYPE ID** list box.
    
    **NOTE:** For the Bulk Execution feature, the OnValidate event must
    run in the foreground so that the messages about validation failures
    can be seen. These messages do not display for background events.

6.  Click **Save**.

7.  Add Validation Rules to the event. Refer to [Validation
    Rules](../../WebApp_Dev/ValidationRules) for more information.

8.  Add Business Rules to the event, if needed. Refer to [Business
    Rules](../../WebApp_Dev/Business_Rules) for more information.
    
    **NOTE:** A page that has an OnValidate event which contains a non
    stored procedure business rule and a non-view validation rule will
    generate warnings relating to performance implications of having
    Bulk Execution enabled on a Page Event with these less-standard rule
    types
