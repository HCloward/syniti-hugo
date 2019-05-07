+++
title = 'Register Stored Procedure Events'
solution = 'Platform'
+++

# Register Stored Procedure Events

Stored procedure events execute a specified stored procedure. The stored
procedure parameters define the name/value pair for each parameter
passed to the stored procedure. Some stored procedures return output
parameters, which are entered with a leading @ character. For example,
the stored procedure GetRecordCount has 2 parameters: PackageName and
RecordCount. The stored procedure passes the parameter
‘PackageName=MARA’ and returns a RecordCount using a create
statement like this:

 

CREATE PROCEDURE GetRecordCount @PackageName nvarchar(100), @RecordCount
int Output AS Begin

….

 

End

 

After the stored procedure event runs, the @RecordCount parameter is
passed to the rest of the events as parameters on the *[WebApp
Event](../Page_Desc/WebApp_Event.htm)* page where

Field is set to CommandName and Value is set to “\[folder path\]”
\#PassedRecordCount\#

And

Field is set to PassedRecordCount and Value is set to @RecordCount

All event parameters are shared by an interface instance and are often
used to pass data to the next event.

To register a stored procedure event in Automate:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click **Add**.
    
    [View the field description for the Interface Events
    page](../Page_Desc/Interface_Events.htm)

<!-- end list -->

1.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** The PRIORITY field indicates the order in which the
    interface event runs.

<!-- end list -->

1.  Select **StoredProcedure** from the **EVENT TYPE** list box.
    
    **NOTE:** The PAGE ID field is not used for StoredProcedure event
    types.

2.  Click the **LOOP** check box to enable it, which indicates the event
    is intended to be processed multiple times based on input. Refer to
    [Set Up a Looping Process](Set_up_a_Looping_Process.htm) for more
    information.

3.  Enter a descriptive comment in the **COMMENT** field.

4.  Click **Save**; the *Vertical* View displays.
    
    **NOTE:** The EVENT TYPE selected on the *Horizontal* View
    determines the fields that display on the *Vertical* View.

<!-- end list -->

9.  Click the **Events** icon for the desired interface.
    
    *[View the field description for the Interface Events page’s
    Vertical View](../Page_Desc/Interface_Events.htm#InterfaceEventsV)*

10. Select a registered stored procedure event from the **Stored
    Procedure** list box.

**NOTE:** All stored procedures from the Data Source (as selected on the
*[Interfaces](../Page_Desc/Interfaces.htm)* page when the interface was
created) display. If a Stored Procedure Filter is defined on the
*[Parameters](../Page_Desc/Parameters.htm)* page, the list is narrowed
based on the filter.

1.  Click **Save**.
2.  Click the **Stored Procedure Parameters** icon to open the *[Stored
    Procedure](../Page_Desc/Stored_Procedure.htm)* page.

**NOTE:** When adding a stored procedure as an event, the parameters in
the stored procedure are automatically created for the event. Click the
Stored Procedure Parameters icon to view all parameters passed to the
event.
