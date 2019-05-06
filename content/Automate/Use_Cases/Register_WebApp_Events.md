# Register WebApp Events

WebApp events are DSP® events designed and declared as Public, which
allows such events to be called from Automate. These events perform a
specific action on a record. For example, Refreshing could be a WebApp
event for a Collect table.

To register a WebApp event in Automate:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click the **Events** icon for the desired interface.

3.  Click **Add**.
    
    [View the field description for the Interface Events
    page](../Page_Desc/Interface_Events.htm)

4.  Enter a value in the **PRIORITY** field.
    
    **NOTE:** The PRIORITY field indicates the order in which the
    interface event runs.

5.  Select **WebApp** from the **EVENT TYPE** list box.
    
    **NOTE:** The PAGE ID field displays a list of all WebApp pages that
    have public events defined. Refer to [About Automate
    Events](About_Automate_Events.htm) for more information.

6.  Select a page ID from the **PAGE ID** list box to configure where
    the event runs.

7.  Click the **LOOP** check box to enable it, indicating the event is
    intended to be processed multiple times based on input. Refer to
    [Set Up a Looping Process](Set_up_a_Looping_Process.htm) for more
    information.

8.  Enter a descriptive comment in the **COMMENT** field.

9.  Click **Save**; the *Vertical* View displays.
    
    **NOTE:** The EVENT TYPE selected on the *Horizontal* View
    determines the fields that display on the *Vertical* View.
    
    [View the field description for the Interface Events page’s Vertical
    View](../Page_Desc/Interface_Events.htm#InterfaceEventsV)

10. Select a WebApp event from the **Event** list box.
    
    **NOTE:** The Event Type and Page ID selected on the *Horizontal*
    View determine the options available in the Event list box. For
    example, if the page is Collect: Table (All Sources), the options
    are Build Package, Refresh, and Refresh DBMoto.

11. Click **Save**.

<!-- end list -->

1.  Click the **Web App Parameters** icon to open the *[WebApp
    Events](../Page_Desc/WebApp_Event.htm)* page. Use this page to enter
    field and values to pass to the event.
    
    **NOTE:** When adding a WebApp as an event, the parameters in the
    WebApp code are automatically created for the event. Click the Web
    Apps Parameters icon to view all parameters passed to the event. 

Enough parameters to uniquely describe the Primary Key in the WebApp
must be provided. If the WebApp contains a two-part Primary Key, a
minimum of two parameters must be defined.
