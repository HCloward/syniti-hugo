+++
title = 'Configure a Registered User to Receive Notifications For Posting Success or Failure at the Request Role Level'
solution = 'Master Data Management'
+++

# Configure a Registered User to Receive Notifications For Posting Success or Failure at the Request Role Level

A Designer can configure settings at the request role level for the Post
role that determine if users registered in the platform receive a
notification when a request posts successfully or fails to post. To add
a registered DSP user to the *Request Post Workflow Notification* page,
select the User ID from the USER ID field then save the record. The DSP
populates the NAME, EMAIL ADDRESS and LANGUAGE fields based on the user
settings.

**NOTE:** If the registered DSP user does not have an associated Name,
Email Address or Language setting, or if these fields are set to NULL,
then edit the record and update these values on the page.

After saving the record for the user, set the SEND POST SUCCESS or / and
the SEND POST FAIL check boxes for the user as applicable to the message
notification requirements.

Refer to Configure Users who Receive Workflow Notifications for
Successful or Failed Postings at the Request Role Level for general
information.

To register a user in the platform who can receive notification emails
for posting success or failure for the Post role:

1.  Click <span style="font-weight: bold;">dspConduct \> Requests</span>
    in the <span style="font-style: italic;">Navigation</span> pane.

2.  Click the <span style="font-weight: bold;">Roles</span> icon for a
    request.

3.  Click <span style="font-weight: bold;">Vertical View</span> for the
    Post role.

4.  Click the <span style="font-weight: bold;">Request Post Workflow
    Notification</span> button.
    
    **NOTE:** The button is disabled until the Review role is finished
    and the Post role has started.:
    
    **NOTE:** dspConduct™ Task Request Post Workflow Notification must
    have been added to the role for this button to display. Refer to
    [Add Task Request Post Workflow Notification to the Post
    Role](Send_Workflow_Notifications_when_a_Post_Fails_or_Succeeds.htm#Add_Task_Request_Post_Workflow_Notification_to_the_Post_Role)
    for more information.

5.  Click <span style="font-weight: bold;">Add</span>.
    
    [View the field descriptions for the Request Post Workflow
    Notification
    page](../Page_Desc/Request_Post_Workflow_Notification.htm)

6.  Select the user ID from the <span style="font-weight: bold;">USER
    ID</span> combo box.
    
    **NOTE:** The USER NAME, E MAIL ADDRESS, and LANGUAGE ID fields are
    populated based on the selected user ID. If the registered DSP user
    does not have an associated Name, Email Address or Language setting
    then edit the record and update these values on the page..
    
    **NOTE:** Workflow messages must have been added for that language
    to the [Category Workflow Language
    Message](../Page_Desc/Category_Workflow_Language_Message_H.htm)
     page for the Posted and Posted with Errors event. If they are not
    added, the notifications are not sent. Refer to [Create
    Language-specific Workflow
    Messages](Create_Language-specific_Workflow_Messages_for_a_Category.htm)
    for more information.

7.  Click the <span style="font-weight: bold;">SEND POST SUCCESS</span>
    check box to enable it, if needed.
    
    **NOTE:** The notification is sent when the posting status is
    Success.

8.  Click the <span style="font-weight: bold;">SEND POST FAIL</span>
    check box to enable it, if needed.
    
    **NOTE:** The notification is sent when the posting status is
    Failed.

9.  Click the **ACTIVE** check box to disable it if the user should not
    receive the notifications.

10. Click <span style="font-weight: bold;">Save</span>.

**NOTE:** Any updates to registered user information on this page is not
reflected in the user’s account information. If, for example, the
Designer updates the email address on this page for a user registered in
the platform, the email address associated with that user account is not
updated.
