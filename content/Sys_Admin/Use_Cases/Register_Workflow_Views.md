+++
title = 'Register Workflow Views'
solution = 'Platform'
+++

# Register Workflow Views

Once the view is created, the view must be registered in the platform.
Each row in this view represents one email. If this view includes two
rows for a specific key from the source page, two emails are sent.

To register a workflow view:

1.  Select **WebApps** in the*Navigation* pane.

2.  Click **Pages** for a **WEB APP NAME**.

3.  Click **Events** for a **DESCRIPTION**.
    
    **NOTE**: The **DESCRIPTION** is the name of the page.
    
    **NOTE:** If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Page Events
    page.](../Page_Desc/Page_Events_H.htm)

4.  Select an option from the **EVENT** list box.

5.  The **ACTIVE** check box is enabled by default.

6.  Select an option from the **EVENT PROCESS TYPE ID** list box.

7.  Click **Save**; the *Vertical View* displays.

8.  Enter the **Pre Message**, **Post Message** and **Comments** for the
    event on the General tab.
    
    **NOTE**: It is very unlikely that a user will need to change the
    options in the Advanced Properties tab (step \#9) when setting up a
    workflow. Most users can skip this step and continue with step \#10.

9.  Click the **Advanced Properties** tab.
    
    1.  Select an option from the **Transaction Method** list box.
    
    2.  Select an option from the **Function** list box.
    
    3.  Select an option from the **Event Level** list box.
    
    4.  Click the **Public** check box to enable it, allowing the event
        to be called via a Business Rule from a page in any WebApp.
    
    5.  Select an option from the **Page View Type** list box.

10. Click **Save**.

11. Click **Business Rules** for an **EVENT**.
    
    **NOTE**: The business rule will run when this event is executed.
    
    **NOTE**: If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Page Business Rules
    page.](../Page_Desc/Page_Business_Rules_H.htm)

12. Enter the value in **PRIORITY** field.
    
    **NOTE**: If multiple business rules exist for the page, this number
    indicates the order in which they are run.

13. Verify **ACTIVE** check box is enabled.

14. Select **Workflow** from **PROCEDURE TYPE** list box.

15. Click **Save**; *Vertical View* displays.

16. Select the workflow view from the **Alternate View** list box.

17. Select a value from the **Message Type ID** list box.

18. Enter a description in **Comment** field.

19. Select an ID from **Link User ID** field.
    
    **NOTE**: The **Link User ID** is used for anonymous users. This
    list box displays all Anonymous user accounts. Refer to the
    [Workflow Views Overview](Workflow_Views.htm) for more information
    on creating an anonymous user account.

20. Enter a value in **Link Expire Days**.
    
    **NOTE**: **Link Expire Days** controls the number of days the
    workflow link is active and therefore accessible.

21. Click **Link Reuse** check box.
    
    **NOTE**: **Link Reuse** enables the workflow link to be used
    multiple times until it expires. Otherwise, the user is denied
    access to the workflow link after one use.

22. Select an ID from **Link to Page ID** list box.
    
    **NOTE**: The **Link to Page ID** field controls the page that opens
    when the user clicks the link. Options in this list box display as
    \[Component Name : Page Name\], e.g., Collect : Copy Targets.

23. Click the **Link To Page Restricted** check box to enable it.
    
    **NOTE**:  The **Link To Page Restricted** restricts page access
    between two pages bound by key fields. Disable the check box to
    deactivate the option and allow a link from one page to another
    without restrictions. This property is used in conjunction with the
    Binding Field Names option.  Normally when two pages contain shared
    key fields (such as Orders and Order Details), restrict the link to
    page by binding key. Turning this option off allows the user to link
    from one page to another without restriction.

24. Enter field names in **Binding Field Names** field, if applicable.
    
    **NOTE**: Binding fields are required when the primary keys are not
    available or if the primary keys have different names. They are
    needed when the linking relationship cannot be inferred, because
    keys are either not defined or have different names from parent to
    child. Specify them here as one or more parent=child pairs,
    separated by commas. For example: *CustomerID=CustID*; or
    *EmployeeID=EmployeeID, Department=DepartNo*. (*=child* portion may
    be omitted if names are not different.)

25. Click the **+** next to **Advanced Properties** label to configure
    additional workflow properties.

26. Click the **Run On Validate** check box to execute the workflow if
    the corresponding validation rule returns zero records or if it
    returns records with a severity level less than Error.

27. Click the **Run On Validate Fail** check box to execute the workflow
    if the corresponding validation rule returns any record that fails
    with a severity level of Error.

28. Click the **Force Foreground Execution** check box to execute the
    workflow in the foreground.
    
    **NOTE**: If the user should be notified that a workflow is being
    sent, then it should be set to run in the foreground.  If the
    workflow will take a long time to send (e.g. emails are being sent
    to many users) than it might be better to run in the background.

29. Click the **Workflow Fields** button to configure the workflow
    fields. Refer to [Configure Workflow
    Fields](Configure_Workflow_Fields.htm) for more information about
    configuring the workflow email sent with this workflow.

30. Click the **Workflow Links** button to create custom workflow links.
    Refer to [Configure Workflow Links](Configure_Workflow_Links.htm)
    for more information.
    
    **NOTE**: The **Workflow Links** button is not accessible until
    **Save** is clicked.

31. Click **Save**.
