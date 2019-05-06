# Register Workflow Events

Workflow events execute a pre-defined workflow view. The workflow view
is selected from a list that contains all views found in the Automate
Data Source selected when adding an interface on the
*[Interfaces](../Page_Desc/Interfaces.htm)* page. Since simple workflow
events are expected to execute quickly, the Retry Parameters are not
necessary; WebApp events only try to execute once.

When creating the workflow view in the Data Source:

  - Name the view using the following convention: webXXXflow. Only views
    with this naming convention within the Data Source display.

  - Include at least 2 fields: EmailToSubject and Body.

Refer to [Workflow
Overview](../../Sys_Admin/Use_Cases/Workflow_Views.htm) in System
Administration for more details about creating workflow views.

The workflow event parameters uniquely define the record within the view
of the workflow event upon which the workflow event is executed. Define
the key-value pair used to filter the workflow view.

To register a workflow event in Automate:

1.  Select **Interfaces** in the *Navigation* pane.

2.  Click the **Events** icon for the desired interface.

3.  Click **Add**.
    
    [View the field description for the Interface Events
    page](../Page_Desc/Interface_Events.htm)

4.  Enter a value in the **PRIORITY** field.
    
    **NOTE**: The PRIORITY field indicates the order in which the
    interface event runs.

5.  Select Workflow from the **EVENT TYPE** list box.

6.  Select a page ID from the **PAGE ID** list box configure where the
    event runs. This field displays a list of all WebApp pages that have
    public events defined. Refer to [About Automate
    Events](About_Automate_Events.htm) for more information.

7.  Click the **LOOP** check box to enable it, indicating the event is
    intended to be processed multiple times based on input. Refer to
    [Set Up a Looping Process](Set_up_a_Looping_Process.htm) for more
    information.

8.  Enter a descriptive comment in the **COMMENT** field.

9.  Click **Save**; the *Vertical* View displays.
    
    **NOTE:** The EVENT TYPE selected on the Horizontal View determines
    the fields that display on the *Vertical* View.
    
    [View the field description for the Interface Events page’s Vertical
    View](../Page_Desc/Interface_Events.htm#InterfaceEventsV)

10. Select a Workflow event from the **Event** list box.

11. Select the workflow view to be used by the workflow event from
    **View** list box.
    
    **NOTE:** The view is created in the Data Source assigned when the
    interface was created on the
    *[Interfaces](../Page_Desc/Interfaces.htm)* page.

12. Select the protocol for sending and receiving emails from the
    **Workflow Method** list box.

13. Select a registered User ID from the **Workflow User ID** list box
    if using anonymous workflow, i.e., the email recipient does not have
    or need to have their own account to log in. To use standard
    workflow (i.e., an email is sent to the email address specified in
    the To field of the workflow view) or semi-anonymous workflow (i.e.,
    the user is automatically signed into their account without entering
    credentials), leave Workflow User ID blank. Refer to [Workflow
    Overview](../../Sys_Admin/Use_Cases/Workflow_Views.htm) in System
    Administration for more information.

14. Enter a number in the **Workflow Expire Days** field. After the
    defined number of days, the workflow link no longer works for the
    user.

15. Click the **Workflow Reuse** check box to enable it, allowing the
    workflow to be reused by another interface event.

16. Click the **Link To Page ID** list box to select the page that
    displays when the user clicks the workflow link in the workflow
    email.

17. Click the **Link To Page Restricted** check box to check it, which
    restricts page access between two pages bound by key fields. Uncheck
    the check box to deactivate the option and allow a link from one
    page to another without restrictions. This property is used in
    conjunction with the Binding Fieldnames field. Typically, when two
    pages contain shared key fields (such as Orders and Order Details),
    restrict the link to page by binding key.

18. Enter the names of the fields to bind the workflow event in the
    **Binding Fieldnames** field.
    
    **NOTE:** Binding fields are required when the primary keys are not
    available or if the primary keys have different names. They are
    needed when the linking relationship cannot be inferred because keys
    are either not defined or have different names from parent to child.
    Specify them here as one or more parent=child pairs, separated by
    commas. For example: CustomerID=CustID; or EmployeeID=EmployeeID,
    Department=DepartNo. (=child portion may be omitted if names are not
    different.)

19. Click **Save**. Two icons are available for further configuration:
    
      - **Fields–** Click to determine what is displayed in the subject
        line, body text, and other fields of the workflow.
        
        **NOTE:** These fields must be added to the view and aliased
        correctly to be utilized in the workflow. Refer to [Create a
        Workflow](../../WebApp_Dev/Create_a_Workflow.htm) in the System
        Administration help.
    
      - **Links –** Click to create links in the Workflow notification.

**NOTE**: Links is only enabled if the Link To Page ID field is
populated.
