# Configure Workflow Links

A workflow can contain a link that navigates a user to a specific page
to then perform a function, such as viewing data or clicking a button to
trigger an event. If the recipient of a workflow is to trigger an event,
such as clicking an Accept button to approve a Purchase Order, the event
can be invoked from within the email or notification message. If a
workflow link is clicked in an email, a new browser opens prompting the
user to sign in to DSP® (if the user is not anonymous or
semi-anonymous).

Before the workflow links can be configured, the required workflow
fields must be populated. Refer to [Configure Workflow
Fields](Configure_Workflow_Fields.htm) for more information.  The
Workflow Links button is disabled until Workflow Fields have been
configured.

To configure event links within a workflow:

1.  Select **Admin \>WebApps** on *Navigation pane*.

2.  Click **Pages** for a WEB APP NAME.

3.  Click **Events** for a **DESCRIPTION**.

4.  Click **Business Rules** for an **EVENT**.

5.  Click **Vertical View** for a business rule with a PROCEDURE TYPE of
    Workflow.

6.  Click **Workflow Links** button.
    
    **NOTE**: If no records exist, the page displays in add mode.
    Otherwise, click **Add**.
    
    [View the field descriptions for the Workflow Links
    page](../Page_Desc/Workflow_Links.htm).

7.  Enter a name in **LINK** field.
    
    **NOTE**: This text displays as the link name in the workflow email.

8.  Select an event from **Link to Event** list box.
    
    **NOTE**: The values in the **Link to Event** list box are events
    registered to the page selected for the **LinkToPageID** column on
    the Page Business Rules vertical view.

9.  Enter a priority in **SORT ORDER** field.
    
    **NOTE**: The **SORT ORDER** determines the order of the links, from
    left to right.

10. Click **Save**.
