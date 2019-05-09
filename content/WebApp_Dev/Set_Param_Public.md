+++
title = 'Set Parameters for a Public WebApp Event'
solution = 'Platform'
+++

# Set Parameters for a Public WebApp Event

Enabling an event to be public allows other events from any WebApp to
call this event. When executed, the event will take in the parameters
configured in these steps, find the associated record from this page,
and fire the event.

At the Business Rule level, a user can set the value to pass to the
parameter on the *[Page Event Rule
Parameters](../Sys_Admin/Page_Desc/Page_Event_Rule_Parameters)*
page.

**NOTE:** When creating an event, a key column property must be set if
the page is based on a view or if the page doesn’t have a primary key.
For example, a user creates a background event that runs on a *Vertical*
View, but the parameter, the primary key, only displays on the
*Horizontal* View.

The user must either:

  - Include the primary key as one of the arguments in the stored
    procedure (since it should be in both the *Horizontal* and
    *Vertical* View) and then, in the stored procedure, run a select
    statement to get another column's value from the *Vertical* View
    using the primary key.
  - Include the column in the *Horizontal* View and hide it via a column
    property with the Horizontal View type. Refer to [Set Column Control
    Status](Set_Column_Control_Status) for more information.

To set parameters:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a WEB APP NAME.

3.  Click the **Events** icon for a page.

4.  Click **Vertical View** for an event.

5.  Click the **Advanced Properties** tab.

6.  Click the **Parameters** icon.
    
    **NOTE:** The Parameters icon is active if the **Public** check box
    is checked on the *Page Events* page's *Vertical* View.
    
    **NOTE:** If no records exist, the page opens in add mode.
    Otherwise, click **Add**.

7.  Enter a number in the **PRIORITY** field.
    
    **NOTE:** The priority order is used when aligning values from
    another event to call this event. The framework auto-inserts the
    table’s key fields in their order from the table, and/or the page’s
    column properties marked as keys. Commonly, higher priority
    parameters are specific to other business rules, such as plugins or
    procedures that expect other row data.

8.  Select a parameter or add one in the **PARAMETER NAME** combo box.
    
    **NOTE:** When the Public check box is checked on the *[Page
    Events](../Sys_Admin/Page_Desc/Page_Events_H)* page’s *Vertical*
    View, the page’s keys are inserted into the *[Page Event
    Parameters](../Sys_Admin/Page_Desc/Page_Event_Param_H)* page as
    the initial parameters.
    
    **NOTE:** This Parameter Name is populated on the *Page Event
    Parameters* page's *Vertical* View, where the user can select the
    parameter value.

9.  Select an option from the **PARAMETER TYPE** list box.
    
    **NOTE:** Options are:
    
      - **Required** – A value for this parameter must be passed to the
        event
      - **Key** – The value passed for this event must be a key(s)
        value. This value is also required, but is treated as a key
        field, not a data field, during event execution.
      - **Optional** – A value for this parameter could be passed to the
        event, but it is not required.

10. Enter a description in the **DESCRIPTION** text box.

11. Click **Save**.
