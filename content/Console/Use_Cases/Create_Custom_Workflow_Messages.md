+++
title = 'Create Custom Workflow Messages'
solution = 'Migration'
+++

# Create Custom Workflow Messages

Console allows users to set up custom workflow messages to notify users
with a report summary. Console is delivered with a weekly Map status;
however, additional workflow messages can be added.

Before adding the workflow message, create the workflow views and
register them in System Administration.

To create the message:

  - [Create the Message](#Create)

  - [Add Users to the Workflow Message](#Add)

  - [Register Workflow Views](#Register)

  - [Process Workflow](#Process)

## <span id="Create"></span>Create the Message

To create a custom workflow message:

1.  Select <span style="font-weight: bold;">Advanced Configuration \>
    Workflow Message Summary</span> in the *Navigation*pane.

2.  Click **Add.**
    
    *[View the field descriptions for the Workflow Message Summary
    page](../Page_Desc/WorkFlow_Message_Summary_H)*

3.  Enter the user-friendly name of the workflow in the **WORKFLOW
    NAME** field.

4.  Select a message type from the **MESSAGE TYPE ID** list box to
    determine the type of workflow message to send to users.

5.  Click **Save.**

6.  Click the **Vertical View** icon to configure the workflow message.

7.  Click **Edit** on the Page toolbar.
    
    [View the field descriptions for the Workflow Message Summary page's
    Vertical View](../Page_Desc/WorkFlow_Message_Summary_H)

8.  Select a schedule from the **Schedule ID** list box to control when
    the workflow email is sent. These schedules are defined in Common.
    Refer to [Create
    Schedules](../../../Platform/Common/Use_Cases/Create_Schedules)
    fro detailed information.

9.  Enter text to display in the body of the workflow email in the
    **Workflow Body Template** field. Use standard dynamic substitution
    enclosed in hashtags (\#) to customize the workflow body at run
    time.

10. Enter a color code in the **Workflow Header Color** field to
    configure the color of the header column in the workflow message.

11. Enter a color code in the **Workflow Row Color** to field configure
    the color of the row color in the workflow message.
    
    **NOTE**: Text within workflow messages is converted into HTML
    tables in the workflow email. Use the **Workflow Header Color** and
    **Workflow Row Color** fields to configure the table colors. Use BG
    color codes and this standard: bgcolor-\#\[color code\].

12. Click **Save.**

Continue with Add Users to Workflow Message.

## <span id="Add"></span>Add Users to Workflow Message

A user’s email address is pulled from their user profile created in
System Administration.

To add users to the workflow message:

1.  From the *[Workflow Message
    Summary](../Page_Desc/WorkFlow_Message_Summary_H)* page’s
    *Horizontal* View, click the **Users** icon for the workflow name.

2.  The page opens in Add mode if no users have been added. If users
    exist on the page, click **Add.**

3.  Select a user name from the **USER ID** list box. The user must be a
    valid user set up in System Administration with security to Console.
    
    [View the field descriptions for the Workflow Message Summary User
    page](../Page_Desc/WorkFlow_Message_Summary_User)

4.  Click **Save**.

Continue with Register Workflow Views.

## <span id="Register"></span>Register Workflow Views

The workflow views must be created and registered in System
Administration before being added to the workflow summary.

To register workflow views in Console:

1.  From the **[Workflow Message
    Summary](../Page_Desc/WorkFlow_Message_Summary_H)*
    page’sHorizontal* View, click **Views** for the workflow name.

2.  Click **Add** on the Page toolbar.
    
    [View  the field descriptions for the Workflow Summary Views
    page](../Page_Desc/WorkFlow_Summary_Views_H)

3.  Enter a sort order in the **PRIORITY** field to control the order in
    which the view is run, if more than one view is registered for a
    single workflow message.

4.  Select a data source from the **DATA SOURCE ID** list box that
    indicates where the workflow views are stored.

5.  Select a view from the **VIEW NAME** list box.

6.  Click **Save** on the Page toolbar.

7.  Click the **Vertical View** icon to further configure the view
    registration.

8.  Click **Edit** on the Page toolbar.
    
    [View the field descriptions for the WorkFlow Summary Views Vertical
    View](../Page_Desc/WorkFlow_Summary_Views_H)

9.  Enter a title for the summary information that will appear in the
    workflow for this view in the **Title** field.

10. Enter a sort order used to sort the data in the workflow in the
    **Order BY** field.

11. Click **Save**.

Continue with Process Workflow.

## <span id="Process"></span>Process Workflow

The workflow is configured to run on a schedule (configured in the
Schedule ID field). The NEXT RUN TIME field displays the next date and
time the workflow is scheduled to run. However, the workflow can also be
run immediately, ignoring the Next Run Time.

To process a workflow message immediately:

1.  From the *[Workflow Message
    Summary](../Page_Desc/WorkFlow_Message_Summary_H)* page’s
    *Horizontal* View, click the **Process** icon for the workflow name;
    a confirmation message displays.
2.  Click **Ok**.
