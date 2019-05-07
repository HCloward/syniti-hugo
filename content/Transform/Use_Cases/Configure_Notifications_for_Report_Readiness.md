+++
title = 'Configure Notifications for Report Readiness'
solution = 'Migration'
+++

# Configure Notifications for Report Readiness

A user can receive a workflow notification when a report is ready for
review. The DSP® sends a report readiness notification to the Business
users assigned to the report automatically when an error report contains
records.

The notification can also be sent manually.

To configure notifications, at a high level:

  - [Configure Subject and Body of the
    Notification](#Configure_Subject_and_Body_of_the_Notification)
  - [Assign a User as a Notification
    Recipient](#Assign_a_User_as_a_Notification_Recipient)
  - [Send Workflow Notification for Report Readiness
    Manually](#Send_Notifications_Manually)

## <span id="Configure_Subject_and_Body_of_the_Notification"></span>Configure Subject and Body of the Notification

The standard workflow template can be updated to change the workflow
notification email’s subject or body text.

To configure the subject and body of the workflow in Transform:

1.  Click the **Objects** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.

2.  Click the **Report Readiness Notification** icon for an object.

3.  Click the **Workflow Template** icon on the *[Report Readiness
    Notification](../Page_Desc/Report_Readiness_Notification.htm)*
    page's Page toolbar.

4.  Click **Edit**.
    
    [View the field descriptions for the Workflow Template
    page](../Page_Desc/Workflow_Template_Transform.htm)

5.  Enter text in the **Subject** field.

6.  Enter text in the **Body** field.
    
    **NOTE:** The body of the Workflow Template can be modified as the
    user chooses. If they are present, the hash tags represent values
    that will be replaced by the platform. Available replacement values
    are \#Wave\#, \#ProcessArea\#, \#Object\#, and \#Targets\#. They
    will be replaced with values relevant to the context selected in the
    Context bar.

7.  Click **Save**.

**NOTE:** Return the Workflow Template to its default setting by
clicking the **Reset Workflow Template to Default** icon on the
*[Workflow Template](../Page_Desc/Workflow_Template_Transform.htm)*
page.

## <span id="Assign_a_User_as_a_Notification_Recipient"></span>Assign a User as a Notification Recipient

To receive the workflow notification when an actionable report has
records that must be reviewed, the user must be set as a recipient of
the notification.

To set a user as a recipient of the notification in Transform:

1.  Click the **Objects** icon in the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.
2.  Click the **Report Readiness Notification** icon for an object.
3.  Select the desired **USER NAME**.
4.  Click the **Add Recipient** icon (“**+**” symbol); a check mark
    displays in the **RECIPIENT** column for the selected user.

**NOTE:** Stop the workflow notifications from being sent to a user by
selecting that user and clicking the **Remove Recipient** icon on the
Page
toolbar.

## <span id="Send_Notifications_Manually"></span>Send Notifications Manually

The DSP® sends a report readiness notification to the Business users
assigned to the report automatically when an error report contains
records.

The notification can also be sent manually.

To manually send a workflow notification to selected recipients in
Transform:

1.  Click the **Objects** icon on the *[Process Area
    Launch](../Page_Desc/Process_Area_Launch.htm)* page.
2.  Click the **Report Readiness Notification** icon for an object.
3.  Click the **Send Notification** icon; a confirmation message
    displays.
4.  Click **OK**.

An email is sent to the selected user(s) containing the Subject and Body
from the Workflow Template.
