+++
title = 'Send Workflow Notifications When a Post Fails or Succeeds'
solution = 'Data Quality'
+++

# Send Workflow Notifications When a Post Fails or Succeeds

Requests are workflow-enabled, meaning that each user assigned to a role
in a request receives a notification when the tasks assigned to that
role have work assigned.

By default, dspConduct™ does not send notifications when a request has
succeeded or failed to post (i.e., when the request’s posting status is
Success or Failed).

A Designer can configure settings at the scenario role level or the
request role level for the Post role that determine if users registered
in the platform or external users (users who are not registered and
cannot log in to the product) receive a notification when a request
posts successfully or fails to post.

For example, these notifications can alert users who do not access
dspConduct™ that a material was successfully created. They could also
inform users who are not assigned to a role for the request about
posting success or failure.

The text of these workflow messages is set on the
<span style="font-style: italic;">[Category Workflow Language
Message](../Page_Desc/Category_Workflow_Language_Message_H.htm)</span>
page for the Posted and Posted with Errors events.

<span style="font-weight: bold;">NOTE</span>: Workflow notifications are
sent as emails only. A user’s workflow receipt options are not used when
sending messages of this type.

<span style="font-weight: bold;">NOTE</span>: If the workflow
notification contains a link, a user may log in to the DSP® using a
valid user name and password to complete a task or view information. If
the user is an external user, a login and password must be provided
on-site if that user must access the platform via the email’s workflow
link.

<span style="font-weight: bold;">NOTE</span>: When users are added on
the <span style="font-style: italic;">[Post Workflow
Notification](../Page_Desc/Post_Workflow_Notification.htm)</span> page,
those users are also added to the
<span style="font-style: italic;">[Request Post Workflow
Notification](../Page_Desc/Request_Post_Workflow_Notification.htm)</span>
page. On that page, a user must be set as active to receive the
notifications. Users are set to receive these notifications by default.

<span style="font-weight: bold;">NOTE</span>: Sending these types of
notifications is optional.

**NOTE**: When using Auto Post, the Post Workflow Notification records
at the specific Scenario's Post role are used to determine which users
receive posting success or failure notifications.

To send workflow messages when a post fails or succeeds:

  - [Add Task "Request Post Workflow Notification" to the Post
    role](#Add_Task_Request_Post_Workflow_Notification_to_the_Post_Role)
  - [Configure Users who Receive Workflow Notifications at the Scenario
    Role
    Level](#Configure_Users_who_Receive_Workflow_Notifications_at_the_Scenario_Role_Level)
  - [Configure Users who Receive Workflow Notifications at the Request
    Role
    Level](#Configure_Users_who_Receive_Workflow_Notifications_at_the_Request_Role_Level)

## <span id="Add_Task_Request_Post_Workflow_Notification_to_the_Post_Role"></span>Add Task "Request Post Workflow Notification" to the Post Role

For users to receive notifications for posting success or failure, the
dspConduct™ task Request Post Notification must be added to the Post
role.

For Request Post Workflow Notifications to be sent, the Designer must
set the priority of the Request Post Workflow Notification Task as the
lowest priority for the Post role (i.e., the Request Post Workflow
Notification task must be the first task assigned to the Post role).

To add the Request Post Workflow Notification task to the Post role:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    category.

3.  Click the <span style="font-weight: bold;">Tasks</span> icon for a
    Post role.

4.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Role (Tasks)
    page](../Page_Desc/Role_Task.htm)

5.  Enter the priority for the task in the
    <span style="font-weight: bold;">PRIORITY</span> field.
    
    **NOTE:** This task must be set as the first task in the Post role
    (i.e., have the lowest priority)

6.  Select <span style="font-weight: bold;">Request Post Workflow
    Notification</span> in the <span style="font-weight: bold;">TASK ID
    </span>combo box.

7.  Click
<span style="font-weight: bold;">Save</span>.

## <span id="Configure_Users_who_Receive_Workflow_Notifications_at_the_Scenario_Role_Level"></span>Configure Users who Receive Workflow Notifications at the Scenario Role Level

Configuring these settings at the scenario role level allows them to be
set once for any request based on the scenario role. After a Designer
saves a record at the scenario role level, the user is added to the
[Request Post Notification
Workflow](../Page_Desc/Request_Post_Workflow_Notification.htm) page.

The Designer can also configure all of these settings at the request
role level without adding them at the scenario role level.  Refer to
[Configure Users who Receive Workflow Notifications at the Request Role
Level](#Configure_Users_who_Receive_Workflow_Notifications_at_the_Request_Role_Level)
for more information.

**NOTE**: Before performing this task, the Designer must access the
<span style="font-style: italic;">[Category Workflow Language
Message](../Page_Desc/Category_Workflow_Language_Message_H.htm)</span>
page once for notifications to be sent. On this page, the Designer can
set the email address that sends the notifications for events, including
the Posted and Posted with Errors event used with these types of
notifications. The default language for notifications is English. If the
text of the notifications is in another language, the Designer must add
the translated text for that message. Refer to [Create Language-specific
Workflow Messages for a
Category](Create_Language-specific_Workflow_Messages_for_a_Category.htm)
for more information. 

To configure a user who can receive notification emails for posting
success or failure for the Post role:

1.  Click <span style="font-weight: bold;">dspConduct \> Design</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Scenarios</span> icon for
    a category.

3.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    scenario.

4.  Click <span style="font-weight: bold;">Vertical View</span> for the
    Post role.

5.  Click the <span style="font-weight: bold;">Post Workflow
    Notification</span> icon.

6.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Post Workflow Notification
    page](../Page_Desc/Post_Workflow_Notification.htm)

7.  If the user is an external user, enter the ID of the external user
    in the <span style="font-weight: bold;">USER ID</span> combo box.
    
    **NOTE:** The user ID cannot match any ID already registered in the
    platform.
    
    OR
    
    Select the user ID of the registered user from the
    <span style="font-weight: bold;">USER ID</span> combo box.

8.  If the user is an external user, enter the external user’s name in
    the <span style="font-weight: bold;">USER NAME</span> combo box.
    
    OR
    
    Select the user name of the registered user from the
    <span style="font-weight: bold;">USER NAME</span> combo box.

9.  If the user is an external user, enter the external user’s address
    in the <span style="font-weight: bold;">E MAIL ADDRESS</span> combo
    box.
    
    OR
    
    Select the email address registered to the registered user in the
    platform in the <span style="font-weight: bold;">E MAIL
    ADDRESS</span> combo box.

10. Select the language of the workflow message in the
    <span style="font-weight: bold;">LANGUAGE ID</span> list box.
    
    **NOTE**: Workflow messages must have been added for that language
    to the [Category Workflow Language
    Message](../Page_Desc/Category_Workflow_Language_Message_H.htm)
     page for the Posted and Posted with Errors event. If they are not
    added, the notifications are not sent. Refer to [Create
    Language-specific Workflow
    Messages](Create_Language-specific_Workflow_Messages_for_a_Category.htm)
    for more information.

11. Click the <span style="font-weight: bold;">SEND POST SUCCESS</span>
    check box to enable it, if needed.
    
    **NOTE**: The notification is sent when the posting status is
    Success.

12. Click the <span style="font-weight: bold;">SEND POST FAIL</span>
    check box to enable it, if needed.
    
    **NOTE:** The notification is sent when the posting status is
    Failed.

13. Click <span style="font-weight: bold;">Save</span>.

**NOTE:** Any updates to registered user information on this page is not
reflected in the user’s account information. If, for example, the
Designer updates the email address on this page for a user registered in
the platform, the email address associated with that user account is not
updated.

## <span id="Configure_Users_who_Receive_Workflow_Notifications_at_the_Request_Role_Level"></span>Configure Users who Receive Workflow Notifications at the Request Role Level

Configuring these settings at the request role level allows them to be
set for any request based on the role.

**NOTE**: Before performing this task, the Designer must access the
<span style="font-style: italic;">[Category Workflow Language
Message](../Page_Desc/Category_Workflow_Language_Message_H.htm)</span>
page once for notifications to be sent. On this page, the Designer can
set the email address that sends the notifications for events, including
the Posted and Posted with Errors event used with these types of
notifications. The default language for notifications is English. If the
text of the notifications is in another language, the Designer must add
the translated text for that message. Refer to [Create Language-specific
Workflow Messages
f](Create_Language-specific_Workflow_Messages_for_a_Category.htm)or more
information. 

To configure an external or registered user who can receive notification
emails for posting success or failure for the Post role:

1.  Click **dspConduct \> Requests** in the *Navigation* pane.

2.  Click the **Roles** icon for a request.

3.  Click **Vertical View** for the Post role.

4.  Click the **Request Post Workflow Notification** button.
    
    **NOTE:** The button is disabled until the Review role is finished
    and the Post role has started.
    
    **NOTE:** The dspConduct™ task Request Post Workflow Notification
    must have been added to the role for this button to display. Refer
    to [Add Task Request Post Workflow Notification to the Post
    Role](Send_Workflow_Notifications_when_a_Post_Fails_or_Succeeds.htm#Add_Task_Request_Post_Workflow_Notification_to_the_Post_Role)
    for more information.

5.  Click **Add**.
    
    [View the field descriptions for the Request Post Workflow
    Notification
    page](../Page_Desc/Request_Post_Workflow_Notification.htm)

6.  If the user is an external user, enter the ID of the external user
    in the **USER ID** combo box.
    
    **NOTE:** The user ID cannot match any ID already registered in the
    platform.
    
    OR
    
    Select the user ID of the registered user from the
    <span style="font-weight: bold;">USER ID</span> combo box.
    
    **NOTE:** The USER NAME, E MAIL ADDRESS, and LANGUAGE ID fields are
    populated based on the selected registered user ID. If the
    registered DSP user does not have an associated Name, Email Address
    or Language setting then edit the record and update these values on
    the page.

7.  If the user is an external user, enter the external user’s name in
    the **USER NAME** combo box.:
    
    **NOTE:** The name entered in the **USER NAME** field will be used
    in the notification email and is a required field that cannot be set
    to NULL.

8.  the user is an external user, enter the external user’s address in
    the **E MAIL ADDRESS** combo box.

9.  Select the language of the workflow message in the **LANGUAGE ID**
    list box.
    
    **NOTE:** Workflow messages must have been added for that language
    to the *[Category Workflow Language
    Message](../Page_Desc/Category_Workflow_Language_Message_H.htm)*
    page for the Posted and Posted with Errors event. If they are not
    added, the notifications are not sent. Refer to [Create
    Language-specific Workflow
    Messages](Create_Language-specific_Workflow_Messages_for_a_Category.htm)
    for more information.:
    
    **NOTE:** The languages that display in the list box are active
    languages in the platform set on the *Languages* page in System
    Administration.

10. Click the **SEND POST SUCCESS** check box to enable it, if needed.
    
    **NOTE:** The notification is sent when the posting status is
    Success.

11. Click the **SEND POST FAIL** check box to enable it, if needed.
    
    **NOTE:** The notification is sent when the posting status is
    Failed.

12. Click the **ACTIVE** check box to disable it if the user should not
    receive the notifications.

13. Click **Save**

**NOTE:** Any updates to registered user information on this page is not
reflected in the user’s account information. If, for example, the
Designer updates the email address on this page for a user registered in
the platform, the email address associated with that user account is not
updated.
