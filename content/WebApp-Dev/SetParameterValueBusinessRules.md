# Set a Parameter Value for Business Rule Parameters for a Public WebApp Event

A public WebApp event can be accessed from any WebApp.

A public WebApp event can have parameters set that must be passed when
calling that event from another event. These parameters are either:

  - Configured on the *[Page Event
    Parameters](../Sys_Admin/Page_Desc/Page_Event_Param_H.htm)* page.
    Refer to [Set Parameters for a Public WebApp
    Event](Set_Param_Public.htm) for more information.
  - Set in the Parameter view when creating the Business rule,

The Business rule that calls the public WebApp event must pass values
with a parameter type of Key or Required. The values to pass are defined
on the *[Page Event Rule
Parameters](../Sys_Admin/Page_Desc/Page_Event_Rule_Parameters.htm)*
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
    Status](Set_Column_Control_Status.htm) for more information.

To set the parameter values to pass to the public WebApp event:

1.  Select **Admin \> WebApps** in the *Navigation* pane.

2.  Click the **Pages** icon for a **WEB APP NAME**.

3.  Click the **Events** icon for a page.

4.  Click the Business Rules icon for an event.

5.  Click **Vertical View** for for a Business rule with a procedure
    type of WebApp Event.

6.  Click the **Parameters** icon.

7.  Click **Edit.**
    
    **NOTE:** The Parameter Name and Parameter Type were added on the
    *Page Event Parameters* page. If the Parameter Type is Required or
    Key, a Parameter Value must be added.

8.  Select a value from the **PARAMETER VALUE** list box.

9.  Click **Save**.
